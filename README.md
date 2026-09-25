<p align="center">
  <img src="https://i.ibb.co.com/C3yD50ZX/IMG-20260925-130809-688.jpg" width="128" height="128" alt="Vanta">
</p>

<h1 align="center">Vanta Launcher</h1>

<p align="center">
  An independent Android launcher framework for users who does NOT own Minecraft or own Minecraft: Java Edition and want to run Java Edition on Android devices. 
</p>

<p align="center">
  <strong>NOT AN OFFICIAL MINECRAFT PRODUCT.</strong><br>
  <strong>NOT APPROVED BY OR ASSOCIATED WITH MOJANG, MICROSOFT, XBOX, OR THE POJAVLAUNCHER PROJECT.</strong>
</p>

---

## About

Vanta Launcher is developed by **@mysteriousGUYbruh** and **@nanowx26** as an independent Android launcher framework and compatibility project.

This project is not affiliated with, endorsed by, sponsored by, reviewed by, or approved by Microsoft, Mojang, Xbox, Minecraft, PojavLauncher, Boardwalk, Amethyst, MojoLauncher, Zalith Launcher, Fold Craft Launcher, or any other third-party launcher project.

Minecraft, Microsoft, Xbox, Mojang, and related names, services, trademarks, and assets are property of their respective owners.

---

## What this repository contains

This repository is intended to contain the public launcher-side framework for Vanta Launcher, including Android UI, settings, instance management, renderer configuration, input handling, legal screens, and compatibility scaffolding.

Depending on the branch, release, or build configuration, this repository may include experimental or in-progress launcher components.

The public project focuses on:

- Android-native launcher UI and instance management.
- Local launcher settings and instance state management.
- Version metadata models and compatibility structures.
- Java runtime and LWJGL integration scaffolding for Android.
- Renderer/runtime compatibility work for Android devices.
- Touch, input, surface, and lifecycle bridge work required to run Java games on Android.
- Mod, modpack, resource pack, shader pack, and world management UI/framework code.
- Legal, privacy, and open-source notice screens.

---

## Recommended private files:

```text
local.properties
keystore.properties
signing.properties
secrets.properties
.env
*.jks
*.keystore
```

---

## Open-source lineage and credits

Vanta Launcher is NOT a DNA Mobile Applications project, but Android Minecraft: Java Edition launchers have a long open-source history.

This repository contains or may contain code, compatibility ideas, runtime integration patterns, API bridge behavior, input/surface handling, or implementation details that are copied from, modified from, derived from, studied from, or inspired by other open-source projects.

Where code is copied, modified, ported, or derived from another project, the original license and notices must be preserved.

See [`OPEN_SOURCE_NOTICES.md`](OPEN_SOURCE_NOTICES.md) for project notices and attribution details.

### PojavLauncher

- Repository: <https://github.com/PojavLauncherTeam/PojavLauncher>
- License: GNU Lesser General Public License v3.0, unless a file says otherwise.
- Relationship: Vanta Launcher may include or adapt launcher-side compatibility interfaces, input/surface bridge ideas, runtime integration patterns, and related Android launcher logic from PojavLauncher.

Any PojavLauncher-derived files must remain under the applicable PojavLauncher license terms. Do not remove source attribution or license notices.

### Boardwalk

- Repository: <https://github.com/zhuowei/Boardwalk>
- License: Apache License 2.0, unless a file says otherwise.
- Relationship: Boardwalk is credited for early Android Minecraft: Java Edition launcher work and historical launcher/runtime concepts that influenced later Android Java launcher projects.

Any Boardwalk-derived files must preserve the Apache License 2.0 notice requirements.

---

## License and source availability

This repository is a mixed-origin source tree.

Files written entirely by DNA Mobile Applications may be licensed separately by DNA Mobile Applications.

Files copied from, modified from, derived from, or based on third-party projects remain subject to their original licenses and notices. That includes files derived from PojavLauncher, Boardwalk, LWJGL, Mesa, GL4ES, Android platform libraries, and other third-party components.

If this repository includes PojavLauncher-derived code, the applicable LGPL-covered source code and modifications must remain available under the LGPL terms.

Before distributing APKs or other binaries, make sure the app includes or links to:

- open-source notices;
- required license texts;
- source-code links required by LGPL/GPL or other applicable licenses;
- the app privacy policy;
- the app terms/legal notice screen; and
- any notices required by files copied or modified from third-party projects.

This README is not legal advice. Review the relevant licenses before commercial distribution or app-store publication.

---

## Privacy

Vanta Launcher is designed to avoid operating a DNA Mobile Applications account server.

Launcher settings, logs, worlds, mods, resource packs, shader packs, and launcher files are intended to remain local to the user’s device unless the user chooses to share, export, upload, or send them through another service.

See `PRIVACY_POLICY.md` for the full privacy policy.

---

## Building

Open the project in Android Studio and let Gradle sync.

Typical local build commands:

```bash
./gradlew assembleDebug
./gradlew assembleRelease
```

On Windows:

```bat
gradlew.bat assembleDebug
gradlew.bat assembleRelease
```

Release builds should be signed with the correct production keystore and should not include debug-only application IDs, private API keys, local paths, or private development configuration.

---

## Contributing

Contributions are welcome if they respect the project’s illegal and technical boundaries.

Do not submit code copied from another launcher or project unless the license permits it and attribution is preserved.

Pull requests that include third-party-derived code should clearly identify:

- the source project;
- the original license;
- the original file or commit if known;
- the files changed in this project; and
- any required notices.
