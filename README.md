<img src="https://images.evetech.net/characters/210307238/portrait?size=128" align="right" width="112" height="112" alt="Beulea" />

# Beulea's EVE Industry — downloads & updates

**A desktop cost & profit calculator for EVE Online manufacturing — built by an industrialist, for industrialists.**

It computes what your builds *actually* cost and earn — T1, T2 invention, T3, and reactions — from **your own** blueprints, structures, and skills. Runs on your machine, works offline, and syncs your characters over ESI. This repository hosts the **downloads**, the **auto-update feed**, and **support** (Issues + Wiki); the source code lives in a separate repository.

**[⬇ Download the latest release](../../releases/latest)** · macOS (Apple Silicon) & Windows (x64)

---

## Why this exists

I'm **Beulea** — a solo high-sec industrialist in The Forge, hauling to Jita like everyone else. The web calculators are good, but two things always bit me:

- **Midpoint-price optimism.** Most tools quote the mid-price, not what the order book will actually fill. Margins look great — until you try to buy 400 units and the price walks away from you.
- **Silent staleness.** You rarely know how old the numbers are, and one MER-deflation month can quietly eat a build you already committed ISK to.

So I built the tool I wanted: **real order-book depth**, a **price-freshness clock you can actually see**, **offline-first** so it opens instantly, and **per-character ESI sync** so the skills, jobs, and wallet are *mine* — not a guess. The classic desktop tool (EVE IPH) is winding down; this is my attempt to carry that torch for the solo builder.

## What it does

- **Accurate economics** — full job-fee model (EIV, system cost index, structure bonuses, taxes) kept current with CCP's rules.
- **Build vs. buy** per material, with ME/TE, structure & rig bonuses, security effects.
- **Invention** — T2 probability, decryptor comparison, per-run profit; T3 relic invention.
- **Sourcing & refining** — ore/ice reprocessing deals, one-stop-shop by station, LP ore-basket optimizer.
- **Profitability scanner** — rank products by margin / ISK-hr / profit-day, with market velocity.
- **Multi-character** — roster, per-character skills, "who's free", wallet realized-P&L ledger, net-worth chart.
- **One-click Multibuy** export on every shopping list (in-game `name⇥qty`).

## Download

Get the latest build from the [**Releases**](../../releases/latest) page:

- **macOS** (Apple Silicon): `.dmg`
- **Windows** (x64): `…-setup.exe` (NSIS installer)

Once installed, the app checks here for updates and installs them in place — a one-click "Update & restart".

## First launch

Builds are unsigned (no paid Apple/Windows certificate yet), so the OS shows a one-time warning. This is expected for fan tools and it's safe to proceed:

- **macOS** — Gatekeeper: right-click the app → **Open** → **Open**; or run
  ```sh
  xattr -dr com.apple.quarantine "/Applications/Beuleas Eve Industry.app"
  ```
- **Windows** — SmartScreen ("Windows protected your PC"): click **More info** → **Run anyway**.

After that it launches normally and updates itself automatically.

## Found it useful? Send ISK — o7

This is **free** and always will be. If it saved you some ISK and you feel like giving back, in-game donations to **Beulea** are very welcome (and fund more datacores for testing 😄). **ISK only — no real money.**

→ In-game: search **Beulea** in *People & Places*, or right-click the name → **Give Money**.
→ Character info: [Beulea on EVE Who](https://evewho.com/character/210307238)

## Feedback

- 🐞 Bugs / feature requests → [**Issues**](../../issues). Include what you were building, your structure/skills if relevant, and what you expected vs. what you saw.
- 📖 Docs / FAQ → [**Wiki**](../../wiki)

## Legal & data

- **EVE Online** and all related logos and trademarks are the intellectual property of **CCP hf.** This is an **unofficial** fan tool and is **not affiliated with, sponsored, or endorsed by CCP hf.** It is distributed **free of charge and non-commercially**, in line with CCP's fan-tool / IP policy.
- Static data (the SDE) courtesy of **[Fuzzwork](https://www.fuzzwork.co.uk/)** (Steve Ronuken). Live market data from **Fuzzwork aggregates** and the **EVE Swagger Interface (ESI)**; industry-cost math is validated against **[EVE Ref](https://everef.net/)**. Huge thanks to all three — they keep New Eden's tooling alive.
- All other trademarks are the property of their respective owners.

*Fly safe. o7*
