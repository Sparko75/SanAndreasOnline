# San Andreas Online

**Created by [TFM]Sparko75.**

Single-player GTA San Andreas life, brought into SA-MP and shared with your friends. A client-side mod: nothing is
needed on the SA-MP server, everyone who wants to play together installs it.

- **Sessions** with your friends - private groups; if the host leaves, another player takes over
- **Street life** - the city's own pedestrians and traffic, the same for everyone in the session
- **Rockstar's minigames, together** - pool, basketball, dancing, lowriders, soccer
- **A smartphone** (P) - FaceTime video calls, Messages with reactions, Maps with GPS, Music with speakers others
  hear, Camera, Pulse (a social network)
- **Interactions** - hold H next to a player: handshake, high five, dance together, hold hands...
- **Every language** - names, chat and typing in any script; Arabic and Hebrew read right to left

## Install

1. Download the latest **SanAndreasOnline_vX.Y.Z.zip** from [Releases](../../releases/latest).
2. Close the game, extract the zip into your GTA San Andreas folder (the one with `gta_sa.exe`) - its `moonloader`
   folder merges into yours.
3. Start SA-MP and join a server: *"San Andreas Online is ready - press F2 or type /sao"*.

Needs GTA SA 1.0 US, SA-MP 0.3.7 (R1-R5) or 0.3.DL, MoonLoader 026.5-beta with an ASI loader (the tested ones are in
the zip's `optional` folder). No installer, no program of its own: Lua scripts and mimgui's standard DLL.

## Updates

The game looks for updates by itself and **asks** you first ("Update available - update now?", then "reload now?").
It downloads them from this repository's releases - or, if GitHub cannot be reached, from the project's relay server
or through the mod's own relay connection. Whatever the source, an update installs only if:

- `manifest.sig` is a valid ECDSA P-256 signature of `manifest.json` by the key built into the mod (checked by
  Windows' own cryptography) - releases are signed on the release PC only; neither GitHub nor the relay can make one
- its sequence number is higher than the installed one (no downgrade)
- every file is a mod file (an allow-list of paths), with exactly the size and SHA-256 the signed manifest lists
- every Lua file compiles - and it installs all or nothing

## Privacy

- Problem reports (errors, freezes, crashes - with where it crashed) help fix the mod. They come with your nickname,
  so the developer can find your logs and help you - never your IP address, folder names or chat. Settings > Logs
  turns them off. The developer can also ask you in game for your logs: nothing is sent unless you accept.
- Privacy & Safety (phone or Settings): who sees you online, who can message, call or invite you, blocking, Stealth
  Mode.

## License

San Andreas Online is the work of [TFM]Sparko75 - all rights reserved (see [LICENSE.txt](LICENSE.txt)). You may download it from this page and play with it. You may not re-upload it, modify it, decompile it or present it as your own. The mod checks its own files: changed files are replaced by the official ones.

This page carries the releases only (the mod, already built); the source code is private.

Built on [MoonLoader](https://www.blast.hk/threads/13305/), [mimgui](https://github.com/THE-FYP/mimgui) and SA-MP.
GTA San Andreas is a trademark of Rockstar Games; this project is not affiliated with Rockstar Games or SA-MP.
