# Vault Wish (Fabric, Minecraft 1.21.11)

Client-side mod for Trial Chamber vaults.

## Commands
- `/vaultwish add`       add the item in your main hand to the wish list
- `/vaultwish addid <item>`    add any item by name, e.g. `/vaultwish addid mace` (tab-complete works)
- `/vaultwish removeid <item>`  remove any item by name
- `/vaultwish addvault`  add the item the vault you're looking at is displaying
- `/vaultwish remove`    remove the held item
- `/vaultwish list` / `/vaultwish clear`
- `/vaultwish auto on|off`   auto-use the key (held in main/off hand) when a wanted item is displayed (default off)
- `/vaultwish guard on|off`  block key use when the vault shows an unwanted item

## What it does
- Look at a vault: if it displays a wanted item you get an action-bar alert + sound.
- Key guard: right-clicking a vault with a (ominous) trial key is cancelled client-side
  unless the displayed item is on your list.

## Build
1. Install JDK 21.
2. Update versions in gradle.properties from https://fabricmc.net/develop
3. Run `gradle wrapper` once (or open in IntelliJ), then `./gradlew build`.
4. Jar is in build/libs/ -> put in your mods folder with Fabric API.
