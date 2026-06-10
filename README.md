# Waterfall

**A pay-yourself-first money cockpit for dual-income couples.** One HTML file, zero dependencies, fully private.

Most budgeting breaks down the same way: you try to save "whatever's left at the end of the month," and there's never anything left. Waterfall flips it. Your investments come out **first** and are locked. Your fixed bills come next. Whatever remains is your spending ceiling — and your card bill becomes the *only* number that varies. Overspend in a heavy month? It draws down a **Flex buffer** you built in good months — never your investments, never your emergency fund.

It's built for the situation a lot of young earning couples are in: no credit-card debt, decent income, but no real visibility into where ₹1.5–2L a month actually goes, and a vague sense of "we should be investing by now."

## What it does

- **This month** — enter your card bill and watch money cascade through locked tiers (investments → bills → spending → surplus). See instantly that a big-spend month doesn't touch your future.
- **Net worth** — assets minus liabilities, asset-class mix, and an emergency-fund-in-months read.
- **Goals** — each goal tagged near / medium / long-term, with the monthly contribution it needs and whether it should sit in safe or equity money.
- **Big buy** — compare a large purchase (e.g. a car) as **cash vs loan vs company lease**, including the liquidity and job-lock-in trade-offs.
- **Settings** — every number is yours to edit: income, bills, locked investments, surplus split, assets, goals.

## The core idea

```
Salary lands
   │
   ▼  1. Investments        ← LOCKED. Non-negotiable. Out first.
   ▼  2. Fixed bills        ← rent, utilities, insurance…
   ▼  3. Card spend         ← the ONLY variable
   ▼  4. Surplus            ← splits into Goals + a Flex buffer
            └─ Flex buffer absorbs the overspend months
```

## Use it

Just open `index.html` in any browser. That's it — no install, no build, no account.

### Publish your own copy (free, on GitHub Pages)

1. Fork this repo.
2. In your fork: **Settings → Pages → Source: `main` branch, `/root`**.
3. Open the URL it gives you. Done.

## Privacy

Everything you type is stored **only in your own browser** (`localStorage`). Nothing is uploaded, there's no server, and there's no account. Use **Export** in Settings to back up to a JSON file or move your data to another device. If your browser blocks local storage, the app still works for the session — just export before you close it.

## Customize it

The app ships with sample data for an illustrative couple. Open **Settings** and overwrite it with your own. The whole engine is config-driven, so it adapts to any income, any set of goals, any currency context — no code changes needed for normal use. If you want to fork and change the logic or design, it's a single readable `index.html` (vanilla JS, custom CSS, commented).

## Not advice

Waterfall is a planning tool, not financial, tax, or investment advice. The "Big buy" comparison and any tax-related figures are illustrative — confirm specifics with a qualified adviser before making decisions.

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, ship your own version.
