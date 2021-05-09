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

**NOTE**: By providing EULA=TRUE you agree to the EULA at https://account.mojang.com/documents/minecraft_eula.

## Environment Variables
- EULA (Required)
  - Default: none

## Docs / Guides

See [client-setup-guide.md](docs/client-setup-guide.md) to setup your minecraft client.