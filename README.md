# silent-portal-ambient

A lightweight Minecraft server resource pack that only mutes the ambient hum of Nether portals while keeping teleportation sounds intact.

## Overview

Nether portals constantly emit an ambient hum (`block.portal.ambient`) that can become overwhelming near bases, gold farms, or chunk loaders. This resource pack overrides only `block.portal.ambient` with an empty sound definition, freeing up sound channels and silencing the idle portal hum while preserving:

- **Portal Travel (`block.portal.travel`)**: Played when teleporting through a Nether portal.
- **Portal Trigger (`block.portal.trigger`)**: Played when stepping into a Nether portal and the screen animation starts.

## Server Setup (`server.properties`)

Add or update the following lines in your Minecraft server's `server.properties` file:

```properties
resource-pack=https\://github.com/loademon/silent-portal-ambient/releases/download/v1.0.0/silent-portal-ambient.zip
resource-pack-sha1=b69c3542a4aca91e92b684ca86890fb19cba5823
require-resource-pack=false
resource-pack-prompt={"text":"Optional resource pack that mutes the constant Nether portal ambient hum.","color":"gray"}
```

- **Direct Download URL:** `https://github.com/loademon/silent-portal-ambient/releases/download/v1.0.0/silent-portal-ambient.zip`
- **SHA-1 Hash:** `b69c3542a4aca91e92b684ca86890fb19cba5823`

## File Structure

```text
silent-portal-ambient.zip
├── pack.mcmeta
└── assets/
    └── minecraft/
        └── sounds.json
```
