# kubejsminestuck
 
simple addon for [kubejs](https://www.curseforge.com/minecraft/mc-mods/kubejs) that adds support for [minestuck](https://www.curseforge.com/minecraft/mc-mods/minestuck)

## current features:
- recipe handlers
    - combination (totem lathe / punch designix)
        - `event.recipes.minestuck.combination(output, input1, mode, input2)`
    - grist costs (alchemiter)
        - `event.recipes.minestuck.grist_cost(item, grist)`
        - when removing, make sure the item is selected as input
    - irradiating (cookalyzer)
        - same syntax and methods as a normal furnace recipe
- Global binding for grist amounts
    - `Grist.of(type, amount)` <- gives single grist amount
    - `GristSet.from(grist, grist, ...)` <- combine multiple into one set
- Ability to add new types of grist
    - still unimplemented
