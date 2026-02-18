# Ashwood Bandit Problem
## Revision: 3
## Generated: 2026-02-16 15:02:05

Designed under Adventure Creation Guidelines v4.

---

# 1. Core Premise

Grey Hollow is economically collapsing due to organized attacks along the Old Timber Road. The Ashwood Bandits are disciplined former soldiers operating under ideological motives tied to trade reform and crown corruption.

Primary Objective
- Stabilize the Old Timber Road through elimination, alliance, or political exposure.

Secondary Objectives
- Identify ideological motives of the Ash Captain.
- Discover evidence of Crown manipulation.

---

# 2. Locations and Travel Times

1. Grey Hollow to Forest Edge: 1 hour (Safe).
2. Forest Edge to Hidden Trail Entrance: 30 minutes (Contested if shortcut not gained).
3. Forest Edge to Watchtower Ruins (Direct Route): 2 hours (Risk of ambush).
4. Watchtower Ruins to Central Chapel Courtyard: 10 minutes interior traversal.
5. Grey Hollow to Regional Capital (Future Hook): 1 full day travel.

Travel impacts daylight and countdown timers. Travel during contested routes may trigger encounter checks.

---

# 3. Social Encounter – Old Bram

Location: Forest edge cabin (1 hour from village).

Social Check: DC 9

Success:
- Hidden trail reduces ambush chance.
- Grants tactical positioning advantage in first combat.

Failure:
- Direct forest approach.
- Increased ambush positioning for enemies.

---

# 4. Combat Encounter 1 – Forest Ambush

Location: Narrow woodland path (2 hours from village via direct route).

Enemies:

Bandit Scout
- Defense: 9
- HP: Standard
- Weapon: Short Bow (weapon_damage: 3, ranged)
- Secondary: Dagger (weapon_damage: 2, melee)
- Carried: 5 arrows, 2 silver coins

Bandit Thug
- Defense: 9
- HP: Standard
- Weapon: Rusted Long Blade (weapon_damage: 3, melee)
- Carried: Coin pouch (4 silver), crude map fragment

Environmental:
- Dense cover allows Dexterity DC 9 repositioning.

Loot:
- Short Bow (3, ranged)
- Rusted Long Blade (3, melee)
- 6 total silver coins
- Map fragment (clue item)

Defeat Transition:
- If hero reaches 0 HP, captured and moved to Watchtower holding chamber.

---

# 5. Combat Encounter 2 – Ruined Watchtower

Location: Collapsing stone structure (2 hours from village).

Enemies:

Bandit Guard A
- Defense: 9
- Weapon: Spear (weapon_damage: 3, melee)
- Secondary: Dagger (2)
- Carried: 3 silver coins

Bandit Guard B
- Defense: 9
- Weapon: Spear (3, melee)
- Carried: Tower key

Environmental Interaction:
- Smarts DC 9 to identify weak structure.
- Strength DC 9 to collapse unstable masonry.

Loot:
- 2 Spears (3, melee)
- Tower key
- 6 total silver coins

Defeat Transition:
- Hero captured and disarmed.
- Equipment stored in secured chamber (recoverable).

---

# 6. Capture Continuation Phase

Options:
1. Bluff guard (Social DC 9)
2. Ideological manipulation (Social DC 12)
3. Escape attempt (Dexterity DC 9)
4. Request audience with Ash Captain

Short rest possible only if patrol cycles permit (tracked in time).

---

# 7. Boss Encounter – The Ash Captain

Location: Burned chapel courtyard (10 minutes interior travel).

Defense: 12 (Elite)
HP: Above standard enemies

Equipment:
- Officer’s Blade (weapon_damage: 4, melee)
- Reinforced Leather Armor (Defense 12 tier)
- Ledger of Trade Manipulation (evidence item)
- Signet token of Crown Agent

Special Ability:
- Stunning Strike (once per combat, applies Stunned condition)

Loot (if defeated):
- Officer’s Blade (4, melee)
- Ledger (quest-critical)
- Signet token (political leverage)

---

# 8. Pre-Boss Negotiation

Social DC 12 to engage ideological discussion.

Possible Outcomes:
1. Immediate combat.
2. Temporary ceasefire.
3. Conditional alliance.
4. Political cooperation to expose Crown Agent.

---

# 9. Planning Phase

If alliance forms:

1. Countdown: 1–2 days until trade convoy interception.
2. Recruit volunteers (Social DC 9).
3. Volunteers provide diversion only.
4. Travel staging 10 minutes outside ruins.

Time tracked in World_state.json.

---

# 10. Resolution Paths

1. Eliminate Ash Captain
   - bandits_active: false
   - timber_road_open: true

2. Form Alliance
   - bandits_active: conditional
   - crown_agent_exposed: pending

3. Expose Crown Agent
   - crown_agent_exposed: true
   - trade_restructured: true

Milestone triggered when trade route stabilizes or corruption exposed.

---

# 11. Escalation Hook

Ledger identifies regional Crown official in capital city.

Future Session:
1. Political confrontation in capital.
2. Escort convoy under new terms.
3. Investigate broader trade conspiracy.
