# Changelog

All notable changes to this site are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html).

## Versioning Rules

- **MAJOR** (X.0.0): incompatible changes, such as a new browser storage data format.
- **MINOR** (0.X.0): backward-compatible new features.
- **PATCH** (0.0.X): backward-compatible bug fixes.

## [2.10.0] - 2026-11-27 ([d1e4b20](https://github.com/Maxxxxior/poe-strat-calculator/commit/d1e4b20deee947ee6b854207c7f4cac20b728707))

### Added
- "Changelog" tab with the list of changes, site version, and latest commit date from GitHub.
- `CHANGELOG.md` file and Semantic Versioning 2.0.0 versioning.
- Toggle in the item search bar: after pasting a description, scroll to the closest listed item, closest sold item, closest match, or not at all.

### Fixed
- "In this session" shows the session selected in the list rather than the latest one. Session comparisons are also calculated relative to the selected session and the one before it.

## [2.9.1] - 2026-11-25 ([fb70bf4](https://github.com/Maxxxxior/poe-strat-calculator/commit/fb70bf47ec95c363e84e45abcb9ee7b6f0b04049))

### Fixed
- Holding Alt in item tooltips worked only once because releasing Alt caused the browser to capture focus. Alt state is now synchronized with mouse movement as well.

## [2.9.0] - 2026-11-25 ([449942d](https://github.com/Maxxxxior/poe-strat-calculator/commit/449942da3ea71baa74f4414fc3ff3b25af6df4d3))

### Added
- Support for items without a Rarity line (such as Viscera) and item editing (name, base, rarity, class, price, stats, icon).
- Shared icon library: uniques matched by name, other items matched by base, class, and attributes.
- Alt+click pins an item tooltip (dragging, closing, and ALT toggle).
- Gems and links assigned to an item, with colors and link connectors.
- Build publishing (nickname, name, class, ascendancy, bloodline, PoB link), friends' builds list, and preview mode.
- Pin button for the total build cost bar.

### Changed
- Inventory layout mirrors the original game, and item tooltips match in-game styling (without Alt: readable stats; with Alt: advanced stats).
- Slot icon no longer disappears after pasting a new item.

## [2.8.0] - 2026-11-24 ([0b57759](https://github.com/Maxxxxior/poe-strat-calculator/commit/0b57759467cbf7dfdd456981b14b10912e0ba227))

### Added
- "Build · valuation" tab: pasting items (Ctrl+V) with name and price, inventory-like slots, icons from screenshots, stat tooltip, total build cost, cost breakdown list, and pie chart.

## [2.7.0] - 2026-11-23 ([341392a](https://github.com/Maxxxxior/poe-strat-calculator/commit/341392a2ac6d70c1b00101be35f779ddf703eebe))

### Added
- New strategy types: Chance (random map), Gambling, and Invitation (boss bundle with importing runs from another strategy).
- Changing an existing strategy's type with confirmation and impact description.
- Price history for listed items ("was: 23c"), date added, and listed/sold filter.
- Step-by-step tutorial (with typing animation) and shorthand such as "4d" for 4 div.
- English language support (PL · EN switcher) and capitalized strategy names.

## [2.6.0] - 2026-11-22 ([848fc6c](https://github.com/Maxxxxior/poe-strat-calculator/commit/848fc6ca508112cea24d6646c45ea5da9a5e9e4f))

### Added
- Stash tab: chaos orbs, divines, other currencies, and items with individual exchange rates, pasting in-game descriptions, and a summary with shares.
- Arithmetic operations (+, -, *, /) and parentheses in quantities and amounts.

### Fixed
- Button collision ("add entered amount") between the stash and investments tabs.

## [2.5.0] - 2026-11-21 ([8e17910](https://github.com/Maxxxxior/poe-strat-calculator/commit/8e17910a6c8a8b44900273d044563d58685750f8))

### Added
- Search result colors (green: listed, blue: sold) and a "✓ Sold" button that toggles status without scrolling.

## [2.4.0] - 2026-11-21 ([33df4e5](https://github.com/Maxxxxior/poe-strat-calculator/commit/33df4e535621233f0b073652eea162eeedfdb079))

### Added
- Floating "↑ Back to search" button after jumping to an item.

## [2.3.0] - 2026-11-21 ([51aa7c6](https://github.com/Maxxxxior/poe-strat-calculator/commit/51aa7c62e7bb6dba7cfec54371c46706cd0ef7c5))

### Added
- Pasting an in-game item description (Ctrl+V) into an item's name or price field fills the row.

### Changed
- Search matches name and price together and compares names more strictly.

### Fixed
- "Doled Quicksilver Flask" matched every other flask.

## [2.2.0] - 2026-11-21 ([7f7ea7e](https://github.com/Maxxxxior/poe-strat-calculator/commit/7f7ea7e702f1a98c93f19cddc8ff5de7d71ab439))

### Added
- Dimmed sold items and item counts next to "Waiting to sale" and "Sold for".
- Average profit per sold item and per investment, plus a summary for each investment.
- Custom count for added items and runs.
- Buy orders (frozen funds) with conversion into an investment.
- Item search by name, price, and pasted in-game description.

## [2.1.0] - 2026-11-21 ([d520e80](https://github.com/Maxxxxior/poe-strat-calculator/commit/d520e8007ed0c466768dbcb4080fbaf770f9f8b3))

### Added
- Splitting existing runs into sessions (✂) and moving runs between sessions.
- Separate chaos/div exchange rate per session.
- Farming time per session and total strategy farming time.

## [2.0.0] - 2026-11-21 ([39b0878](https://github.com/Maxxxxior/poe-strat-calculator/commit/39b087818d4dfc18795db04df3c15f5cf4573d9b))

### Added
- Amount fields supporting expressions ("12c+3 div", "2+4c+5", "4+2+6div"): formatted display on blur, original expression restored on focus.
- Sessions, statistics range selector (all runs / last 10 / this session / per session), and session comparisons.
- "Investment" strategy type: items, prices, statuses, realized and potential profit, ROI.

### Changed
- Updated storage data format (v3) with automatic migration of older data.

## [1.4.0] - 2026-11-21 ([43978ad](https://github.com/Maxxxxior/poe-strat-calculator/commit/43978ad83da813aba4fbfdb80fb3d9095edd38bd))

### Added
- Single-run return chance, run-series return chance, and minimum run count (99% confidence) for each strategy.

## [1.3.0] - 2026-11-20 ([2e7723a](https://github.com/Maxxxxior/poe-strat-calculator/commit/2e7723a29e2798cb5fe1632f4da01c4fa6cf595a))

### Added
- Top statistics stay pinned on screen while scrolling down to the "Strategy comparison" section.

## [1.2.0] - 2026-11-20 ([8222b46](https://github.com/Maxxxxior/poe-strat-calculator/commit/8222b465ba17658d927fb96a73e8b44736d8f887))

### Added
- TL;DR section (with colored examples) inside the ROI explainer modal.

## [1.1.1] - 2026-11-20 ([0d1bae4](https://github.com/Maxxxxior/poe-strat-calculator/commit/0d1bae467edb655c20a6efc2de1cd9cd6044504e))

### Changed
- Simpler ROI explanation referring to chaos and divines instead of "coins".

## [1.1.0] - 2026-11-20 ([7bc7b30](https://github.com/Maxxxxior/poe-strat-calculator/commit/7bc7b30601023884dd3e2ed3e1bba93793d9152f))

### Added
- Nicknames such as "xXx_Chris_Kisser_xXx" and players under a strategy expandable by clicking its name.
- Pie chart of players' share of the result (percentages or divines/chaos, showing lead over others and gap to the leader).
- Option to pick an existing friends' strategy when creating a new one, with similar-name suggestions.
- PoE-style tooltip modals (hover to preview, click to pin, drag to move), starting with ROI.

## [1.0.0] - 2026-11-20 ([84c770a](https://github.com/Maxxxxior/poe-strat-calculator/commit/84c770aaf3932e9e043bec6282c7721ae7a6eeca))

### Added
- Farming calculator: strategies, runs (time, cost, drop value), net profit, profit per hour, and strategy comparison.
- "Random drop" column with a toggle to include it in results.
- Chaos/divine exchange rate with automatic display in div or c and CSV export.
- Sharing data with friends via Firebase and a shared comparison table.