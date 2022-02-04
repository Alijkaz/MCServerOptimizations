# FAQ

## Iron Farms are not working correctly
Try enabling the `tick-inactive-villagers` in **spigot.yml** (`tick-inactive-villagers: false`)

## Mobs spawned from a spawner are dumb (they don't do anything)
Try disabling `nerf-spawner-mobs` in **spigot.yml** (`nerf-spawner-mobs: false`)
They're nerfed so that they have no AI upon spawning from a spawner, You also can enable `spawner-nerfed-mobs-should-jump` in **paper.yml** without changing `nerf-spawner-mobs` to make the mobs jump while in water

## One of my plugins that uses armorstands is not working or acting weird
This is probably caused by `armor-stands-tick` in  **paper.yml**. Try fixing the issue by re-enabling it (`armor-stands-tick: true`)

## Hoppers are not working properly
This is probably caused by `hopper-check` and `hopper-transfer` values in **spigot.yml**. try changing them as specified:
```
hopper-transfer: 8
hopper-check: 1
```

## Treasure maps are not working
You can fix this by enabling `enable-treasure-maps` in **paper.yml** (`enable-treasure-maps: true`)
Please note that generating treasure maps is extremely expensive and can hang a server if the structure it's trying to locate is outside of your pregenerated world

