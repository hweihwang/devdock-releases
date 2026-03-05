# DevDock Releases

**DevDock** is a local development dashboard for macOS that helps you run multi-repo stacks like an operations control plane.

If you manage several services locally (web, API, workers, queues, scripts), DevDock gives you one place to start/stop everything, detect process leaks, resolve port conflicts, and inspect runtime logs.

This repository is the **public distribution channel** for DevDock binaries.
The app source code lives in a separate private repository during the current product phase.

## Download DevDock

- Latest release (DMG, ZIP, AppImage): [github.com/hweihwang/devdock-releases/releases/latest](https://github.com/hweihwang/devdock-releases/releases/latest)
- DevDock landing page: [hweihwang.com/devdock](https://hweihwang.com/devdock/)

### Install on macOS with Homebrew

```bash
brew install --cask hweihwang/devdock/devdock
```

## What DevDock Solves

DevDock is built for developers and teams dealing with:

- too many terminal tabs to run local services
- recurring local environment drift across projects
- orphan processes draining CPU/RAM after crashes
- repeated port conflicts when switching branches or repos
- slow debugging because service status and logs are spread out

## Core Features

- **Service orchestration:** run and stop grouped services across repositories
- **Workspace sessions:** save and restore local service sessions
- **Process monitoring:** detect suspicious/orphan background processes
- **Port conflict detection:** surface collisions before they derail startup
- **Runtime visibility:** inspect live state and stream recent logs in one UI
- **Local-first architecture:** runtime and app state stay on your machine

## Local-First Data Model

DevDock stores state under `~/.devdock/` (for example: config, sessions, runtime snapshots).

No mandatory cloud backend is required for local operations.

## Release Assets

Each version may include:

- `DevDock-mac-arm64.dmg`
- `DevDock-mac-x64.dmg`
- `DevDock-mac-arm64.zip`
- `DevDock-mac-x64.zip`
- `DevDock-linux-arm64.AppImage`
- `DevDock-linux-x86_64.AppImage`
- `latest-mac.yml` and `latest-linux*.yml` (update manifests)

## Auto Update Notes

macOS auto-updater flows rely on the ZIP artifacts and update manifests.
DMGs are provided as the primary human download format.

## Support and Feedback

- Email: [hoangmaths96@gmail.com](mailto:hoangmaths96@gmail.com)
- Discord: [discord.gg/VF5y89RqxP](https://discord.gg/VF5y89RqxP)

If you run complex local stacks and want DevDock to fit your workflow better, send your setup details and pain points.
