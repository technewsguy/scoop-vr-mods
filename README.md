# VR mods – a Scoop bucket

Install and update technewsguy's VR projects with [Scoop](https://scoop.sh) or [UniGetUI](https://github.com/marticliment/UniGetUI) (formerly WingetUI).

| Package | What it is |
|---|---|
| `nslt-vr` | [NSLT-VR](https://github.com/technewsguy/NSLT-VR): VR mod for **New Super Lucky's Tale** (Steam) |
| `rollingquest-vr` | [Rolling Quest VR](https://github.com/technewsguy/RollingQuest-VR): VR mod for **Rolling Quest** (itch.io) |
| `shmcd-vr` | [SHMCD-VR](https://github.com/technewsguy/SHMCD-VR): VR mod for **SUPERHOT: MIND CONTROL DELETE** (Steam) |
| `fez-vr` | [FEZ-VR](https://github.com/technewsguy/FEZ-VR): VR mod for **FEZ** (Steam), the game as a 3D diorama |
| `shattervr` | [ShatterVR Runtime](https://github.com/technewsguy/ShatterVR-Runtime): plays the **Smash Hit** Gear VR build on PC VR (bring your own APK) |

New releases of each project show up here automatically within a few hours.

## UniGetUI

1. **Settings → Package managers → Scoop.** If Scoop isn't installed yet, UniGetUI offers to install it.
2. Under **Buckets**, add a bucket named `vrmods` with the URL `https://github.com/technewsguy/scoop-vr-mods`.
3. Search for `nslt-vr`, `rollingquest-vr`, `shmcd-vr`, `fez-vr` or `shattervr` and install. Updates and uninstalls then work like any other package.

## Command line

```powershell
scoop bucket add vrmods https://github.com/technewsguy/scoop-vr-mods
scoop install vrmods/nslt-vr
scoop install vrmods/rollingquest-vr
scoop install vrmods/shmcd-vr
scoop install vrmods/fez-vr
scoop install vrmods/shattervr
```

## What each package does

**nslt-vr**
- Finds New Super Lucky's Tale through your Steam libraries and runs NSLT-VR's installer.
- Play with the **New Super Lucky's Tale VR** shortcut.
- Start menu: **NSLT-VR - Add to Steam** adds the VR version to your Steam/SteamVR library with artwork. Steam closes and restarts while it runs.
- Game somewhere unusual? Set `NSLTVR_GAMEDIR` to its folder.

**rollingquest-vr**
- Finds your Rolling Quest folder. It looks in the itch app's folder and the usual places, or asks you to pick it, and then remembers it.
- Installs the mod and BepInEx into that folder.
- Start menu: **Rolling Quest VR - Add to Steam** adds **Rolling Quest VR** to Steam/SteamVR with artwork, plus a desktop shortcut.
- To use a specific folder, set `ROLLINGQUEST_DIR`.

**shmcd-vr**
- Finds SUPERHOT: MIND CONTROL DELETE through your Steam libraries and runs SHMCD-VR's installer (BepInEx 5 x86, the mod, VR switched on in the game data).
- Needs **Python 3** once for that last step (Scoop suggests `main/python`); originals are kept as `*.orig`.
- Start SteamVR, then the game. Start menu: **SHMCD-VR - Add to Steam** adds **SUPERHOT: MIND CONTROL DELETE VR** to Steam/SteamVR with artwork. Steam closes and restarts while it runs.
- Game somewhere unusual? Set `SHMCDVR_GAMEDIR` to its folder.

**fez-vr**
- Finds FEZ through your Steam libraries and adds the mod next to `FEZ.exe` (FEZ's own files are not changed).
- The first install adds **FEZ VR** to Steam and SteamVR with FEZ's artwork, plus desktop / Start menu shortcuts. Steam closes and restarts once; updates don't restart it.
- Play **FEZ VR**; regular FEZ stays flat. Game somewhere unusual? Set `FEZVR_GAMEDIR` to its folder.

**shattervr**
- Installs ShatterVR with a Start menu shortcut.
- Copy your own Smash Hit Gear VR APK to the install folder as `game.apk`. Scoop shows the path after installing.
- The APK is kept when ShatterVR updates or is uninstalled.

**Updating and uninstalling:** updating the mods replaces only the mod files. Uninstalling removes them from the game folder again. A Steam entry added with "Add to Steam" is removed in Steam: right-click it > *Manage* > *Remove non-Steam game*.

## Support

These are free, unofficial fan projects. If you enjoy them: [ko-fi.com/technewsguy](https://ko-fi.com/technewsguy)
