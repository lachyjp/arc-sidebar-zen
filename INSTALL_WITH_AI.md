# Install with an AI coding agent

Paste the prompt below into Claude Code, Codex or a similar agent that can run shell commands on your computer.

```text
Install the "Arc Sidebar" Zen Browser mod from https://github.com/lachyjp/arc-sidebar-zen for me.

1. Find my Zen profile folder:
   - macOS: ~/Library/Application Support/zen
   - Linux: ~/.zen, or ~/.var/app/app.zen_browser.zen/.zen for Flatpak
   - Windows: %APPDATA%\zen
   Read profiles.ini. Use the profile named in the [Install…] section's "Default=" line, which is the one Zen opens. If there are several, list them and ask me which one.
2. Download https://raw.githubusercontent.com/lachyjp/arc-sidebar-zen/main/chrome.css. Read it and confirm it is plain CSS, then show me a one-line summary.
3. Ask me before quitting Zen. Then quit it gracefully (on macOS: osascript -e 'tell application "Zen" to quit'), and wait until it has exited.
4. In <profile>/chrome/, create the folder if needed:
   - If userChrome.css already exists, back it up as userChrome.css.bak-<date>. Then append the mod between the markers "/* arc-sidebar-zen start */" and "/* arc-sidebar-zen end */". If those markers already exist, replace what's between them instead. Never delete my other CSS.
   - Otherwise, save the mod as userChrome.css.
5. In <profile>/user.js (back it up first if it exists; never remove existing lines), make sure each of these lines is present exactly once:
   user_pref("toolkit.legacyUserProfileCustomizations.stylesheets", true);
   user_pref("mod.arcsidebar.spacing", true);
   user_pref("mod.arcsidebar.tinted_text", true);
   user_pref("mod.arcsidebar.selected_tab", true);
   user_pref("mod.arcsidebar.essentials", true);
   user_pref("mod.arcsidebar.url_text", true);
6. Reopen Zen. Then tell me:
   - which files you changed
   - where the backups are
   - that I can switch any part off in about:config by setting its mod.arcsidebar.* setting to false and restarting
   - how to uninstall: remove the arc-sidebar-zen block from userChrome.css and restart Zen
```

The mod was built and tested on Zen 1.23 for macOS.
