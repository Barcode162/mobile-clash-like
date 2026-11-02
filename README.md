# Stackfort

A mobile-first merge tower defense game. You duel an AI commander lane against lane, send attackers to raise your income, and upgrade a Clash-style base between battles.

Open `index.html` in any browser. It has no build step and no dependencies. All art is drawn in code, and the sound is synthesized.

## Modes
- **Duel:** you and an AI commander each defend your own lane, and the first gate to fall loses.
  - Waves arrive every 22 seconds on both lanes.
  - Sending attackers to the other lane raises your income, which pays out every 6 seconds.
  - Tap the opponent's name to watch their lane live.
  - Winning earns trophies and ranks, from Recruit up to Legend. The AI gets stronger as your trophies rise.
- **Endless Siege:** survive as many rounds as you can.

## Battle systems
- **Merge:** drag a tower onto one with the same type and level to level it up, to a maximum of 8.
- **Branches:** at level 4 every tower picks one of two specializations. Examples are Ballista → Repeater or Siege Bolt, and Mortar → Cluster or Quake.
- **Runes:** buy runes to the bench and drag them into tower sockets. Towers have 1 socket, 2 at Lv 3 and 3 at Lv 5.
  - Merging two matching runes on the bench raises the tier, from I to III.
  - The six runes are Ember, Rime, Venom, Volt, Haste and Focus.
- **Fusions:** certain rune pairs on one tower unlock a bonus. Examples are Thermal Shock, Overdrive, Corrosion, Deadeye, Superconductor and Weak Point.
- **Stacking synergy:** 3 or more towers of one type give +20% damage, and 5 or more give +40%. Running 3–4 different types gives an attack-speed bonus.
- **Enemy traits that need counters:**
  - Armor (Brute, Colossus) reduces small hits.
  - Shields (Bulwark) take double damage from splash and burns.
  - Splitters burst into mites.
  - Wraiths stay hidden until a Railgun or Focus rune spots them.
  - Menders heal nearby enemies.
- **Powers:** Meteor (tap a target), Blizzard and Overcharge, each on a cooldown.

## Towers
| Tower | Role | Unlocks at |
|---|---|---|
| Ballista | Fast single-target bolts | TH 1 |
| Mortar | Lobbed splash shells | TH 1 |
| Frost Spire | Slows | TH 1 |
| Pyre | Flame cone that ignores armor | TH 2 |
| Tesla Coil | Chain lightning | TH 3 |
| Railgun | Piercing beam that spots Wraiths | TH 4 |

## Base (between battles)
Battles pay out **Crowns**, which you spend on:
- **Town Hall:** unlocks towers, runes and powers, and raises every cap.
- **Tower cards:** permanent +15% damage per level. Kills also earn mastery stars.
- **Loadout:** pick up to 4 towers. Buying a tower in battle draws from this loadout.
- **Buildings:**
  - Mint: more starting coins.
  - Bastion: more lives.
  - Forge: chance to buy a Lv 2 tower.
  - Arcanum: chance to buy a tier II rune.
  - Watchtower: faster power recharge.
  - Treasury: more Crowns.

Progress is saved in the browser's localStorage.
