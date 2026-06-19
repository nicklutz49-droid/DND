# Frontier Campaign — A Claude Code DM System

A sandbox, rules-light fantasy campaign run by Claude as your Dungeon Master. You play a
**newcomer to a contested frontier** who, over a long campaign (years or decades of
in-game time), grows from an unproven arrival into someone who can **effect real change** —
build reputation, grow settlements, run businesses, and maybe found a nation.

This is a **Claude Code** project: the world lives as files that Claude reads and updates
as you play, so it persists and accumulates across sessions.

---

## Quick Start

1. **Open this folder in Claude Code.** `CLAUDE.md` loads automatically — it's the DM's
   brain and operating rules.
2. **Start a session.** Tell Claude something like:
   > *"Let's begin. Run character creation, then start Session 1."*
   Claude will see your character sheet is an empty template and walk you through building
   your character (`character/CHARACTER-CREATION.md`), then open the story.
3. **Play.** Describe what you do. Claude narrates, voices NPCs, and resolves outcomes by
   judgment (no dice) based on your plan, your character, and a little luck.
4. **End a session.** Say:
   > *"Let's wrap up — run the session-chronicler."*
   It consolidates everything that happened into the world files and writes a recap.
5. **Skip time between sessions** (optional). Say:
   > *"Three months pass — run the world-simulator."*
   The world moves on its own: factions maneuver, the Empire advances, settlements change,
   the date rolls forward.

Later sessions: just say *"Continue the campaign"* — Claude reads the latest recap and
current state and picks up where you left off.

---

## How It Works

| Folder / File | What it holds |
|---|---|
| `CLAUDE.md` | **The DM instructions** — tone, pacing, resolution, plot philosophy, all auto-loaded. |
| `rules/attributes.md` | The attribute scale (what a 10 vs. a 30 looks like) + Luck. |
| `rules/skills.md` | Skill list and proficiency tiers (classless; learn abilities in play). |
| `rules/resolution.md` | How the DM decides success/failure without dice. |
| `character/` | Your character sheet + the creation walkthrough. |
| `world/` | **Known** world: world bible, factions & reputation, locations, NPCs, calendar/timeline. |
| `inventory/` | Coin, items, property, businesses, late-game nation assets. |
| `dm-secrets/` | **DM-only.** Hidden lore, undiscovered places, secret agendas, and the Empire metaplot. *You agree not to open this — it's what keeps discovery real.* |
| `sessions/` | One recap file per session — the campaign's memory. |
| `.claude/agents/` | The three subagents (below). |

### The Subagents
- **`session-chronicler`** — end of session: folds events into the world files, writes the recap.
- **`world-simulator`** — between sessions: advances the date and simulates the world off-screen.
- **`cartographer`** — on demand: generates new towns and locations, splitting public from secret.

You can invoke any of them by asking Claude to "run the [name]," or Claude will reach for
them at the right moments.

---

## The Design, in One Breath
- **Sandbox.** Your choices steer everything; the DM offers hooks but never rails you.
- **Skill over luck.** Outcomes hinge on your plan and your character; luck only nudges.
- **The world remembers.** Consequences are written down — reputations, deaths, growth, holdings.
- **Failure bends the story, never ends it.** You can lose, be captured, be arrested — but
  there's **no permadeath**, so a long campaign can't be wiped by one bad turn.
- **Secrets are earned.** The DM knows far more than you do; you discover it by playing.
- **A slow-burn metaplot** (the Empire's true design) hums under everything you can choose
  to chase or ignore.

### The two ground rules for *you*
1. **Don't open `dm-secrets/`.** Let the world surprise you.
2. **Run the chronicler when you stop**, so nothing gets lost between sessions.

Now open this in Claude Code and say *"Let's begin."*
