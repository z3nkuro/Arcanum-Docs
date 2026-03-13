# Spell Crafter Guide

Arcanum spells are built as hex-grid programs. Each piece you place becomes part of a graph that your CAD compiles and executes when you cast.

If you are coming from a normal spell mod, the important mental shift is this: you are not picking a finished spell from a list. You are wiring one together.

## Opening the Spell Crafter

Depending on your setup, you will usually interact through the in-game UI and CAD workflow. If commands are enabled on your server, these are also available:

```text
/spellcrafter
/cad load <spell_name>
/castspell <spell_name>
```

## The Short Version

Every spell usually follows the same structure:

1. something starts the cast
2. something provides values or targets
3. something modifies or routes those values
4. an effect consumes the final result

## How the Grid Works

The Spell Crafter uses a hex grid, not a square grid. That matters because each node can pull values from six neighboring directions.

Key rules:

- inputs pull values from adjacent hex neighbors that they face
- colored arrows show typed inputs
- if an input faces the wrong way, rotate it until it points at the node feeding it
- `Sigil Link` is used to bridge gaps when two pieces are too far apart
- math and utility pieces shape values before they reach the final effect

Think of it like this:

1. a trigger starts the cast
2. perception or constant pieces provide data
3. logic or math pieces modify that data
4. an effect consumes the result

## What the Arrows Mean

Every arrow on a piece matters. If a spell is broken, the arrows are usually the first place to look.

- An input arrow means the piece expects data from that side.
- The arrow color tells you what kind of value that input wants.
- If a spell is not compiling, the first thing to check is whether the input arrows are facing the correct neighboring node.

If two pieces look close enough but still do not connect cleanly, insert a `Sigil Link` between them.

## Basic Build Flow

Use this pattern for almost every spell:

1. Place a trigger or starting piece.
2. Add the target, position, entity, or number data the spell needs.
3. Add any math, comparison, or control pieces.
4. Place the final effect piece.
5. Rotate inputs until every required arrow is fed.
6. Save the spell.
7. Load it into your CAD.
8. Cast it in the world and adjust.

## Your First Reliable Test Spell

If you want a simple first success, build a self-heal:

1. place `Self`
2. place `Mend Essence`
3. rotate the input so `Mend Essence` is pulling from `Self`
4. save and cast

This is a better learning spell than a large combat graph because it teaches the core connection rule without adding too many moving parts.

## Common Reasons a Spell Fails

- the CAD does not have enough complexity for the graph
- an input arrow is facing empty space
- you are missing a required piece unlock
- the graph needs a `Sigil Link` to bridge the path
- the spell is valid but your current mana pool is too small to sustain it

## Practical Tips

- Start with very small spells and prove each part works before scaling up.
- Use the Copper CAD to learn layout discipline, then upgrade once you hit slot or complexity limits.
- Keep [PIECES.md](PIECES.md) open while building so you know which codex unlock to chase next.
- If a build feels messy, rebuild it from the effect backward: decide what the spell should do, then feed only the values it actually needs.

## Where to Go Next

- Need a progression overview: [Getting Started](GETTING_STARTED.md)
- Want spell templates to experiment with: [Common Spells](COMMON_SPELLS.md)
- Want to browse every available piece: [PIECES.md](PIECES.md)
