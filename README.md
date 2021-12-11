# Minecraft Server 

docker-compose for the Forge modded server with a couple of mods installed and a sidecar for backup/restore to Amazon S3.

Using the following Docker images: 
- itzg/minecraft-server:latest
- quay.io/spesnova/dockup:latest 
- quay.io/spesnova/dockup:latest

( See docker-compose.yml )

## Quickstart

```
docker-compose up
```

Ensure `/server` dir has proper permissions:

On Windows: `takeown /F server /A /R` 
On Linux/OSX: `chown -R server`

**NOTE**: By providing EULA=TRUE you agree to the EULA at https://account.mojang.com/documents/minecraft_eula.

## Environment Variables
- EULA (Required)
  - Default: none

## Docs / Guides

See [client-setup-guide.md](docs/client-setup-guide.md) to setup your minecraft client.

## Mods List

| Mod Name                                                                            | Mod File Path                              | Latest MC Version | Notes                   |
|-------------------------------------------------------------------------------------|--------------------------------------------|-------------------|-------------------------|
| [Additional Lights](https://www.curseforge.com/minecraft/mc-mods/additional-lights) | `mods\additional_lights-1.16.4-2.1.3.jar`  | 1.17.1            |                         |
| [Apple Skin](https://www.curseforge.com/minecraft/mc-mods/appleskin)                | `mods\AppleSkin-mc1.16.2-forge-1.0.14.jar` | 1.18              |                         |
| [Architectury](https://www.curseforge.com/minecraft/mc-mods/architectury-forge)     | `mods\architectury-1.19.27-forge.jar`      | 1.16.5            |                         |
| [Auto Reg Lib](https://www.curseforge.com/minecraft/mc-mods/autoreglib)             | `mods\AutoRegLib-1.6-47.jar`               | 1.16.5            | Dependency of Quark     |
| [Cloth Config](https://www.curseforge.com/minecraft/mc-mods/cloth-config-forge)     | `mods\cloth-config-4.11.26-forge.jar`      | 1.18.1            |                         |
| [Discord Integration](https://www.curseforge.com/minecraft/mc-mods/dcintegration)   | `mods\dcintegration-forge-2.1.1-1.16.jar`  | 1.12.2            |                         |
| [Light Overlay](https://www.curseforge.com/minecraft/mc-mods/light-overlay)         | `mods\light-overlay-5.8.1.jar`             | 1.18.1            |                         |
| [Quark](https://www.curseforge.com/minecraft/mc-mods/quark)                         | `mods\Quark-r2.4-311.jar`                  | 1.16.5            |                         |
| [QuarkOddities](https://www.curseforge.com/minecraft/mc-mods/quark-oddities)        | `mods\QuarkOddities-1.16.3.jar`            | 1.16.5            | NOTE: Addition to Quark |
| [Torchmaster](https://www.curseforge.com/minecraft/mc-mods/torchmaster)             | `mods\mods\torchmaster-2.3.7.jar`          | 1.12.2            |                         |
| [Waystones](https://www.curseforge.com/minecraft/mc-mods/waystones)                 | `mods\Waystones_1.16.5-7.5.1.jar`          | 1.18.1            |                         |
| [XP Tome](https://www.curseforge.com/minecraft/mc-mods/xp-tome)                     | `mods\xptome-1.16.5-v2.1.jar`              | 1.18              |                         |
