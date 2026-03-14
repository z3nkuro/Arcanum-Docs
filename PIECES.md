# Spell Pieces

Generated from `PieceCatalog` so UI, unlock pools, and docs stay aligned.

## Invocation

| Piece | ID | Unlock |
| --- | --- | --- |
| Invoke Self<br><sub>Retrieve the caster position.</sub> | `arcanum:trigger_self` | Default |
| Invoke Mark<br><sub>Retrieve the targeted position.</sub> | `arcanum:trigger_target` | TRIGGER codex (12) |
| Invoke Gaze<br><sub>Raycast to a hit position.</sub> | `arcanum:trigger_raycast` | TRIGGER codex (10) |
| Invoke Vessel<br><sub>Launch a projectile trigger payload.</sub> | `arcanum:trigger_projectile` | TRIGGER codex (7) |
| Bind Glyph<br><sub>Place a trigger zone that runs deferred effects.</sub> | `arcanum:trigger_place_trigger` | TRIGGER codex (4) |

## Manifestation

| Piece | ID | Unlock |
| --- | --- | --- |
| Manifest Bolt<br><sub>Launch a projectile with explicit origin and direction.</sub> | `arcanum:construct_projectile` | TRIGGER codex (6) |
| Shape Vector<br><sub>Build a vector from X/Y/Z components.</sub> | `arcanum:construct_vector` | LOGIC codex (8) |

## Effects

| Piece | ID | Unlock |
| --- | --- | --- |
| Unleash Ruin<br><sub>Deal direct structural damage.</sub> | `arcanum:effect_damage` | Default |
| Mend Essence<br><sub>Restore target health.</sub> | `arcanum:effect_heal` | Default |
| Raise Ward<br><sub>Apply a temporary ward shield.</sub> | `arcanum:effect_shield` | EFFECT codex (7) |
| Arcane Force<br><sub>Apply kinetic force to an entity.</sub> | `arcanum:effect_impulse` | EFFECT codex (12) |
| Translocate<br><sub>Teleport an entity.</sub> | `arcanum:effect_teleport` | EFFECT codex (5) |
| Kindle Flame<br><sub>Ignite a target.</sub> | `arcanum:thermal_ignite` | EFFECT codex (9) |
| Bind Frost<br><sub>Freeze a target.</sub> | `arcanum:thermal_freeze` | EFFECT codex (8) |
| Quench Flame<br><sub>Remove the burn effect from a target.</sub> | `arcanum:thermal_extinguish` | EFFECT codex (9) |
| Arcane Rupture<br><sub>Create an explosion at a position.</sub> | `arcanum:effect_explosion` | EFFECT codex (5) |
| Bind Motion<br><sub>Apply a slowing status effect.</sub> | `arcanum:effect_slow` | EFFECT codex (8) |
| Ascend<br><sub>Apply a levitation status effect.</sub> | `arcanum:effect_levitate` | EFFECT codex (7) |
| Haste<br><sub>Increase a target's movement speed.</sub> | `arcanum:effect_speed_boost` | EFFECT codex (11) |
| Fracture Matter<br><sub>Break a block at the target position.</sub> | `arcanum:world_break_block` | EFFECT codex (8) |
| Shape Matter<br><sub>Place the Arcanum magic block.</sub> | `arcanum:world_place_block` | EFFECT codex (7) |
| Lumos<br><sub>Place a temporary magical light block.</sub> | `arcanum:world_place_light` | EFFECT codex (6) |
| Arcane Surge<br><sub>Schedule a periodic area effect.</sub> | `arcanum:effect_area_of_effect` | EFFECT codex (3) |

## Perception

| Piece | ID | Unlock |
| --- | --- | --- |
| Self<br><sub>Resolve the caster entity.</sub> | `arcanum:info_self_entity` | Default |
| Marked Presence<br><sub>Resolve the targeted entity.</sub> | `arcanum:info_target_entity` | TRIGGER codex (11) |
| Vessel<br><sub>Resolve projectile payload hits to an entity.</sub> | `arcanum:info_projectile_entity` | TRIGGER codex (7) |
| Nearest Presence<br><sub>Find the nearest entity to a position.</sub> | `arcanum:info_nearest_entity` | TRIGGER codex (8) |
| Nearby Presences<br><sub>List entities in a radius.</sub> | `arcanum:info_entities_in_radius` | TRIGGER codex (7) |
| Discern Bearing<br><sub>Calculate a normalized bearing between two positions.</sub> | `arcanum:info_direction_to` | TRIGGER codex (8) |
| Presence Facing<br><sub>Read the facing direction of any entity.</sub> | `arcanum:info_get_facing` | TRIGGER codex (9) |
| Gaze Presence<br><sub>Raycast to an entity.</sub> | `arcanum:info_raycast_entity` | TRIGGER codex (9) |
| Gaze Distance<br><sub>Raycast to a distance value.</sub> | `arcanum:info_raycast_distance` | TRIGGER codex (8) |
| Gaze Surface<br><sub>Raycast to a surface normal.</sub> | `arcanum:info_raycast_normal` | TRIGGER codex (8) |
| Position<br><sub>Read the caster position.</sub> | `arcanum:get_position` | TRIGGER codex (7) |
| Presence Position<br><sub>Read any entity position.</sub> | `arcanum:info_get_position` | TRIGGER codex (9) |
| Count<br><sub>Count items in an entity list.</sub> | `arcanum:list_length` | LOGIC codex (6) |
| Extract Presence<br><sub>Select an entity from a list by index.</sub> | `arcanum:list_get_entity` | LOGIC codex (5) |

## Arcana

| Piece | ID | Unlock |
| --- | --- | --- |
| Number Sigil<br><sub>Emit a constant number.</sub> | `arcanum:constant_number` | Default |
| Vector Sigil<br><sub>Emit a constant vector.</sub> | `arcanum:constant_vector` | LOGIC codex (8) |
| Combine<br><sub>Add two numbers.</sub> | `arcanum:math_add` | Default |
| Subtract<br><sub>Subtract two numbers.</sub> | `arcanum:math_subtract` | Default |
| Amplify<br><sub>Multiply two numbers.</sub> | `arcanum:math_multiply` | Default |
| Diminish<br><sub>Divide two numbers.</sub> | `arcanum:math_divide` | LOGIC codex (12) |
| Modulo<br><sub>Take the remainder of a division.</sub> | `arcanum:math_modulo` | LOGIC codex (8) |
| Purify<br><sub>Return the absolute value of a number.</sub> | `arcanum:math_abs` | LOGIC codex (10) |
| Lesser<br><sub>Return the lesser of two numbers.</sub> | `arcanum:math_min` | LOGIC codex (9) |
| Greater<br><sub>Return the greater of two numbers.</sub> | `arcanum:math_max` | LOGIC codex (9) |
| Chaos<br><sub>Emit a pseudo-random number.</sub> | `arcanum:math_random` | LOGIC codex (11) |
| Spiral Bearing<br><sub>Emit a Fibonacci-sphere unit direction.</sub> | `arcanum:math_fib_dir` | LOGIC codex (2) |
| Merge Vectors<br><sub>Add two vectors.</sub> | `arcanum:vector_add` | LOGIC codex (7) |
| Subtract Vectors<br><sub>Subtract two vectors.</sub> | `arcanum:vector_subtract` | LOGIC codex (7) |
| Amplify Vector<br><sub>Scale a vector.</sub> | `arcanum:vector_scale` | LOGIC codex (7) |
| Normalise Vector<br><sub>Normalize a vector.</sub> | `arcanum:vector_normalize` | LOGIC codex (5) |
| Vector Strength<br><sub>Measure vector length.</sub> | `arcanum:vector_magnitude` | LOGIC codex (5) |
| Turn Vector<br><sub>Rotate a vector around the Y axis.</sub> | `arcanum:vector_rotate_y` | LOGIC codex (4) |
| Equal<br><sub>Compare two numbers for approximate equality.</sub> | `arcanum:compare_eq` | LOGIC codex (9) |
| Greater<br><sub>Compare two numbers with greater-than.</sub> | `arcanum:compare_gt` | LOGIC codex (9) |
| Lesser<br><sub>Compare two numbers with less-than.</sub> | `arcanum:compare_lt` | LOGIC codex (9) |
| Conjunction<br><sub>Boolean conjunction.</sub> | `arcanum:logic_and` | LOGIC codex (8) |
| Union<br><sub>Boolean disjunction.</sub> | `arcanum:logic_or` | LOGIC codex (8) |
| Negate<br><sub>Boolean negation.</sub> | `arcanum:logic_not` | LOGIC codex (8) |
| Judgement<br><sub>Select between two values based on a boolean.</sub> | `arcanum:logic_conditional` | LOGIC codex (6) |
| Converge<br><sub>Intersect two entity lists.</sub> | `arcanum:logic_intersection` | LOGIC codex (3) |
| Separate<br><sub>Subtract one entity list from another.</sub> | `arcanum:logic_difference` | LOGIC codex (3) |
| Delay Mark<br><sub>Attach delay time to deferred effects.</sub> | `arcanum:modifier_delay` | LOGIC codex (4) |

## Iteration

| Piece | ID | Unlock |
| --- | --- | --- |
| Cycle<br><sub>Repeat a spell graph a fixed number of times.</sub> | `arcanum:loop_range` | LOGIC codex (4) |
| Cycle Index<br><sub>Emit the current loop index.</sub> | `arcanum:loop_index` | LOGIC codex (5) |
| Channel<br><sub>Repeat while cast input remains held.</sub> | `arcanum:channel` | LOGIC codex (3) |

## Utility

| Piece | ID | Unlock |
| --- | --- | --- |
| Sigil Link<br><sub>Bridge distant nodes without adding runtime behavior.</sub> | `arcanum:connector` | LOGIC codex (7) |
| Arcane Trace<br><sub>Print runtime values for debugging.</sub> | `arcanum:debug_print` | LOGIC codex (4) |

