# Blueprint Beacon Plugin

Plugin to expose Unreal Online Beacon functionality to Blueprints.

## Overview

- Runtime module: `BlueprintBeacon`
- Primary goal: Blueprint-accessible beacon host/client flow built on OnlineSubsystemUtils

## Requirements

- Unreal Engine project that can build plugins
- `OnlineSubsystemUtils` plugin enabled
- `BlueprintBeaconClient` plugin enabled
- OnlineSubsystem configuration in your project config if your beacon workflow requires it

## Setup

1. Copy this repository folder into your project at `Plugins/BlueprintBeacon`.
2. Ensure `BlueprintBeacon.uplugin` lives at `Plugins/BlueprintBeacon/BlueprintBeacon.uplugin`.
3. Enable `BlueprintBeacon`, `OnlineSubsystemUtils`, and `BlueprintBeaconClient` in your project (Editor: Plugins menu, or your `.uproject`).

## Development commands

- Build: Build your Unreal project normally; the plugin compiles as part of the project build.
- Test: No automated tests are included in this repository.
- Lint: No lint tooling is configured for this plugin.

## Release / deployment

- No automated release pipeline is provided. Distribute the plugin by shipping the `Plugins/BlueprintBeacon` folder or tagging a source release.

## Repository layout

- `Source/BlueprintBeacon`: C++ module source
- `Resources`: Plugin resources (icons, metadata)
