# MMD Mod Template
A template for modding at MMD, it contains build scripts for testing on pushing commits, actions for releasing builds to CurseForge, Github and the maven MMD uses.

GitHub actions is used for build testing and releasing, releases are made by using Git tags on a commit, tags must always contain the Minecraft version being targeted and the mods version, for example `1.12.2-1.0.0` or `26.1-5.0.0` The Minecraft version is REQUIRED!

This readme is a WIP, feel free to join the Discord server and message Kiri with questions.

[![Discord Badge](https://img.shields.io/badge/Discord-16181C?style=for-the-badge&logo=discord&logoColor=5865F2)](https://discord.moddev.zone)
[![Github Badge](https://img.shields.io/badge/GitHub-16181C?style=for-the-badge&logo=github&logoColor=BBDDE5)](https://github.com/minecraftmoddevelopmentmods/mmd-mod-template)

# Setup
On Windows:

```powershell
.\gradlew.bat eclipse genEclipseRuns
.\gradlew.bat build
```

On Linux or macOS:

```bash
./gradlew eclipse genEclipseRuns
./gradlew build
```

`setupDecompWorkspace` was a ForgeGradle 2 task and is not used by this
template as we use ForgeGradle 7 instead.
