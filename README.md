# Stackfort

A mobile-first merge tower defense game with a Clash-style base to upgrade between runs.

Open `index.html` in any browser (phone or desktop). No build step and no dependencies.

## Battle (merge tower defense)
- **Buy tower** places a random Lv 1 tower on a free tile. Each buy costs 3 more coins than the last.
- **Merge:** drag a tower onto one with the same type and level to make the next level (max Lv 8).
- **Move / swap:** drag onto an empty tile or onto a different tower.
- **Sell:** drag onto the Sell bin.
- **Stack synergy:** 3+ towers of one type give that type +20% damage, and 5+ give +40%. Merging lowers the count, which creates a trade-off.
- **Mixed army:** 4 different tower types give +10% attack speed, and all 5 give +20%.
- Every 5th wave adds tanks, and every 10th wave brings a boss. You can play at 1×/2×/3× speed or turn on Auto waves.

| Tower  | Role                    | Unlocks at |
|--------|-------------------------|------------|
| Archer | Fast single target      | TH 1       |
| Cannon | Splash                  | TH 1       |
| Frost  | Slow                    | TH 2       |
| Flame  | Burn damage over time   | TH 3       |
| Storm  | Chain lightning         | TH 4       |

## Base (upgrade layers)
Cleared waves pay out **Crowns**, which you spend at your base:
- **Town Hall** (max 8) unlocks towers and sets the level cap for everything else.
- **Tower cards** give +20% damage per level, up to Town Hall level + 1.
- **Mastery stars** come from every 150 kills with a tower type, worth +4% damage each, up to 5.
- **Buildings** are capped at Town Hall level:
  - Coin Mine gives more starting coins.
  - Walls give more lives.
  - Forge gives a chance to buy a Lv 2 tower.
  - Treasury gives more Crowns.

Progress is saved in the browser's localStorage.

## Ideas for next steps
- Builder timers with stacking helpers
- Prestige resets for maxed cards
- Stacked buildings on one tile (for example Wall + Cannon)
- More maps and enemy types (flying, shielded, healers)
- Sound and music
