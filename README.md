# VL BA office 3D-printing manual

We are caring for a good ol' trusty `Prusa i3 MKS` generously provided by @mirosko 🧡.

You can usually find it in the kitchenette area on the 7th floor near the game room.

<!-- TOC -->

* [VL BA office 3D-printing manual](#vl-ba-office-3d-printing-manual)
    * [❓ How it works](#-how-it-works)
    * [🤝 Having someone else print stuff for you](#-having-someone-else-print-stuff-for-you)
    * [Printing stuff yourself](#printing-stuff-yourself)
        * [⚙ Setting up PrusaSlicer](#-setting-up-prusaslicer)
        * [🔪 Slicing](#-slicing)
        * [🔀 Switching the loaded filament](#-switching-the-loaded-filament)
        * [❄ Removing completed prints](#-removing-completed-prints)
        * [🧽 Cleaning the bed](#-cleaning-the-bed)
    * [💔 Common issues](#-common-issues)
        * [Print not sticking to the bed.](#print-not-sticking-to-the-bed)
        * [SD card is not detected](#sd-card-is-not-detected)
        * [Filament won't load](#filament-wont-load)

<!-- TOC -->

---

## ❓ How it works

Currently, using the printer is free-for-all, meaning that if the printer is not printing (and it
doesn't have a sticky-note with some kind of a warning on it), you can use it.

Feel free to edit this manual if you feel something's not right.

## 🤝 Having someone else print stuff for you

Message `#ba-3d-print` slack channel, asking nicely and attaching a model (`.stl` mesh file) you
want to have printed. Check the spools around the printer to see which colors are available.

Most common websites with a huge database of models are [Printables](https://www.printables.com) and
[Thingiverse](https://www.thingiverse.com).

## Printing stuff yourself

1. Slice the mesh (`.stl`) file using PrusaSlicer and put the exported gcode on the printer SD card.
1. Hit `Print from SD` and choose your model.

### ⚙ Setting up PrusaSlicer

1. Check out [this Prusa guide](https://help.prusa3d.com/article/first-print-with-prusaslicer_1753)
   if you haven't already.
1. Install [PrusaSlicer](https://www.prusa3d.com/page/prusaslicer_424/).
1. Download the recommended [settings bundle](configuration/recommended_settings.ini) and import it
   to Slicer via `File` > `Import` > `Import Config Bundle`. This will do most of the configuration
   for you, so unless you want to do some tweaks, you should be ready to slice.

### 🔪 Slicing

Most of the time, you simply:

1. Drag-and-drop your `.stl` model(s) into PrusaSlicer.
1. _Optional:_ if your print has sharp outer corners, you might want to
   configure `Print Settings` > `Skirt and brim` > `Brim`.
1. Hit `Slice now`
1. Hit `Export G-code`

### 🔀 Switching the loaded filament

1. Choose `Preheat` (PLA) from the main menu and wait until the target temperature is reached.
1. Choose `Unload the filament` from the main menu.
1. ⚠️ **Secure the loose end of the filament you just unloaded!**<br>When unloading the filament,
   don't let go of it until it's secured in the spool frame. Otherwise, the filament might become
   tangled - it's hard to notice, and it might do damage to the print, or worse, the printer.
1. Before loading new spool, first clip off the tip if it is bent/deformed.

### ❄ Removing completed prints

1. **Wait until the bed cools down.** This is not so much to protect your fingers (you should handle
   the bed temperature for PLA without issues), but removing the print while it's still hot will
   most likely cause it to bend as it cools.
1. Use the red scraper near the printer to remove the print.<br>⚠️ **Never use any sharp objects to
   do this!**<br>Most of the prints can be simply pulled off from the bed, but the larger the
   contact surface with the bed, the harder it will be.

### 🧽 Cleaning the bed

Occasionally clean the print bed with a paper wipe and a bit of isopropyl-alcohol. This usually
helps if your print failed due to first layer not sticking to the bed.

## 💔 Common issues

### Print not sticking to the bed.

Try [cleaning the bed](#-cleaning-the-bed).

### SD card is not detected

Pull the SD card out, and put it back again, **_gently_**.
This printer likes it slow.

### Filament won't load

When you select `Load filament`, keep holding the filament and push slightly down to help the
loading. The printer likes this part a bit rougher (but don't force it too much).
