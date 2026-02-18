# Adventure Creation Guidelines 

**Revision:** 1
**Updated:** 2026-02-19 01:44:06 +02:00
**Scope:** Standards for designing adventure content compatible with `Game_Rules.md` and `LLM_Rules.md`; not a replacement for core mechanics or DM operational rules.


------------------------------------------------------------------------

# 1. Adventures Must Support Continuation After Defeat

1.  Every major encounter must define a Defeat Transition State.
2.  Capture must create new social or political play opportunities.
3.  Boss encounters should allow post-defeat dialogue.
4.  Defeat should escalate stakes rather than reset progress.

------------------------------------------------------------------------

# 2. Negotiation Must Be Viable at All Tiers

1.  Every major faction must have negotiable motives.
2.  Bosses must have ideology, not just hostility.
3.  Social checks should meaningfully redirect the adventure.
4.  Temporary alliances must be mechanically supportable in
    `world_state.json`.

------------------------------------------------------------------------

# 3. Planning Phases Are Core Gameplay

1.  Include at least one pre-boss planning phase.
2.  Allow players to stage allies or volunteers.
3.  Define explicit time pressure.
4.  Planning must modify encounter framing and positioning.

------------------------------------------------------------------------

# 4. Resource Pressure Must Matter

1.  Ensure HP attrition before major confrontation.
2.  Limit safe rest windows.
3.  Rest must require fictionally justified safety.
4.  Villages may offer limited aid but not unlimited recovery.

------------------------------------------------------------------------

# 5. NPC Durability Across Sessions

1.  Major NPCs must support repeated interaction.
2.  Trust levels must evolve based on player action.
3.  NPC motivations must remain internally consistent.

------------------------------------------------------------------------

# 6. Multiple Resolution Paths Required

1.  Boss must support at least three resolution paths.
2.  `world_state.json` flags must support faction realignment.
3.  Secondary antagonist threads should exist.

------------------------------------------------------------------------

# 7. Combat Structure Standards

1.  2--3 enemies per encounter preferred.
2.  Clear tactical roles per enemy.
3.  Environmental interaction opportunity required.
4.  Avoid excessive enemy counts to preserve state clarity.

------------------------------------------------------------------------

# 8. Equipment and Loot Requirements (Mandatory)

All enemies and all potential combat encounters must include explicit
equipment definitions.

Each enemy must specify:

1.  Primary weapon (name, type, damage, initiative_penalty).
2.  Secondary weapon if applicable (name, type, damage,
    initiative_penalty).
3.  Defense tier.
4.  Carried items.
5.  Potential loot on defeat.

Loot must be:

1.  Concrete and transferable to `hero.json` inventory.
2.  Mechanically defined if weapon or armor.
3.  Economically coherent with setting.
4.  Non-duplicative unless justified.

Boss encounters must include:

1.  Unique item, document, or evidence object.
2.  At least one progression-relevant asset.

No combat encounter may exist without defined equipment and loot
structure.

------------------------------------------------------------------------

# 9. Travel and Movement Time (New Rule)

Adventures must define travel time between major locations.

For every location transition, specify:

1.  Distance classification (close, short journey, half-day, full day,
    multi-day).
2.  Expected travel duration in hours or days.
3.  Whether travel is safe, contested, or risky.
4.  Whether random encounters are possible.
5.  Whether travel consumes daylight or impacts countdown timers.

Travel time must:

1.  Be consistent across sessions.
2.  Integrate with time pressure mechanics.
3.  Affect rest opportunities.
4.  Be trackable in `world_state.json` when relevant.

Time must never be abstract or undefined between locations.

------------------------------------------------------------------------

# 10. Save and Load Integration

1.  Define clean save breakpoints.
2.  Avoid ambiguous mid-resolution states.
3.  Ensure `world_state.json` contains sufficient flags for resumption.
4.  Adventures must be resumable from the standard save bundle containing:
    `hero.json`, `world_state.json`, `combat.json`, `scene.json`, and
    `long_memory.md`.
5.  Avoid requiring hidden off-file context to continue play after load.

------------------------------------------------------------------------

# 11. Political and Economic Stakes

1.  Introduce institutional tension.
2.  Include hidden document or proof mechanics.
3.  Allow systemic conflict beyond immediate enemies.

------------------------------------------------------------------------

# 12. Volunteers and Secondary Actors

1.  Recruitment must require a Social check.
2.  Volunteers must have defined tactical role.
3.  Volunteers must not overshadow hero agency.
4.  Volunteer risk must be meaningful.

------------------------------------------------------------------------

# 13. Explicit Time Tracking

1.  Define countdown elements.
2.  Track days or hours in `world_state.json`.
3.  Time pressure must influence options.
4.  Travel time must integrate with countdown systems.
5.  Scene-bound deadlines should be represented as clocks in `scene.json`.
6.  Long-term/global deadlines should be represented as clocks in
    `world_state.json`.
7.  Adventures should provide clear triggers for clock advancement and
    consequences when clocks complete.

------------------------------------------------------------------------

# 14. System Alignment Requirements

1.  Combat design must assume 3 actions per turn and allow meaningful
    action tradeoffs (attack, move, hide, weapon handling, surrender, potion
    use).
2.  Rest pacing must account for system limits:
    1.  Short Rest can be used up to 3 times per day.
    2.  A day boundary occurs on completed Long Rest.
3.  Social design should include proof-step opportunities that can grant
    scene-only one-use social bonuses.
4.  Milestone progression points must be explicitly declared in the adventure
    flow.
5.  If an adventure intentionally overrides a core rule from
    `Game_Rules.md`, it must state the override explicitly and include a clear
    in-world or design rationale for why the exception is needed.

------------------------------------------------------------------------

# 15. Moral Ambiguity

1.  Boss must have coherent rationale.
2.  Player alignment shift must be viable.
3.  Authority figures should not be automatically correct.
4.  Institutional corruption increases replayability.

------------------------------------------------------------------------

# 16. Escalation Across Sessions

1.  Include unresolved thread.
2.  Include political ripple effect.
3.  Avoid clean narrative closure unless milestone finalizes arc.
4.  Preserve future expansion hooks.

------------------------------------------------------------------------

# Summary

Adventures must:

1.  Support defeat without collapse.
2.  Support alliance without railroading.
3.  Support political branching.
4.  Preserve mechanical determinism.
5.  Encourage tactical planning.
6.  Maintain controlled combat encounters.
7.  Allow negotiation at every conflict tier.
8.  Embed time pressure and scarcity.
9.  Define equipment and loot for all enemies.
10. Define explicit travel duration between locations.
11. Remain JSON-compatible and persistence-safe.
12. Stay aligned with current `Game_Rules.md` and `LLM_Rules.md`.
