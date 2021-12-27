
## Description

This has my [antimicrox](https://github.com/AntiMicroX/antimicroX) setup for mapping an xbox 360 controller => keyboard for Satisfactory.

I'm playing on a bigscreen TV with a [Logitech k400](https://www.amazon.com/Logitech-Wireless-Keyboard-Multi-Touch-Touchpad/dp/B005DKZTMG) so I don't have all the same keys as a full sized keyboard and mouse. I generally have the htpc keyboard in my lap and use it for building and then use the controller for roaming the world.

**I also choose to disable controller input.** I did this from several locations:

* Inside the game's menus (Options > Controls > uncheck "Enable Gamepad Input")
* Disable Steam mapping the Guide button to BPM (Steam > Big Picture Mode > Settings > ?? > disable Guide button in dropdown)
* **With steam and the game closed**, I apply a registry hack in wine to indicate that wine should not share the controller. I have a [reg file](https://raw.githubusercontent.com/zpangwin/antimicro-profiles/master/beyond-good-and-evil/disable-controller-in-current-wineprefix.reg) but `wine regedit <file.reg>` never works for me. You'll need to go to the game's compatdata folder (`<your steam dir>/steamapps/compatdata/526870/pfx`). Then you can either copy it under the drive_c for the wine prefix and run `wine regedit`, choose import/merge from the menu, and manually browser/import the file. Or just **backup** then manually edit the `system.reg` file by searching for `System\\CurrentControlSet\\Services\\winebus` and adding the `"Enable SDL"=dword:00000000` value under that section.

## Non-default keybindings

I generally prefer to keep the default keybindings unless they are overly complicated (e.g. Alt + Left mouse), they are not present on my physical keyboard (numpad, middle mouse, mouse wheel, etc), or I just can't remember them (Flashlight = B?).

Here are my non-default mappings that I had to setup from the game's options menu:

| Action                                      | Default binding         | My remapped binding             |
| :------------------------------------------ | :---------------------- | :------------------------------ |
| Ping                                        | Alt + Left Mouse button | Dot/Period (.)                  |
| Rotate Holo Right (e.g. Counterclockwise)   | Mouse wheel up          | Minus (-)                       |
| Rotate Holo Left (e.g. Clockwise)           | Mouse wheel down        | Equals (=)                      |
| Toggle Photo Mode                           | Middle Mouse            | Alt + Backspace (not used)      |
| Cycle to previous hotbar                    | Alt + Mouse wheel down  | Slash (/)                       |
| Toggle Specified Multi Select               | Thumb Mouse button      | (unchanged/not used)            |
| Flashlight                                  | B                       | L                               |
| (Mod: Hotswap Equipment) Hotswap Parachute  | (empty)                 | P                               |


## Details

Number of Profiles: 1

--------------------------------------------------------

### satisfactory_profile_01.gamecontroller.amgp

Number of Sets: 2

Basic idea is two control "Sets" (or layouts if you prefer). First / main set is for general movement and common actions.

Secondary set is for mostly for building or non-critical actions that are used just enough to warrant avoiding a switch between controller and keyboard.


#### Satisfactory - Set \#1


| Xbox 360 Controller    | Maps to                 | Description |
| :--------------------- | :---------------------- | :------------------------------ |
| Left joystick          | WASD keys               | Movement |
| Right joystick         | Mouse directions        | Look up/down, Pan right/left |
| D-Pad Up               | Period (.) key          | Ping (custom binding) |
| D-Pad Right            | Equals (=) key          | Rotate Holo Counter-Clockwise (custom binding) |
| D-Pad Down             | V key                   | Resource Scanner |
| D-Pad Left             | Minus (-) key           | Rotate Holo Clockwise (custom binding) |
| Right trigger          | Left Mouse button       | Primary Fire/Attack/Place/Build |
| Left trigger           | Right Mouse button      | Secondary Fire |
| A button               | Space key               | Jump |
| B button               | I key                   | Crouch (Slide when running) |
| X button               | Left Control key        | Reload |
| Y button               | Backslash (\\) key      | Interact/Collect |
| Guide button           | L key                   | Dismantle mode |
| Back button            | M key                   | Build menu |
| Start button           | Esc key                 | Main Menu (note: does **not** pause game) |
| Left Bumper            | (Control Set 2)         | Use Set 2 while held |
| Right Bumper           | Middle Mouse button     | Inventory |
| Press Left Stick       | press Left Control      | Run/Walk toggle (requires in-game option to "toggle") |
| Press Right Stick      | L key                   | Flashlight (custom binding) |


#### Satisfactory - Set \#2 (when Left Bumper held)

Note: Joysticks (Movement and Camera) and Trigger controls remain the same in both control sets to give you a fighting change when you get the occasional"oh fuck" situations where you are attacked while messing with something on control set \#2 / antimicro bugs out and locks on control set \#2 (rare but have had it happen a few times).

| Xbox 360 Controller           | Maps to                 | Description |
| :---------------------------- | :---------------------- | :------------------------------ |
| Left Bumper + D-Pad Up        | 1 key                   | Quickslot Item \#1 |
| Left Bumper + D-Pad Right     | 2 key                   | Quickslot Item \#2 |
| Left Bumper + D-Pad Down      | 3 key                   | Quickslot Item \#3 |
| Left Bumper + D-Pad Left      | 4 key                   | Quickslot Item \#4 |
| Left Bumper + A button        | 7 key                   | Quickslot Item \#7 |
| Left Bumper + B button        | 6 key                   | Quickslot Item \#6 |
| Left Bumper + X button        | 8 key                   | Quickslot Item \#8 |
| Left Bumper + Y button        | 5 key                   | Quickslot Item \#5 |
| Left Bumper + Guide button    | M key                   | Open Map (must unlock in Game) |
| Left Bumper + Back button     | 9 key                   | Quickslot Item \#9 |
| Left Bumper + Start button    | 0 key (zero)            | Quickslot Item \#0 |
| Left Bumper + Right Bumper    | O key (O as in Oscar)   | Open Codex |
| Left Bumper + Left Stick      | G key                   | Cycle Nobelisk Ammunition |
| Left Bumper + Right Stick     | P key                   | Hotswap Parachute (mod + custom binding) |
| Left Bumper + Left Trigger    | Slash (/) key           | Cycle to previous hotbar (custom binding) |

--------------------------------------------------------






