<p align="center">
  <img src="docs/logo.png" width="96" alt="Loot Sense logo">
</p>

<h1 align="center">Loot Sense</h1>

<p align="center">
  A price checker for <b>Path of Exile 2</b>: copy an item, see what it's worth.<br>
  <a href="../../releases/latest"><b>Download the latest version</b></a>
</p>

<p align="center">
  <img src="docs/main-window.png" width="840" alt="The Loot Sense window">
</p>

## What it does

- **Prices items on Ctrl+C.** A small overlay shows what an item is worth right
  in game: a quick-sale price, the price to list at, and a patient price, with
  how sure it is. Junk just says **Vendor it**.
- **Watches your shop.** It checks your trade listings and tells you what to
  vendor, lower, raise or re-check.
- **Keeps your loot filter up to date.** NeverSink's strict filter with live
  prices on top, rebuilt every 30 minutes.
- **Knows currency.** Orbs, runes, essences and the like are priced at the
  in-game exchange rate.

<p align="center">
  <img src="docs/overlay.png" width="840" alt="The overlay: a rare ring, a magic jewel, and an item to vendor">
</p>

## Install

1. Download the zip from **[Releases](../../releases/latest)**.
2. Unzip the **Loot Sense** folder anywhere and keep its files together.
3. Double-click **LootSense.exe**.

The first time, Windows may say *"Windows protected your PC"*. Click
**More info → Run anyway**.

Closing the window keeps Loot Sense running in the tray (next to the clock).
Right-click the tray icon and choose **Exit** to quit.

Loot Sense tells you when a new version is out.

## Using it

| In game | What happens |
|---|---|
| Hover an item, press **Ctrl+C** | The overlay prices it (it never takes focus from the game) |
| Keep pressing Ctrl+C through your stash | Each new item replaces the last one |
| **Ctrl+Shift+L** | Brings the overlay back after it fades |
| Drag the overlay | Moves it; it remembers where you put it |
| Double-click the overlay | Opens the main window |

**Your shop:** press Ctrl+C once on one of your own listed items (one with a
price note). Loot Sense then finds your listings by itself and checks them
regularly.

**Loot filter:** pick **LootSense-NeverSink** in the game's options. The file
lives in `Documents\My Games\Path of Exile 2`.

## FAQ

**Is it safe to use?**
Loot Sense only reads your clipboard and the public trade site, the same way
your browser does. It never touches the game's files or memory, never logs in
to your account, and never lists, buys or sells anything. It stays inside the
trade site's request limits.

**Why do some prices say "low confidence"?**
The market for that item is thin or all over the place. Treat the number as a
range and have a look on the trade site before selling cheap.

**It says I hit the trade limit.**
The trade site allows only a few searches a minute. Checking lots of items
quickly fills that up; Loot Sense waits it out and carries on.

**Does it work with Path of Exile 1?**
No, Path of Exile 2 only.

**Where are my settings? How do I uninstall?**
Everything Loot Sense remembers is in `C:\Users\<you>\.loot_sense`. If you
turn on the daily backup in Settings, the last 7 copies are also kept in
`OneDrive\LootSense backups` (or `Documents\LootSense backups`). To uninstall,
delete the Loot Sense folder, that folder, and the backups if you made any.

**What does it connect to?**
Only the Path of Exile website (the trade site), poe.ninja and poe2scout (for
prices), and this page to see if there's a new version.
No tracking, no ads, no accounts. It only looks at copied text that is a Path
of Exile item; anything else you copy is ignored.

**How do I know my download is the real one?**
Download only from this page. Each release lists a SHA-256 checksum: in
PowerShell, `Get-FileHash LootSense-1.0.0.zip` should print the same one.

## License

Free to use. Please don't re-upload, sell or rebrand it. Share the link to this
page instead. See [LICENSE.txt](LICENSE.txt).

Not affiliated with or endorsed by Grinding Gear Games.
