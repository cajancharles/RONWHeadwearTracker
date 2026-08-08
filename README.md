# Ragnarok: The New World - Headwear Tracker

A single-page crafting tracker for the RONW headwear list — 44 items across six towns
(Prontera, Morroc, Alberta, Payon, Geffen, Izlude). For every headwear item it shows
the town it's found in, the blueprint it needs (if any), the doll requirement, the
element core, and the coin cost to craft it.

Everything lives in one self-contained `index.html` file — no build step, no
dependencies, nothing to install. Open it in a browser and it works.

## Features

**Browse by town.** Tabs across the top filter to a single town, or stay on
**All Towns** to see everything grouped by map, each with its own crafted count.

**Search.** Find a headwear item or the doll it needs by typing in the search box.

**Blueprint filter.** Toggle **Blueprint only** to see just the items that need a
blueprint to craft.

**My Stockpile — track what you own.** Open the **My Stockpile** panel to enter how
much Adv. Coin, and how many of each element core and doll, you're currently holding.
Every card updates automatically to show `have / need` for its doll, core, and coin
requirements — green when you have enough, red with "need X more" when you're short.
Items you can fully craft right now get a **"✓ Ready to craft"** pill, and the
**Craftable now** toggle filters the list down to just those.

Two pairs of doll names in the source sheet were spelled two different ways
(Bahoment Jr. / Baphoment Jr., and Familiar / Familliar) — the tracker treats each
pair as one doll so you only enter a count once.

**Crafted checklist.** Click the checkbox on any card to mark it crafted. The header
progress bar and each town's tab count update to match.

**Saved automatically.** Your stockpile counts and crafted checkmarks are saved in
your browser (`localStorage`) as you go, so they're still there next time you open
the page. This is local to the browser/device you're using — it isn't synced
anywhere. Use **reset crafted progress** or **reset stockpile** in the footer to
clear either one.


---

## Tech

Just plain HTML, CSS, and vanilla JavaScript. No frameworks, no build tools, no npm install. Open the file and it works.

---

## Credits

Built by [@CharlesPlaysGG](https://www.youtube.com/@CharlesPlaysGG)

- YouTube: https://www.youtube.com/@CharlesPlaysGG
- TikTok: http://tiktok.com/@charlesplaysgg
- Twitch: _(coming soon)_

## Support

If this tool saves your guild some headaches, consider supporting the project — every bit helps keep it maintained and free for everyone.

**Crypto:**

| Currency | Address |
|---|---|
| BTC | `15zZzbk9t4Gf9xsaNJ7FqoomKmgjJyKWvE` |
| BNB (BEP20) | `0xceacfec618768e01a1dd68fe407f69f1b87162b3` |
| USDT (TRON) | `TYmZd9LntLQXs2GhK9D49Y5AehUPLadJme` |
| Solana | `o6TZyGN23P9ju2i9EuENT7XNdM5na2pmMtUq4w5ukco` |

**GCash:**

<p align="center">
  <img src="gcash-qr.jpg" alt="GCash QR code for donations" width="250">
</p>

## Disclaimer

Not affiliated with Gravity Co., Ltd. or Ragnarok: The New World. This is an unofficial, fan-made tool.

## License

MIT — free to use, modify, and share.

