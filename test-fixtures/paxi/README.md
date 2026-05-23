# Paxi beta smoke test packs

Copy the contents of `datapacks` to `<instance>/minecraft/config/paxi/datapacks`.
Copy the contents of `resourcepacks` to `<instance>/minecraft/config/paxi/resourcepacks`.
Copy `datapack_load_order.json` and `resourcepack_load_order.json` to `<instance>/minecraft/config/paxi`.

Expected in-game checks:

- Create a new world with cheats enabled.
- `/datapack list enabled` should include `paxi-smoke-datapack-alpha` and `paxi-smoke-datapack-beta`.
- Put one dirt in the crafting grid. The test recipe should output an emerald if load ordering is honored.
- `/function paxi_smoke:give_marker` should give the player one emerald.
- Open resource packs/options or inspect a diamond item name. It should be `Paxi Beta Ordered Diamond` if resource pack ordering is honored.
