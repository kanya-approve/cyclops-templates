# Cyclops Template Repository

![Cyclops Logo](cyclops-simplistic.png "Cyclops Logo")

## Overview 📜

### /mekanism-minecraft-server

- creates a Mekanism tech/electricity Minecraft Server using [docker-minecraft-server](https://github.com/itzg/docker-minecraft-server), [Youer](https://mohistmc.com/) (Forge/NeoForge + Bukkit hybrid), and the [Mekanism](https://modrinth.com/mod/mekanism) mod suite

### /pixelmon-minecraft-server

- creates a Pixelmon Minecraft Server using [docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) and [Youer](https://mohistmc.com/)

### /vanilla-minecraft-server

- creates a Vanilla Minecraft Server with the latest version supported by given plugins using [docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) and [Purpur](https://github.com/PurpurMC/Purpur)

## Configuration ⚙️

Each server's options are defined in its `values.schema.json` and rendered as form fields in Cyclops. Notably, `accessType` selects how the server is exposed: a `cloudflare-tunnel` ingress at `<name>-mc.<domain>` (set `domain`), a `LoadBalancer`, or a `NodePort`.
