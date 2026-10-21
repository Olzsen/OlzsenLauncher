# Hearth Launcher prototype

A desktop UI prototype for a Minecraft launcher, built with a small vanilla JavaScript frontend and a Tauri 2 shell.

## Run it

Install the Tauri prerequisites for your operating system, then run:

```sh
npm install
npm run dev
```

To create a desktop bundle, run `npm run build`.

The same interface can be previewed by opening `frontend/index.html` in a browser.

## Prototype flows

- Switch between the dashboard, instance library, mod catalog, download queue, and settings.
- Create, filter, inspect, and remove local demo instances.
- Find sample mods from Modrinth and CurseForge, choose an instance, and simulate installation.
- Adjust memory, Java selection, launch preferences, and download concurrency. Settings persist in local storage.
- Search the app with `Ctrl+K` / `⌘K` and simulate launch preparation.

## Not connected yet

Mod entries and download progress are sample data. No Minecraft files are downloaded or launched. Microsoft sign-in, Mojang version manifests, Fabric/Forge/NeoForge/Quilt/OptiFine installers, CurseForge and Modrinth APIs, Java discovery, and the native game process still need implementation. The Tauri shell currently supplies the desktop window; the launcher operations will need Rust commands and secure credential storage.

