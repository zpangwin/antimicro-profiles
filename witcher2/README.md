
## Description

This has my antimicro setup for mapping xbox 360 controller => keyboard for the witcher 2.

unlike most of my antimicro profiles, this does not map all of the keys. Instead it relies on the default controller mappings and just adds an additional custom mapping on the guide button. 

I modified my User.ini and Input_QWERTZ.ini file (on Linux, these are under `${STEAMDIR}/compatdata/20920/pfx/drive_c/users/steamuser/My Documents/Witcher 2/Config/`). It has been awhile since I played and I forget exactly what I changed. I think these may have been intermediate copies I had saved elsewhere on my drive may have been an intermediate copy of the file... I stupidly deleted my game folder awhile back but if I find my mod merge folder, I may create a repo for that.

In my Input_QWERTZ.ini, I have made the following changes (there might be others as well; I recommend comparing mine to the original with WinMerge or Meld or a similar diff tool):

    IK_Pad_DigitDown=(Gamekey=,Value=1.000000)
    IK_Y=(Gamekey=GI_Medallion,Value=1.000000)

The ini files in the repo are from an old email where I had shared my settings with my brother... unfortunately, think the final copies were either not in the email or I attached the wrong file (perhaps I had meant to attach Input_QWERTY instead of Input_QWERTZ?).

I think I may have also had:

    IK_G=(Gamekey=GI_CatToggle,Value=1.000000)

After merging the changes from [this toggleable cat eye effect mod](https://www.nexusmods.com/witcher2/mods/918) into my own custom mod stack. I believe I had moved the Medallion key from "Z" to "Y" for no other reason than that the two were closer together on the keyboard (I was playing primarily with controller but had a htpc keyboard in my lap I would use for less combat focused stuff occasionally). I don't recall why I would have unmapped D-Pad Down unless I was accidentally bumping it or something... I would have guessed myself much more likely to unbind the medallion mapping on the controller to avoid bumping it during combat (especially since I could still use it on the htpc keyboard).

To that should be:

    IK_Pad_LeftThumb=(Gamekey=,Value=1.000000)


In any case, you might need to experiment a bit unless you are just using this for reference.

## Details

Number of Profiles: 1

#### Set \#1

| Xbox 360 Controller    | Maps to                 | Description |
| ====================== | ======================= | =============================== |
| Guide button           | G key                   | custom binding for cat eye effect mod |

Note 1: Everything else was unmapped to avoid conflicts with the default controls (e.g. antimicro was just adding some additional mappings)

Note 2: The "custom binding for cat eye effect mod" requires both the mod and messing with your ini files to map the indentifier to a keyboard key (I chose "G" so I could remember it as "Gamma").

If you want some more drastic changes to the controls, check out a related post on [gaming.stackexchange.com](https://gaming.stackexchange.com/questions/256661/where-are-witcher-2-save-game-files-located) where I cover location of gave saves and config files. In this post, I also link to several anti-micro profiles available on nexus mods.

Alternatively, there was an old deleted steam forum guide [here](https://web.archive.org/web/20170529092930/http://forums.steampowered.com/forums/showthread.php?t=2658771) which I had saved the transcript of in a txt file (included in this folder for convenience). This guide covers how to make some changes to the mappings using the Input_QWERTZ.ini file.
