# Changelog

## 1.1.0 - 2026-09-25

A big round of fixes, most of them to prices.

**Prices**
- No more "Vendor it" when only one or two sellers list an item. You get a price instead, marked low confidence; if that comes out under 10ex, it says to list at ~10ex and expect a wait.
- A strong item whose closest listings are worse items (missing its best mods) is no longer told to vendor.
- Corrupted items copied with advanced descriptions (Ctrl+Alt+C) are now priced as corrupted.
- White and magic crafting bases are priced only off their own base, and waystones only off their own tier.
- Rings count their own resistance when finding comparable rings, belts are compared on their charm slots, and relics on relic stats.
- Prices shown in Divine no longer round up or down by as much as a third.
- Unidentified items say "Identify it first" instead of "Vendor it".
- When part of a search fails on the trade site's side, Loot Sense says so instead of pricing off half the market.

**Trade limits**
- Searches you make in your browser are tracked better, so Loot Sense no longer runs into the trade site's limit after a pause.
- Starting Loot Sense a second time brings up the one that's already open instead of running two copies.

**Your shop**
- Each listing's advice now comes from a check of that exact item (same item level and rolls), not from another copy with the same name.
- The panel shows when the next automatic re-check is.
- Changing league in Settings now switches the shop, the re-pricing and remembered checks too.
- Shops with over 100 listings no longer use up the trade limit.
- After this update, your listings are re-priced in the background once.

**Everything else**
- Loot Sense no longer gets stuck on "Checking…" after an error.
- An item copied while another is being checked is checked right after it.
- The loot filter is found and written in the right place when Documents is in OneDrive.
- The filter keeps updating with your own exchange rates turned on, and the panel says why when it can't update.
- Settings are saved safely; a damaged settings file no longer stops the app or resets everything.
- The Update button only ever opens this page.

## 1.0.0 - 2026-09-23

The first release.

- **Price check on Ctrl+C:** a small overlay shows the price in game (quick
  sale, the price to list at, and a patient price) or says to vendor it,
  with how sure it is.
- **Your shop:** checks your trade listings and tells you what to vendor,
  lower, raise or re-check.
- **Loot filter:** NeverSink's strict filter with live prices on top, rebuilt
  every 30 minutes.
- **Currency** priced at the in-game exchange rate.
- Stays inside the trade site's rate limits; reads only, never lists or buys.
