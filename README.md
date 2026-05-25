# Paxi Continuation

Paxi Continuation is an unofficial continuation of Paxi, a Minecraft mod for automatically loading global data packs and resource packs.

This branch currently targets Minecraft `1.21` and `1.21.1` with Fabric, Forge, and NeoForge support.

## What It Does

The first time you run Paxi, it creates a `paxi` folder in your Minecraft config directory. Packs placed in that folder are loaded automatically when you play.

Paxi supports:

- global data packs
- global resource packs
- zipped packs
- normal folders that contain a `pack.mcmeta` file

This is useful for modpacks, private servers, and players who want the same packs available across worlds without manually copying them into each save.

## Installation

1. Install the correct mod loader for your Minecraft version.
2. Install any loader dependencies required by the release file.
3. Put the Paxi Continuation jar in your `mods` folder.
4. Launch the game once so the config folder is created.
5. Put global packs inside the generated `config/paxi` folder.
6. Restart the game or reload resources/world data as needed.

## Supported Loaders

This branch is configured for:

- Fabric
- Forge
- NeoForge

Use the jar that matches your loader.

## Downloads

Use the approved Modrinth or CurseForge project page when available. Development builds may also be attached to GitHub releases for this repository.

The original Paxi project page remains useful for general behavior documentation and older supported versions.

## Reporting Issues

Open issues on this continuation repository for bugs in this fork.

Include:

- Minecraft version
- loader and loader version
- Paxi Continuation version
- whether the pack is a data pack or resource pack
- whether the pack is zipped or a folder
- `latest.log` or the crash report

## Building

```bash
./gradlew build
```

Built jars are written to the loader-specific `build/libs` folders.

## Credits

Paxi was originally created by YUNGNICKYOUNG. This continuation keeps the mod available for newer Minecraft versions and loaders.
