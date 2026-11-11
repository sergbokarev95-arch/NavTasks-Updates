# NavTasks Updates

Official **binary-only** distribution channel for the NavTasks Android application.

- Main application source and signing keys are **not** hosted here.
- Only reviewed, signed Android APK assets, SHA-256 checksums and update-channel metadata are distributed here.
- The `stable` channel does not include beta builds, release candidates, emergency recovery builds or draft releases.
- No Google Play or GitHub sign-in is required to download public stable builds.
- Never uninstall NavTasks to apply an update; Android must verify the existing installed package and signing certificate.
- Keep a full export of your profiles before any major upgrade.

## Channel state

Machine-readable stable metadata: [channels/stable.json](channels/stable.json).

Until the first approved stable release, this file says `"available": false`. **No APK is currently published in this public repository.**

Each future stable release will provide:

- One complete signed APK (no incremental patch chain);
- A matching `.sha256` file;
- Release notes in Russian and English;
- A pinned-version metadata record with the package name, versionCode, APK size, SHA-256 digest and HTTPS download URL.

The installed application must independently verify the **APK signing certificate**, not rely on the SHA-256 from this repository as proof of publisher identity. Updates remain optional, and all application features remain offline-capable.

**Main private development repository:** source access is restricted. Do not upload source code, profile exports, certificates, keystores or credentials here.
