<p align="center">
  <img src="docs/app_icon.png" alt="DroidBridge app icon" width="128" height="128">
</p>

<h1 align="center">DroidBridge (or GreenBridge) Launcher</h1>

<p align="center">
  An independent Android launcher framework for users who own Minecraft: Java Edition and want to run Java Edition on Android devices. 
</p>

<p align="center">
  <strong>NOT AN OFFICIAL MINECRAFT PRODUCT.</strong><br>
  <strong>NOT APPROVED BY OR ASSOCIATED WITH MOJANG, MICROSOFT, XBOX, OR THE POJAVLAUNCHER PROJECT.</strong>
</p>

---

## About

DroidBridge Launcher is developed by **DNA Mobile Applications** as an independent Android launcher framework and compatibility project.

This project is not affiliated with, endorsed by, sponsored by, reviewed by, or approved by Microsoft, Mojang, Xbox, Minecraft, PojavLauncher, Boardwalk, Amethyst, MojoLauncher, Zalith Launcher, Fold Craft Launcher, or any other third-party launcher project.

Minecraft, Microsoft, Xbox, Mojang, and related names, services, trademarks, and assets are property of their respective owners.

Users are responsible for owning Minecraft: Java Edition and for complying with the Minecraft EULA, Minecraft Usage Guidelines, Microsoft Services Agreement, and any other applicable terms.

---

## What this repository contains

This repository is intended to contain the public launcher-side framework for DroidBridge Launcher, including Android UI, settings, instance management, renderer configuration, input handling, legal screens, and compatibility scaffolding.

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

## What this repository must not contain

Do **not** commit private or user-specific configuration.

The public source tree must not include:

- private authentication credentials;
- production signing keys or keystores;
- private API keys;
- user account tokens or session data;
- local machine paths such as Android SDK paths;
- bundled Minecraft game files, assets, libraries, or proprietary content;
- private endpoint details;
- private production service implementation code; or
- private release-only launcher implementation classes.

Keep private configuration in local files that are ignored by Git.

Recommended private files:

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

## Microsoft account sign-in clarification

Some private or production builds of DroidBridge Launcher may allow users to sign in with a Microsoft account through Microsoft identity services.

A working Microsoft sign-in flow, registered application, redirect URI, or consent screen means only that the launcher uses Microsoft identity services for authentication where that feature is available. It does **not** mean Mojang, Microsoft, Xbox, or Minecraft has approved, endorsed, sponsored, reviewed, or partnered with this launcher.

This public source release does not provide production account-service configuration, private token exchange details, app secrets, private endpoint details, or release-only authentication implementation code.

---

## Open-source lineage and credits

DroidBridge Launcher is a DNA Mobile Applications project, but Android Minecraft: Java Edition launchers have a long open-source history.

This repository contains or may contain code, compatibility ideas, runtime integration patterns, API bridge behavior, input/surface handling, or implementation details that are copied from, modified from, derived from, studied from, or inspired by other open-source projects.

Where code is copied, modified, ported, or derived from another project, the original license and notices must be preserved.

See [`OPEN_SOURCE_NOTICES.md`](OPEN_SOURCE_NOTICES.md) for project notices and attribution details.

### PojavLauncher

- Repository: <https://github.com/PojavLauncherTeam/PojavLauncher>
- License: GNU Lesser General Public License v3.0, unless a file says otherwise.
- Relationship: DroidBridge Launcher may include or adapt launcher-side compatibility interfaces, input/surface bridge ideas, runtime integration patterns, and related Android launcher logic from PojavLauncher.

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

DroidBridge Launcher is designed to avoid operating a DNA Mobile Applications account server.

Launcher settings, logs, worlds, mods, resource packs, shader packs, and launcher files are intended to remain local to the user’s device unless the user chooses to share, export, upload, or send them through another service.

See `PRIVACY_POLICY.md` for the full privacy policy.

---

## App icon in this README

The icon at the top of this README expects this file to exist:

```text
docs/app_icon.png
```

Before publishing, place the PNG app icon at that path so GitHub displays it correctly.

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

Contributions are welcome if they respect the project’s legal and technical boundaries.

Do not submit code copied from another launcher or project unless the license permits it and attribution is preserved.

Pull requests that include third-party-derived code should clearly identify:

- the source project;
- the original license;
- the original file or commit if known;
- the files changed in this project; and
- any required notices.

---

## Legal disclaimer

This project is not an official Minecraft product and is not approved by or associated with Mojang, Microsoft, Xbox, or Minecraft.

This README is not legal advice. Before commercial distribution or app-store publication, review all third-party licenses, Microsoft/Minecraft terms, Google Play policies, and any store-specific requirements that apply to your release.
