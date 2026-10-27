# Installing and submitting Arc Sidebar

## Install it yourself

1. In Zen, open `about:config` and set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`.
2. Open `about:support` and click **Open Folder** next to **Profile Folder**. Inside it, make a folder called `chrome` and copy [`chrome.css`](chrome.css) into it as `userChrome.css`.
3. In `about:config`, add these five settings as **Boolean** and set each to `true` (set any to `false` to switch that part off):
   - `mod.arcsidebar.spacing`
   - `mod.arcsidebar.tinted_text`
   - `mod.arcsidebar.selected_tab`
   - `mod.arcsidebar.essentials`
   - `mod.arcsidebar.url_text`
4. Restart Zen.

## Zen Mods store

The store's submission repository, [`zen-browser/theme-store`](https://github.com/zen-browser/theme-store), was archived in July 2026. Its issue form no longer accepts new mods, and Zen hasn't published a replacement as of October 2026. This repository is ready to submit once one exists:

| Store field | Value |
|---|---|
| Name | `Arc Sidebar` |
| Description | `Matches Zen's sidebar to Arc: row height, type, space-tinted text, selected tab and Essentials.` |
| Homepage | `https://github.com/lachyjp/arc-sidebar-zen` |
| Image | `https://raw.githubusercontent.com/lachyjp/arc-sidebar-zen/main/image.png` (600×400) |
| Styles | [`chrome.css`](chrome.css) |
| README | [`README.md`](README.md) |
| Preferences | [`preferences.json`](preferences.json) |
