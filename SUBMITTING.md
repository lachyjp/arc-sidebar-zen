# Submitting Arc Sidebar to the Zen Mods store

Zen mods are submitted through an issue form on the `zen-browser/theme-store` GitHub repository. A bot then opens the pull request for you.

## 1. Put the mod on GitHub

The form asks for a homepage, and the image has to be reachable by URL. Done: https://github.com/lachyjp/arc-sidebar-zen holds:

- `chrome.css`
- `preferences.json`
- `README.md`
- `image.png` (600×400, as the store requires)

## 2. Fill in the form

Open https://github.com/zen-browser/theme-store/issues/new/choose and choose the create-theme form.

| Field | What to enter |
|---|---|
| Name | `Arc Sidebar` (must be under 25 characters) |
| Description | `Matches Zen's sidebar to Arc: row height, type, space-tinted text, selected tab and Essentials.` (95 characters; the limit is 100) |
| Homepage | `https://github.com/lachyjp/arc-sidebar-zen` |
| Image | `https://raw.githubusercontent.com/lachyjp/arc-sidebar-zen/main/image.png` |
| Styles | All of `chrome.css` |
| README | All of `README.md` |
| Preferences | All of `preferences.json` |

## 3. Updating later

Open a new issue on the same repository and describe the changes.

## Sharing before it's approved

Your friend can use it straight away without the store:

1. In Zen, open `about:config` and set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`.
2. Open `about:support` and click **Open Folder** next to **Profile Folder**. Inside it, make a folder called `chrome` and copy `chrome.css` into it as `userChrome.css`.
3. In `about:config`, add these five settings as **Boolean** and set each to `true`:
   `mod.arcsidebar.spacing`, `mod.arcsidebar.tinted_text`, `mod.arcsidebar.selected_tab`, `mod.arcsidebar.essentials`, `mod.arcsidebar.url_text`
4. Restart Zen.
