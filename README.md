# Seek for Jellyfin

A Jellyfin plugin for the [Seek](https://seek.nerdspar.com) app. It keeps an exact log of what each
person plays, finishes, ticks and un-ticks, so Seek's watch history matches Jellyfin without a webhook.

- A play counts only when Jellyfin says it was played to completion; stopping partway (or a partial
  rewatch) never adds a play.
- Ticking played / un-ticking in Jellyfin comes through to Seek too.
- Each person reads only their own log, signed in as themselves.
- Stored in the plugin's own folder, not Jellyfin's database.

Requires **Jellyfin 12.0 or later**.

## Install

1. Jellyfin → Dashboard → Plugins → **Repositories** → add:
   `https://raw.githubusercontent.com/nerdspar/jellyfin-plugin-seek/main/manifest.json`
2. Catalog → **Seek** → Install, then restart Jellyfin.
3. In the Seek app: Settings → Jellyfin → sign in. It shows "Seek plugin: Installed".

This repository holds the plugin's releases and repository manifest.
