<p align="center">
	<img src="https://github.com/4ranger/4ranger-music/blob/master/4RANGER_Music_Github.png" alt="4RANGER Banner" />
	<br />
	<a href="https://github.com/4ranger/4ranger-extras/wiki/Adding-New-Music">
		<img src="https://img.shields.io/badge/4RANGER_Extras_Wiki-How to Add Music-orange.svg?style=for-the-badge&logo=github" alt="Wiki" />
	</a>
	<a href="https://discord.gg/DRaWNyf">
		<img src="https://img.shields.io/discord/532683310409842728.svg?label=Discord&logo=Discord&colorB=7289da&style=for-the-badge" alt="Discord Server">
	</a>
	<a href="https://steamcommunity.com/sharedfiles/filedetails/?id=2265715499">
		<img src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-steam-workshop.jross.me%2F2265715499%2Fsubscriptions-text&style=for-the-badge" alt="Steam Subscriptions">
	</a>
</p>
<p align="center">
	<a href="https://steamcommunity.com/sharedfiles/filedetails/?id=2265715499">
		<img src="https://img.shields.io/steam/size/2265715499?label=Download&logo=steam" alt="Download" />
	</a>
	<a href="https://github.com/4ranger/4ranger-music/releases">
		<img src="https://img.shields.io/github/release/4ranger/4ranger-music.svg?label=Version" alt="Version" />
	</a>
	<a href="https://github.com/4ranger/4ranger-music/issues">
		<img src="http://img.shields.io/github/issues-raw/4ranger/4ranger-music.svg?label=Issues&style=flat" alt="Issues" />
	</a>
	<a href="https://github.com/4ranger/4ranger-music/blob/master/LICENCE">
		<img src="https://img.shields.io/github/license/4ranger/4ranger-music.svg?style=flat&label=Licence" alt="License">
	</a>
</p>
<p align="center"><sup><strong>Making Arma 3 a better place for all members of the 2nd Battalion, Nord Brigade.</strong></sup></p>

## Dependencies
There aren't any dependencies, but the music and sounds are meant to be played through [KLPQ Music Player](https://steamcommunity.com/sharedfiles/filedetails/?id=1241545493), making it a recommended mod.

# For Developers of this mod
## Install
We have a build system to allow for key signing and addon compiling.

### Requirements
1. [Git for Windows](https://git-scm.com/download/win)
1. Windows PowerShell v5.1 or higher

<ins>Automated Process:</ins>

To automatically set up your system and build the mod you can execute the included `build.bat` file.
You can do this by either going to `\tools` and double clicking the `build.bat` file, or if you use VSC you can select the bat file then in the `TERMINAL` at the bottom you can select the `Run Active File` option from the `...` menu.

<ins>Manual Proccess:</ins>

To set up your system to use the build script:
- Open Windows PowerShell as Administrator and execute `set-executionpolicy remotesigned`
- In the future, always use PowerShell as Admin

### Windows
If on Windows, use the `tools\make.ps1` file to build the mod for you. It will build the mod, sign the addons, include the public key in the `keys` folder, and also copy across all files found in the `extras` folder, as well as the files specified in the file `tools\support-files.txt`.

The build script will NOT leave the private key in the `keys` folder. It will delete it instead, to avoid any accidental uploading or distribution.

Be aware, that the names of the `.bisign` and `.bikey` files depend on the latest tag on git. This means that, if you wish to upload a release, it is advised to first tag the latest git commit, and then build the mod. That way you have a nice version, such as `vsc_m_v1.0.3.bikey` rather than `vsc_m_v1.0.3-g0558b0c.bikey`.

## Naming conventions
To make the names of this mod less likely to run into problems in the future regarding the inclusion of a number in the name:
- for code: bnb_m
- for urls: 4ranger-music
- for presentation: 4RANGER Music

### Prefixes
The prefix `vsc_m_` should be used where appropriate to avoid any potential name clashes with other mods.

## Credits
4RANGER Mod Team
