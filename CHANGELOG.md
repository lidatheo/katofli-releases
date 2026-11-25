# Changelog

All notable changes to Katofli. The format follows Keep a Changelog (https://keepachangelog.com/en/1.1.0/) and versions follow Semantic Versioning (https://semver.org/).

## [Unreleased]

Nothing yet. Every PR with a user-visible change adds its line here, under its type and area (docs/release.md).

## [0.9.0] - 2026-11-25

The first public release.

### Added

#### Bar and task strip

- A bar that replaces the system taskbar, one per display, on any edge (top, bottom, left or right), with a DPI-aware height you choose, an optional gap and rounded corners.
- Extra bars on any display, each with its own modules, task strip, colours and placement.
- Layout presets and saved layouts you switch in one click.
- Task strip: pinned and running apps, grouping by app, app-name labels, drag to pin and reorder, drop files on a tile to open them, middle-click to close, window peek and group flyouts with live thumbnails.
- Per-app rules: hide, rename, re-icon and group apps on the task strip, and open an app on a chosen display or desktop.
- Pins follow the system's own pin-to-taskbar, and existing pins can be imported.
- Auto-hide with show and hide delays, reveal on attention and an overlap mode; an always-visible bar steps aside for a full-screen app.
- Bar transparency: solid, see-through or floating icons.
- Drag-and-drop editing of the modules on a bar, with left, centre or right alignment per zone.

#### Launcher

- A launcher with fuzzy search, recent and pinned apps, several looks (menu, full-screen grid, search-first) and an always-visible Settings button.
- Custom web searches with a template gallery, opening in a chosen browser or browser profile.
- The launcher button can also open the system Start menu, another launcher you have installed, or a program you choose.

#### Game bar

- A game library from Steam, Epic Games Launcher, GOG, Ubisoft Connect, Heroic, Xbox and Store games and your own folders, with cover art, recent games, play time and companion tools.
- Library, shelf and search layouts.

#### Modules and widgets

- Clock and calendar, weather with several locations, media controls for every player, volume with a per-app mixer, network with VPN and sign-in notices, Bluetooth, battery, resource meters, notifications, clipboard history, keyboard layout, keep awake, a privacy indicator, show desktop, a power menu, window title, virtual desktops, command buttons and quick settings (including a mobile hotspot with a QR code).
- Other looks for many modules, and several copies of one module on different bars, each with its own settings.
- A status icon area you can sort, hide and tint.
- Desktop widgets on the wallpaper, under the desktop icons.
- A themed Alt+Tab task switcher with live previews.
- A wallpaper manager with collections, rotation and per-display images.
- Plugins: small scripts in a sandbox, each enabled on its own after a confirmation.

#### Pop-ups

- Every pop-up has S, M, L and XL sizes and fits on the screen.
- Themed on-screen flyouts for volume and brightness.
- Themed tooltips on every bar chip and in every pop-up.

#### Themes and customisation

- Seven themes (Bento, Glasswork, Neo-Brutalist, Tonal, Mono Terminal, CRT Vaporwave, Risograph) with variants, a theme gallery and cross-fades between them.
- Theme options per theme and an advanced colour editor.
- Follows the system accent colour, light or dark mode and high-contrast mode, with a high-contrast variant in every theme.
- Motion speed, minimal borders and a module gallery.

#### Settings

- A Settings window with a grouped sidebar, a page for every module and every bar, and a search that finds any setting by its name or hint.
- An Apps group: pinned apps in order, an installed apps list to pin from, and per-app rules.
- An About page with the licence, the privacy note and the third-party notices. The licensor is Dimitra Lida Theodorou and the licence is governed by the laws of Greece.
- A What's new tab on the About page that lists the changes in the version you run, which the Updates page links to after an update.
- Help on every Settings page: the `?` button beside the title, or F1, opens that page's help beside it, with each setting's default, choices and config key.

#### Keyboard and shortcuts

- Keyboard navigation inside the bar, with a focus ring.
- Win+number shortcuts on Katofli's tiles, an optional launcher key, and a Shortcuts page with conflict detection.
- Emergency keys: one reloads every Katofli window, one quits and brings the system taskbar back.

#### Languages

- Katofli in 14 languages: English, Greek, German, French, Spanish, Italian, Brazilian Portuguese, Polish, Turkish, Russian, Ukrainian, Simplified Chinese, Japanese and Korean. All but English are machine-assisted.
- Native dialogs, pickers and menus follow the chosen language.

#### Reliability and safety

- The system taskbar always comes back: on exit, after a crash (a watchdog process), with `katofli.exe --restore-shell`, and on the next start.
- Recovery from WebView2 crashes, a safe start after a failed start, and a message when the WebView2 Runtime is missing.
- After an Explorer restart Katofli hides the system taskbar again.
- Windows run only Katofli's own code: a content security policy, a navigation guard, and files, folders and links open only after a check.
- Katofli keeps a capped log file in its logs folder for bug reports; paths inside your user folder are shown as `%USERPROFILE%`.

#### Performance and privacy

- Performance mode: Full, Reduced and Minimal levels by power state, with an optional pause while a full-screen app runs.
- One shared pop-up window and pop-ups created only when first opened, to keep memory down.
- Streaming mode hides notification text, media titles, clipboard previews and network names.
- No telemetry: nothing is sent to the developer.

#### Install and update

- A per-user installer that closes Katofli and restores the taskbar before installing or uninstalling, and refuses to run as administrator.
- A portable zip that keeps its data next to the program.
- An update check with an Updates page in Settings; a failed or cancelled update brings the old version back. Release copies check for a new version once a day; installed copies install only updates signed with the release key, when you choose to.
- Settings from builds before the rename to Katofli are copied over on first start.
- Katofli has its own icon, the Slit mark, on the program, the setup, the Start menu, Installed apps and the Settings window, drawn separately for each small size so it stays sharp.
