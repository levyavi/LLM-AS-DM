# LLM-AS-DM

LLM-AS-DM is a lightweight tabletop RPG framework for running adventures with an LLM acting as Dungeon Master.
It separates:
- game mechanics (`Game_Rules.md`)
- LLM behavior and state protocol (`LLM_Rules.md`)
- adventure content (`Ashwood_Adventure.md` and future adventures)

## Project Purpose

This repository is designed to make LLM-led adventures:
- mechanically consistent
- narratively immersive
- stateful across sessions

## Starting an Adventure Usage

1. Open `Game_Rules.md`, `LLM_Rules.md`, and an adventure file (for example `Ashwood_Adventure.md`).
2. Start a new chat/session with your LLM.
3. Provide both rules files + adventure as context.
4. Tell the model to run as DM using these rules.
5. Play by describing actions in plain language.
6. At session end, or at any points that you would like to stop, ask the LLM to give you a save zip bundle. Save the bundle file.

## Continuing From a Save Bundle

Use this flow to continue an existing adventure from a prior save:

1. Locate the exported bundle zip file.
2. In a new LLM session, provide:
   - `Game_Rules.md`
   - `LLM_Rules.md`
   - the active adventure file (for example `Ashwood_Adventure.md`)
   - The Zip bundle
4. Instruct the DM to resume from loaded state (do not reinitialize character, world time, or scene/combat state unless intentionally starting over).
5. Continue play normally, then export a new end-of-session save bundle.

## Recommended Session Flow

1. Character setup using `Game_Rules.md` Section 4.
2. Run scenes from the selected adventure.
3. Resolve checks/combat/social outcomes using `Game_Rules.md`.
4. Enforce DM conduct, roll transparency, memory logging, and state handling from `LLM_Rules.md`.
5. Save/export state at the end of the session.

## Repository Files

- `Game_Rules.md`  
  Core system mechanics: checks, combat, social encounters, items, rest, and milestone progression.

- `LLM_Rules.md`  
  Operational rules for the LLM DM: hard behavior constraints, conflict resolution priority, dice-roll transparency, file authority model, schema requirements, time tracking, and save protocol.

- `Ashwood_Adventure.md`  
  Example adventure module ("Ashwood Bandit Problem") with locations, encounters, transitions, and resolution paths.

- `Adventure_Creation_Guidelines.md`  
  Design standards for building new adventures that are compatible with this system.

- `AGENTS.md`  
  Repository-local working rules for Codex contributors/editors (editing constraints, validation expectations, and safety rules).

- `README.md`  
  This file.

## Runtime State Files (Used During Play)

These are defined in `LLM_Rules.md` Section 9 and are expected during active sessions:
- `hero.json`
- `world_state.json`
- `combat.json`
- `scene.json`
- `long_memory.md`

They may be generated/updated as gameplay progresses, even if they are not committed as static source files in this repository.

## Creating a New Adventure

1. Start from `Adventure_Creation_Guidelines.md`.
2. Write a new `*_Adventure.md` file with clear social/combat structure and continuation states.
3. Ensure compatibility with `Game_Rules.md` mechanics.
4. Ensure DM-operational compatibility with `LLM_Rules.md` (state tracking, time pressure, and logging rules).
