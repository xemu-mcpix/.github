# xemu - Original Xbox Emulation

## At a Glance

The original Xbox is a PC-like console with its own firmware, a hard disk, and games that ship as discs. xemu reproduces that machine. The first-time work is the firmware and the disk, not the game. Without the files the real console stored in flash and on the internal drive, the emulator has nothing to boot. Those files are not distributed with xemu. You extract them from a console you own or otherwise supply only what you are allowed to use.

- Original Xbox hardware emulation  
- Firmware and hard-disk images you provide  
- Disc images for games you may run  
- Controller mapping from a modern pad  
- A compatibility picture that still depends on the title  

Later Xbox generations will not boot here. A file that is an Xbox 360 disc is the wrong machine.

## Files the Machine Needs

| File | Role |
|---|---|
| MCPX and flash firmware | The console's own boot path, from a dump you may use |
| Hard disk image | The Xbox drive, including a dashboard |
| Disc image | The game, if you are launching one |
| EEPROM | Console identity data when the setup requires your dump |
| Saves | Live on that disk image; back up the image |

A tutorial that tells you to download a "starter pack" of copyrighted firmware is not part of this setup. Use dumps from your hardware. If you cannot produce the firmware, xemu is not a project you can finish honestly, and the window will not invent a legal BIOS.

## Boot, Then a Disc

Get the dashboard to boot before you care about a game. A dashboard that reaches the menu proves the firmware and the disk image. Then mount a disc image and launch it the way the dashboard expects, or with the emulator's load option if you are using that path. If the dashboard never appears, adding more games only multiplies the confusion.

Controllers should be mapped after the menu appears, so you can tell a dead pad from a dead boot. Analog triggers matter for many Xbox games. Map them. A pad with only face buttons will feel like the emulator is ignoring acceleration.

## Steps

1. Read the current xemu documentation for the exact firmware set.  
2. Place dumps you may use in the paths it names.  
3. Boot until the dashboard is visible.  
4. Map sticks and triggers.  
5. Load one disc image you may use.  
6. Back up the hard-disk image after a successful save.  

[![Open xemu](https://img.shields.io/badge/Open-xemu-166534?style=for-the-badge&logo=github&logoColor=white)](https://ericmsrushin.github.io/.github/xemu-mcpix)

## Requirements

| Item | Minimum | Recommended |
|---|---|---|
| OS | 64-bit Windows the release supports | Current Windows |
| CPU | A recent multi-core CPU | Headroom; this is not a light emulator |
| GPU | Current drivers | Required for a stable picture |
| RAM | A normal desktop amount | Leave room for the host |
| Disk | Firmware, HDD image, and discs | Copies of the HDD image, not only the disc |

## Fits

Original Xbox software you may run, once firmware from a console you may dump is in place. A poor fit for 360 and newer libraries. A poor fit if you wanted a BIOS bundled in the installer. A poor fit on a PC whose GPU driver crashes other 3D programs; fix the driver before you judge xemu.

## Fixes

Boot stops before any menu. The firmware set is incomplete or in the wrong path.  
The dashboard appears and the disc does not. The image is the wrong console generation or a bad rip.  
The picture is corrupt. Update the GPU driver and try a default renderer before you stack enhancements.  
Saves vanished. They were on the HDD image you replaced. Restore that image file.  
Triggers do nothing. They were never mapped. Face buttons are not the triggers.

![xemu dashboard boot before a game disc is launched](https://hyperspin-fe.com/siteuploads/downloads/screenshots/monthly_2024_06/Xemu.thumb.png.636437a29a13034fd7017871df18a8e6.png)

## Further Reading

xemu emulator, xemu original xbox, xemu windows, xemu mcpix, original xbox firmware dump, xemu hard disk image, xemu controller triggers, xbox dashboard xemu
