# Game_Rules.md

**Revision:** 1
**Updated:** 2026-02-17 15:52:00 IST
**Scope:** System rules usable by any DM (human or LLM)

------------------------------------------------------------------------

## 1. Introduction

This document defines the core game rules for running adventures in this system. 

------------------------------------------------------------------------

## 2. Core Resolution Mechanic (Xd6 vs DC)

### 2.1 Checks

1.  Choose the relevant attribute.
2.  Roll AttributeScore d6.
3.  Sum results.
4.  If sum >= DC, succeed. Otherwise, fail.

### 2.2 Advantage / Disadvantage

1.  Advantage: +1d6 to the pool.
2.  Disadvantage: -1d6 from the pool, minimum 1d6.

### 2.3 Standard Difficulty Ladder (DM Reference)

1.  5 Easy
2.  8 Standard
3.  12 Hard
4.  16 Very Hard
5.  20 Extreme

DC values are hidden from the player.

------------------------------------------------------------------------

## 3. Attributes

All characters use four attributes:

1.  Strength abbreviated to STR
2.  Dexterity abbreviated to DEX
3.  Wits abbreviated to WIT
4.  Influence abbreviated to INF

### Attribute Guidelines

1.  Strength: melee, endurance, physical force.
2.  Dexterity: stealth, ranged, initiative.
3.  Wits: perception, lore, tactics.
4.  Influence: persuasion, deception, intimidation.

------------------------------------------------------------------------

## 4. Character Creation (Level 1)

### 4.1 Fixed Starting Values

1.  Level = 1
2.  Max HP = 20
3.  Current HP = 20
4.  Gold = 10
5.  Starting item: Healing Herbs x1

### 4.2 Player Choices

1.  Name
2.  Distribute exactly 10 points across attributes
    1.  Minimum 1
    2.  Maximum 4
3.  Buy equipment using available gold.
4.  Optional: Short narrative background

------------------------------------------------------------------------

## 5. Combat Encounters

There are two encounter types: combat encounters (this section) and social encounters (Section 6).

### 5.1 When Combat Starts

Combat begins when both are true:

1.  Hostile intent is established.
2.  Immediate timing matters, meaning the order of actions can change what happens (for example: interrupting an attack, reaching cover first, escaping first, or preventing an objective).

If combat starts because someone declares an opener attack:

1.  Roll initiative first.
2.  Resolve the declared opener on the attacker's first turn, if they can still spend an action to attack when that turn arrives.
3.  If the attacker cannot attack before their first turn (for example due to surprise, stun, or another effect), the opener attack does not occur.

### 5.2 Initiative

1.  Roll DexterityScore d6.
2.  Subtract equipped weapon initiative penalty.
3.  Highest total acts first.
4.  If a hero and an enemy tie, the enemy acts first.
5.  If enemies tie with each other, the DM may decide their order arbitrarily.
6.  Initiative totals can go below 0.

### 5.3 Surprise

Surprise applies when one side is unaware and the other initiates hostilities.

1.  A surprised combatant loses all 3 actions on their first turn only.
2.  After that first turn ends, surprise no longer applies to that combatant.

### 5.4 Turn Structure

Each combatant gets 3 actions each turn.

1.  Attack is an action.
2.  Move is an action.
3.  Switch weapon is an action.
4.  Draw weapon is an action.
5.  Hide is an action.
6.  Attempt surrender is an action.
7.  Using a healing potion is an action.

Examples:
1.  Attack, Move, Attack
2.  Attack, Attack, Attack

### 5.5 Attacks

1.  Melee uses Strength.
2.  Ranged uses Dexterity.
3.  Roll attribute d6.
4.  If result >= target Defense, hit.

5.  If a combatant attacks more than once on the same turn:
    1.  First attack: regular dice pool.
    2.  Second attack: roll one fewer d6 (-1d6).
    3.  Third attack: roll two fewer d6 (-2d6).
6.  Apply advantage/disadvantage and other dice modifiers first, then apply multi-attack penalties.
7.  Minimum attack roll is 1d6 after all modifiers.

### 5.6 Defense

1.  Hero Defense = 9 + floor(Dexterity / 2)
2.  Typical enemy Defense = 9
3.  Elite enemy Defense = 12

### 5.7 Damage

1.  Melee: weapon.damage + floor(Strength / 2)
2.  Ranged: weapon.damage + floor(Dexterity / 2)
3.  Minimum 1 damage on hit

### 5.7.1 Applying Damage and Defeat

1.  Subtract damage from the target's current HP.
2.  If current HP is 0 or below, the target is defeated.

### 5.8 Status Effects

Poisoned
1. Disadvantage on all checks and attacks.
2. Duration: 3 rounds or until cured.

Stunned
1. Lose 1 action on next turn.
2. Duration: 1 turn.

### 5.9 Hiding in Combat

1.  You can hide only when fiction supports it (cover, darkness, clutter, smoke, or similar).
2.  Hiding costs 1 action.
3.  Make a Dexterity check against a hidden DC set by the DM.
4.  On success, you become Hidden.
5.  On failure, you remain visible.
6.  Distance affects hiding:
    1.  At close distance, hiding is harder (higher DC) unless you have strong concealment.
    2.  At longer distance, hiding is easier when line of sight is broken or obscured.
    3.  If an enemy is adjacent and has clear line of sight, you cannot become Hidden.
7.  While Hidden:
    1.  Your first attack from Hidden gets +1d6.
    2.  Attacking reveals your position; Hidden ends after the attack resolves.
    3.  Enemies that cannot clearly locate you attack with -1d6.
8.  Hidden also ends if:
    1.  You move into clear open view.
    2.  An enemy uses an action to search and succeeds a Wits check.

### 5.10 Surrender Attempt (Combat Action)

1.  The hero may spend 1 action to attempt to make enemies surrender.
2.  Resolve as an Influence check against enemy Morale DC (hidden).
3.  On success, the target enemy group may surrender, flee, or drop weapons (DM choice based on fiction).
4.  On failure, enemies refuse and continue combat.
5.  Default Morale DC:
    1.  Minions: 9
    2.  Trained: 12
    3.  Elite: 15
6.  Common modifiers:
    1.  +3 DC if enemies clearly outnumber the hero.
    2.  -3 DC if enemy leader is down or enemy group is at half HP.
7.  Repeated surrender attempts in the same combat are harder:
    1.  First attempt: normal dice pool.
    2.  Second attempt: roll one fewer d6 (-1d6).
    3.  Third and later attempts: roll two fewer d6 (-2d6).
    4.  Minimum surrender-attempt roll is 1d6 after all modifiers.
8.  Apply advantage/disadvantage and other dice modifiers first, then apply repeated-attempt penalties.

------------------------------------------------------------------------

## 6. Social Encounters

### 6.1 Social Stance System

For significant social scenes (negotiations, interrogations, alliances), track a stance:

1.  Hostile
2.  Wary
3.  Neutral
4.  Open

Rules:
1.  Start stance based on context (usually Wary or Neutral).
2.  Each meaningful social check can shift stance by 1 step:
    1.  Success: shift 1 step toward Open.
    2.  Failure: shift 1 step toward Hostile or create a complication.
3.  Repeating the exact same argument without new leverage should not grant another roll.
4.  A new roll requires a changed approach, new evidence, or a concession.

### 6.2 Social Pressure and Outcomes

Social scenes can still de-escalate conflict, but combat surrender attempts are resolved under Section 5.10.

### 6.3 Proof Steps (Social Encounters)

A proof step is concrete evidence or a completed task that addresses a demand (for example: bring proof, complete a test, demonstrate intent).

When a proof step is completed, the DM chooses one effect (no roll required):
1.  Shift stance +1 toward Open.
2.  Grant a scene-only bonus of +1d6 to the next relevant social check.
3.  Scene bonuses are temporary; each use reduces remaining uses by 1, and bonuses are removed when uses reach 0.
4.  All scene-only bonuses are cleared when the scene ends.

### 6.4 Recruiting NPC Help

NPC helpers can assist, but they must not replace hero agency in major actions.

1.  Helpers may support in minor ways (warnings, distractions, carrying gear, simple errands).
2.  Helpers must not resolve the main objective on the hero's behalf.

------------------------------------------------------------------------

## 7. Weapons and Equipment

### 7.1 Melee Weapons
1. Iron Sword: cost 8, damage 3, initiative penalty 1.
2. Battle Axe: cost 10, damage 4, initiative penalty 2.
3. Dagger: cost 3, damage 2, initiative penalty 0.
4. War Hammer: cost 12, damage 4, initiative penalty 3.

### 7.2 Ranged Weapons
1. Shortbow: cost 8, damage 3, initiative penalty 1.
2. Crossbow: cost 12, damage 4, initiative penalty 2.
3. Throwing Knives: cost 5, damage 2, initiative penalty 0.
4. Longbow: cost 15, damage 4, initiative penalty 2.

### 7.3 Misc Items

Misc items are non-weapon inventory items.
Misc items do not use damage or initiative_penalty fields.
1. Healing Herbs: cost 3 gold, +3 HP, out of combat only.
2. Healing Potion: cost 8 gold, +6 HP, usable in combat and using it costs 1 action.
3. Rope (50 ft): cost 2 gold.
4. Torch: cost 1 gold.
5. Bedroll: cost 2 gold.
6. Rations (1 day): cost 1 gold.
7. Lockpick Set: cost 6 gold.


------------------------------------------------------------------------

## 8. Healing and Rest

Short Rest
1. Up to 3 times per day.
2. Heal 3 + floor(level / 2).
3. Short Rest uses reset when a Long Rest is completed.
4. A day is defined as the period between completed Long Rests.

Long Rest
1. Safe location required.
2. Restore HP to full.

Healing items can be used during play when available in inventory. In combat, only potions can be used and they cost 1 action. Herbs cannot be used in combat.

------------------------------------------------------------------------

## 9. Progression (Milestone)

Milestone progression is gated by the adventure.

1.  Progression occurs only when a milestone is explicitly declared reached by the adventure flow.
2.  No level-up is granted from XP totals, enemy defeats, or elapsed time unless the adventure explicitly says so.
3.  The DM must clearly announce the milestone in-session before applying progression.

4.  Level +1.
5.  Choose:
    1.  +1 attribute, or
    2.  +2 max HP and +2 current HP.

------------------------------------------------------------------------




