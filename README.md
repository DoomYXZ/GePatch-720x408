# GE Patch Plugin 720x408 edit

This is an experimental plugin for [Adrenaline](https://github.com/TheOfficialFloW/Adrenaline) that allows you to play a few games in native resolution. (not this version)

## Compatibility List

Please help testing games and filling out the [spreadsheet](https://docs.google.com/spreadsheets/d/1aZlmKwELcdpCb9ezI5iRfgcX9hoGxgL4tNC-673aKqk/edit#gid=0).

## Changelog v0.19

- Fixed a small bug that was introduced earlier.
- Fixed a few bugs that caused certain games to crash.

## Installation

- Before you start make sure that you have

  - Adrenaline 7 or higher.
  - The option `Recovery Menu->Advanced->Advanced configuration->Force high memory layout` **DISABLED**.
  - All plugins in `ux0:pspemu/seplugins/game.txt` and `ux0:pspemu/seplugins/vsh.txt` disabled (you can gradually enable them if you think they should not interfere with GePatch. Please be aware that plugins that print stuff to the screen may not be visible with GePatch since the framebuffer is redirected.

- Download [ge_patch.prx](https://github.com/TheOfficialFloW/GePatch/releases) and copy it to `ux0:pspemu/seplugins/`.

- Write this line to `ux0:pspemu/seplugins/game.txt` (`ux0:pspemu` is mounted as `ms0:` in the PSP emu):

  ```
  ms0:/seplugins/ge_patch.prx 1
  ```

  You can also do the same change in file `ux0:pspemu/seplugins/vsh.txt` to get a XMB in higher resolution, but be aware that the VSH menu will be invisible.

## Known Issues

Some games may:

- Not display cutscenes.
- Have a black screen.
- Not display all textures.
- Contain clipping/culling.

## Donation

If you like my work and want to support future projects, you can make a donation:

- via bitcoin `361jRJtjppd2iyaAhBGjf9GUCWnunxtZ49`
- via [paypal](https://www.paypal.me/flowsupport/20)
- via [patreon](https://www.patreon.com/TheOfficialFloW)
