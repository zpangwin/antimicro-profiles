# antimicro-profiles
game profiles for [antimicro](https://github.com/AntiMicro/antimicro)

## Setup notes

i use these with a wireless xbox 360 controller under linux.

you are welcome to adjust them for use on other controllers and antimicro profiles should not be system-dependent unless you are launching apps etc as an action (which I do not and will try to call out if that ever changes).

if you are also under linux and using the same controller, this may require installing the xboxdrv package as it is installed on my system.

In the past, I have installed antimicro v2.23 from the artful deb package in [this launchpad repo](https://launchpad.net/~mdeguzis/+archive/ubuntu/libregeek) without issues on Linux Mint 19.x (Ubuntu 18.04 base). I have also installed it on Linux Mint 20 (Ubuntu 20 base) in a VM without issues but did not test it thoroughly there.

I noticed recently that there is also [another launchpad repo](https://launchpad.net/ubuntu/+source/antimicro) with a build specifically for focal fossa (Ubuntu 20) but have not used or tested this one at the time of writing. As far as I can tell, neither launchpad maintainer is officially affliated with the github project but I could be mistaken.

## Game notes

I will try to add games / mappings as I get time or make new ones. This section will describe anything unusual

* Mass Effect 1: Experimented with creating a template image from an old mapping I had and trying to document some of the changes. Also including my game config files. I confirmed some values against the Proton version of the game on Mint 19.3 but have not actually tested these in-game. Most of the changes had been previously tested in antimicro on windows several years back but there is a small possibility that I messed something up when remapping. Will update if/when I go back and confirm things in-game. On Linux, BIOInput.ini goes in `{SteamDir}/steamapps/compatdata/17460/pfx/drive_c/users/steamuser/My Documents/BioWare/Mass Effect/Config` where SteamDir corresponds to either your custom steam library folder or the default of `~/.local/share/Steam`.

* Witcher 2: For this game, I did not create a full controller mapping. Instead, I opted to use i am letting the game use 80% default controls, 10% remapped controls (removed medallion from left-stick + defined new cat effect hotkey as "G" for Gamma), and 10% new controls defined in antimicro so that I can bind medallion (press) and cat effect (hold) to the guide button (guide button doesn't appear to be bindable via ini's and they don't support custom press/hold mappings). I will also include my game config files for comparison with the game's vanilla ones. Last played using the Proton version of Witcher2 under Linux Mint 19.3 in Jul 2020 and it worked great with no issues that I recall. On Linux, assuming you are using the Proton version rather than the Native version of the game, the ini files go in `{SteamDir}/steamapps/compatdata/20920/pfx/drive_c/users/steamuser/My Documents/Witcher 2/Config` where SteamDir corresponds to either your custom steam library folder or the default of `~/.local/share/Steam`. Also see my write-up of Witcher 2 Save locations + Proton setup [here](https://gaming.stackexchange.com/questions/256661/where-are-witcher-2-save-game-files-located).

* Old Profiles: this applies to: arkham asylum, evoland, fallout3, gothic1, oblivion, and risen1 profiles. I haven't tested these in some time (pretty sure the batman one is ok but don't remember for sure). Some of these are probably from old windows or Mint 18.x-19.1 playthoughs. Most of these are probably fine but some of them might just be duplicates of another profile that I never got around to actually mapping. If anyone feels like testing these, please feel free to submit a ticket saying "tested {file} - works" or "tested {file} - invalid mappings" etc and I will make the appropriate corrections. otherwise, i am unlikely to go back and replay these games just to test out and confirm the profiles.



