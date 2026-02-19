# Ashwood Bandit Problem
## Revision: 3
## Generated: 2026-02-16 15:02:05

Designed to conform with the current Adventure Creation Guidelines, Game Rules, and LLM Rules.

---

# 1. Core Premise

Grey Hollow is economically collapsing due to repeated attacks on the Old Timber Road.
The Ashwood Bandits are disciplined former soldiers led by Captain Rowan Ash, who claims the crown has engineered scarcity for profit.

Primary Objective:
- Stabilize the Old Timber Road through force, alliance, or political exposure.

Secondary Objectives:
- Identify who is manipulating regional trade.
- Decide whether Captain Rowan is an enemy, a temporary ally, or a witness.

---

# 2. Opening Hook

At dawn, Grey Hollow's mill bell rings in panic: a supply wagon from the Old Timber Road arrives burned, with two wounded guards and a stamped crown crate split open.

Immediate ask to hero:
- The council requests urgent action before sunset to prevent famine pricing and unrest.
- A survivor says the attackers shouted about \"stolen bread and blood tariffs,\" pointing to the Ashwood Bandits.

Why now:
- If no action is taken today, merchants raise prices and the first local deadline clock starts.
- The hero is offered legal authority to investigate, negotiate, or strike immediately.

First-scene leads:
1. Social lead: question Old Bram at Forest Edge for route intelligence.
2. Combat lead: pursue fresh tracks toward the direct ambush route.

Discovery-gated content (DM-only; do not reveal before discovery):
1. Hidden trail route that can bypass or soften the first ambush setup.
2. Ledger-page clue pointing to the chapel records chamber.
3. Crown witness identity tied to the `crown_coverup` clock.

---

# 3. Factions and Negotiation Anchors

Grey Hollow Council:
- Public stance: restore order immediately.
- Private concern: fear of losing tax and supply lines.

Ashwood Bandits:
- Public stance: armed resistance against corrupt trade policy.
- Private concern: low supplies, poor morale among newer recruits.

Regional Crown Office:
- Public stance: "bandit suppression."
- Private concern: concealment of trade manipulation evidence.

Town Merchant - Elric Voss:
- Role: quartermaster and legal trader in Grey Hollow market square.
- Inventory: sells standard equipment at regular prices from `Game_Rules.md` Section 7.
- Default buyback policy: buys items from the hero at 1/4 of listed item cost.
- Persuasion tier 1 (successful social leverage): buyback improves to 1/2 of listed item cost.
- Persuasion tier 2 (further successful leverage): buyback improves to 3/4 of listed item cost.
- Hard limit: Elric will never sell equipment below listed price and cannot be persuaded to give purchase discounts.

Negotiation viability notes:
- Every major faction has negotiable motives.
- Boss-level dialogue is always possible before violence is finalized.

---

# 4. Locations and Travel Times

1. Grey Hollow to Forest Edge
   - Distance class: close
   - Duration: 1 hour
   - Route safety: safe
   - Random encounter risk: low

2. Forest Edge to Secondary Trail (discoverable)
   - Distance class: short journey
   - Duration: 30 minutes
   - Route safety: contested until a local guide or clue is secured
   - Random encounter risk: medium

3. Forest Edge to Watchtower Ruins (direct)
   - Distance class: short journey
   - Duration: 2 hours
   - Route safety: risky
   - Random encounter risk: high

4. Watchtower Ruins to Chapel Courtyard
   - Distance class: close
   - Duration: 10 minutes
   - Route safety: contested
   - Random encounter risk: low

5. Grey Hollow to Regional Capital
   - Distance class: full day
   - Duration: 1 day
   - Route safety: contested
   - Random encounter risk: medium

Travel affects daylight, short-rest opportunity, and active clocks.

---

# 5. Time Pressure and Clocks

Scene-bound clock examples (`scene.json.clocks`):
1. Clock id: alarm_raised
   - Segments: 4
   - Trigger: Bandit reinforcements enter current combat scene.

2. Clock id: convoy_window
   - Segments: 6
   - Trigger: Convoy departs; negotiation leverage drops.

Global clock example (`world_state.json.clocks`):
1. Clock id: crown_coverup
   - Segments: 6
   - Trigger: Key witness disappears and evidence route changes.

Clock advancement guidance:
- Advance on loud failures, prolonged indecision, travel on risky routes, or failed social leverage attempts.
- State active deadline pressure in non-combat interactions when it applies.

---

# 6. Encounter Flow Overview

1. Social Encounter: Old Bram at Forest Edge.
2. Combat Encounter: Forest Ambush.
3. Combat Encounter: Ruined Watchtower.
4. Defeat Transition or Infiltration Phase (if captured or stealth route fails).
5. Boss Negotiation and/or Boss Combat at Chapel Courtyard.
6. Planning Phase (if temporary alliance or ceasefire is formed).
7. Resolution Path and Milestone.

---

# 7. Social Encounter - Old Bram

Location:
- Forest-edge cabin.

Intent:
- Gain route intelligence, avoid early attrition, and obtain proof-step leverage.

Scene tone cues:
- Damp pine air, kettle smoke, and creaking shutters.
- Bram is cautious, practical, and tired of empty promises.

Check framing:
- Primary: Influence (negotiate trust)
- Alternative: Wits (offer actionable information)

Success outcomes:
- Reveals a safer secondary route (reduces ambush positioning advantage).
- Grants one proof-step bonus for next relevant social check: +1d6, 1 use.
- Adds a clue about relocated trade records in the chapel complex.

Failure consequences (non-combat):
- Lose time: +1 hour.
- Worse position: direct route only.
- Increased suspicion: Bram warns lookouts, making stealth entry harder.

If the player hesitates, offer options:
1. Ask Bram for the safest route and local dangers.
2. Offer proof of intent (coin, favor, or recovered clue).
3. Pressure Bram with urgency about the road collapse.
4. Other.

---

# 8. Combat Encounter 1 - Forest Ambush

Location:
- Narrow woodland pass.

Enemies:
1. Bandit Scout
   - Defense tier: Typical (9)
   - HP: 10
   - Primary weapon: Shortbow (type: ranged, damage: 3, initiative_penalty: 1)
   - Secondary weapon: Dagger (type: melee, damage: 2, initiative_penalty: 0)
   - Carried items: 6 arrows, 2 silver
   - Tactical role: ranged pressure and relocation

2. Bandit Thug
   - Defense tier: Typical (9)
   - HP: 12
   - Primary weapon: Iron Sword (type: melee, damage: 3, initiative_penalty: 1)
   - Secondary weapon: Throwing Knives (type: ranged, damage: 2, initiative_penalty: 0)
   - Carried items: crude map fragment, 4 silver
   - Tactical role: front-line lock and surrender pressure

Environment:
- Dense brush allows hide attempts where fiction supports concealment.
- Fallen cart can provide cover but blocks direct movement lane.

Opening beat:
- Arrows snap through brush as a shouted warning echoes from the trees.

Loot on victory:
- Shortbow, Dagger, Iron Sword, Throwing Knives
- Map fragment (clue item)
- 6 silver

Defeat transition:
- If hero reaches 0 HP, hero is captured and moved to Watchtower holding chamber.

If the player hesitates, offer options:
1. Push to cover and return ranged fire.
2. Rush the front-line thug to break formation.
3. Attempt a surrender action after applying pressure.
4. Other.

---

# 9. Combat Encounter 2 - Ruined Watchtower

Location:
- Collapsing stone watchtower complex.

Enemies:
1. Bandit Guard A
   - Defense tier: Typical (9)
   - HP: 11
   - Primary weapon: Spear (type: melee, damage: 3, initiative_penalty: 1)
   - Secondary weapon: Dagger (type: melee, damage: 2, initiative_penalty: 0)
   - Carried items: 3 silver
   - Tactical role: zone control

2. Bandit Guard B
   - Defense tier: Typical (9)
   - HP: 11
   - Primary weapon: Spear (type: melee, damage: 3, initiative_penalty: 1)
   - Secondary weapon: Throwing Knives (type: ranged, damage: 2, initiative_penalty: 0)
   - Carried items: tower key
   - Tactical role: flank and intercept

3. Optional reinforcement if `alarm_raised` clock fills
   - Bandit Runner
   - Defense tier: Typical (9)
   - HP: 8
   - Primary weapon: Dagger (type: melee, damage: 2, initiative_penalty: 0)
   - Carried items: signal whistle

Environment:
- Weak masonry can be collapsed with a successful Strength approach.
- High rubble provides partial cover for ranged combatants.

Opening beat:
- Loose stones shift underfoot while sentries call positions from cracked battlements.

Loot on victory:
- 2 Spears, Dagger, Throwing Knives
- Tower key
- 6 silver

Defeat transition:
- Hero captured, disarmed, and equipment moved to a locked side chamber (recoverable).

If the player hesitates, offer options:
1. Use rubble cover and isolate one guard.
2. Try to collapse weak masonry to split enemies.
3. Attempt stealth repositioning before committing.
4. Other.

---

# 10. Defeat Continuation and Capture Phase

If captured, the adventure continues with social and planning opportunities.

Available approaches:
1. Influence: bluff a sentry for movement rights.
2. Wits: identify patrol pattern and escape window.
3. Influence: request audience with Captain Rowan.
4. Strength or Dexterity: physical escape attempt.

Consequences on failure:
- Time loss and clock advancement.
- Increased guard suspicion.
- Resource cost (consumable or positioning loss).

Short rest handling:
- Allowed only in fictionally safe windows (patrol gap, hidden alcove, or secured room).

If the player hesitates, offer options:
1. Bluff for movement rights and gather info.
2. Track patrol timing and plan a quiet escape.
3. Request direct audience with Captain Rowan.
4. Other.

---

# 11. Boss Phase - Captain Rowan Ash

Location:
- Burned chapel courtyard and attached records chamber.

Boss profile:
- Defense tier: Elite (12)
- HP: 18
- Primary weapon: War Hammer (type: melee, damage: 4, initiative_penalty: 3)
- Secondary weapon: Dagger (type: melee, damage: 2, initiative_penalty: 0)
- Carried items: Trade Ledger, Crown Signet, sealed dispatch note
- Special trait: once per combat, one hit may apply Stunned

Pre-combat negotiation is always available:
- Captain Rowan argues the crown created scarcity.
- Proof steps (ledger fragment, witness statement, convoy records) can shift stance and open non-combat outcomes.

Boss outcomes (minimum three paths):
1. Combat defeat
   - Bandit command structure collapses.
   - Road stabilizes quickly but political truth may be delayed.

2. Conditional alliance
   - Rowan stands down in exchange for exposing crown corruption.
   - Hero remains principal decision-maker; bandits only assist in limited ways.

3. Political exposure without alliance
   - Hero secures ledger and signet, forcing regional inquiry.
   - Bandits disperse or flee depending on pressure.

If the player hesitates, offer options:
1. Open negotiation with evidence first.
2. Demand surrender and terms before combat.
3. Initiate combat immediately.
4. Other.

---

# 12. Planning Phase (If Ceasefire or Alliance Occurs)

Planning objective:
- Intercept convoy and expose falsified tariffs before `convoy_window` expires.

Planning choices:
1. Recruit village volunteers (support role only; no objective replacement).
2. Stage diversion near ruined mill.
3. Assign proof courier to Grey Hollow council.
4. Set fallback route for withdrawal.

Volunteer constraints:
- Volunteers can distract, carry messages, and secure exits.
- Volunteers cannot resolve the main objective for the hero.

If the player hesitates, offer options:
1. Build a diversion-first plan.
2. Prioritize courier/evidence delivery.
3. Set an extraction route and fallback signal.
4. Other.

---

# 13. Resolution Paths and Milestone Gating

Resolution path flags (examples for `world_state.json`):
1. Force Resolution
   - `bandit_command_active: false`
   - `timber_road_open: true`

2. Alliance Resolution
   - `bandit_truce_active: true`
   - `crown_inquiry_pending: true`

3. Exposure Resolution
   - `crown_agent_exposed: true`
   - `trade_reform_motion: true`

Milestone declaration trigger:
- Milestone is reached only when the adventure explicitly declares road stabilization or corruption exposure complete.

---

# 14. Save and Resume Breakpoints

Recommended clean save points:
1. After Old Bram social encounter resolves.
2. After each combat encounter fully resolves.
3. At start of boss phase (before first boss roll).
4. After final resolution state is applied.

Minimum resumable state expectations:
- Active location and scene label
- Encounter outcomes so far
- Current clocks and in-game time/day
- Critical flags tied to selected resolution path

---

# 15. Escalation Hook for Next Adventure

The Trade Ledger names a regional crown official in the capital and references parallel operations in two neighboring routes.

Future arc seeds:
1. Political confrontation in the capital.
2. Convoy protection under contested authority.
3. Investigation of a wider trade manipulation network.
