# Factorio 2.1 promotion compatibility

Promotions use current entity health/fluid APIs and retain entity quality. Native ammunition stacks are copied slot by slot, retaining partial ammunition and item data; fluid storage amount/type/temperature and connector wiring are transferred before the old entity is removed. The replacement keeps flags, combat statistics, force and direction. Native turret base visualisations are recognized so all four vanilla turret classes receive their four original ranks, including flamethrower turrets.

Native Factorio 2.1.24 headless scenarios exercised 16 actual enemy-kill-triggered promotions (four turret types by four ranks), followed by 250 ticks. Base and rare-quality profiles passed. Assertions covered partially used ammunition, fluid amount and temperature, health, quality, force, direction, combat statistics, flags and circuit connections. An original-function regression fixture reproduced the removed max_health API failure. No graphical badge-rendering or real multiplayer client claim is made.

Original PixelWhipped/ModMash history and authorship are retained through an explicit subtree extraction. The original portal license is GNU LGPLv3; COPYING.LESSER and COPYING contain the corresponding GNU license texts.

Native namespace migration uses migrates_from and adopts the complete original storage root before initialization. It retains root cycles, object references and engine-transferred owned objects. Existing target state is never silently overwritten: overlapping keys reject the import before mutation, while disjoint target fields are retained by the shared legacy_import helper. Literal prototype names, setting names and metatable identifiers remain stable.

Public namespace: heroturrets-updated 1.0.0 adopts the original complete storage root through native migrates_from. Native headless adoption and subsequent save/reload retain root cycles, domain aliases, rendering ownership, script inventory quality/partial ammo/durability and entity references. Original prototype, setting and remote interface identifiers remain unchanged.

Native migration preserves all 48 historical generated Rampant turret items across Rampant's authentic base-item renames, keeping rank and matching generated target. Native target checks confirm all 48 target items and recipes exist. Original recipe IDs remain available; Factorio1.1 had no recycling recipes, so no speculative recipe alias is introduced.
