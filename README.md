# RTNW Headwear Codex

A single-page crafting tracker for the RTNW headwear list — 44 items across 6 towns
(Prontera, Morroc, Alberta, Payon, Geffen, Izlude), each showing the blueprint needed
(if any), the doll requirement, the element core, and the coin cost.

Everything lives in `index.html` — no build step, no dependencies to install.

## Publish it on GitHub Pages

1. Create a new GitHub repo (or use an existing one) and add `index.html` to the root.
2. Push it to GitHub.
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Pick your default branch (e.g. `main`) and `/ (root)` as the folder, then **Save**.
6. GitHub will give you a URL like `https://yourusername.github.io/your-repo/` within a
   minute or two — that's your live tracker.

## Using it

- Click a town tab to filter to that map, or stay on **All Towns** to see everything
  grouped by map.
- Use the search box to find a headwear item or the doll it needs.
- Toggle **Blueprint only** to see just the items that require a blueprint.
- Click the checkbox on any card to mark it crafted — progress is saved in your
  browser (`localStorage`), so it's there next time you open the page. It's local to
  each browser/device, not synced anywhere.
- "reset all progress" at the bottom clears every checkmark.

## Editing the data

All the data is a single JS array (`DATA`) near the top of the `<script>` tag in
`index.html` — each item has `map`, `headwear`, `blueprint`, `dollQty`, `dollName`,
`coreQty`, `coreName`, and `coin`. Edit that array directly to add, remove, or fix
entries; no rebuild needed, just save and refresh.

## Tracking what you own (new)

Click **My Stockpile** in the toolbar to open the input panel. Enter:
- how much **Adv. Coin** you're holding
- how many of each **element core** you have
- how many of each **doll** you have

Every card below updates instantly to show `have / need` for its doll, core, and coin
requirements — green when you have enough, red with "need X more" when you're short.
Cards that are fully covered get a **"✓ Ready to craft"** pill, and you can flip on
**Craftable now** in the toolbar to show only those. Everything you enter is saved in
your browser (`localStorage`) alongside your crafted checkmarks, so it's still there
next time you open the page.

Two pairs of doll names in the original sheet are spelled two different ways
(Bahoment Jr. / Baphoment Jr., and Familiar / Familliar) — the tracker treats each
pair as the same doll so you only enter a count once.
