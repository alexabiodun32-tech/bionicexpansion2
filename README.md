# Bionic's Chaos: Expansion (Minecraft 1.21.1 / NeoForge)

The second mod. It adds upgradable pickaxes, mob-themed swords, animated 3D enemies, five bosses
(with a final boss), and rideable vehicles.

**You need all three in your `mods` folder:**
1. **Bionic's Ultimate Chaos** (Mod 1, `bionicchaos-1.0.0.jar`), for the Power Cores this mod builds on
2. **Bionic's Chaos: Expansion** (this mod, `bionicexpansion-1.0.0.jar`)
3. **GeckoLib** for NeoForge 1.21.1 (free on Modrinth / CurseForge), which draws the animated models

## Build the .jar
Push this folder to its own GitHub repository. The workflow in `.github/workflows/build.yml` builds it.
Open the **Actions** tab, wait for the green tick, then download **bionicexpansion-jar** from the bottom of the run.
Or with Java 21 installed: `./gradlew build` and the jar is in `build/libs/`.

## Progression
Normal Minecraft → Power Cores (Mod 1) → Bionic enemies → Bosses → Quantum technology → Final boss → Ultimate gear

Upgrades are made at a **Smithing Table** with a **Bionic Upgrade Template**
(craft: Power Core + diamond + 2 iron ingots → 2 templates).

### Pickaxes (smithing chain)
| Pickaxe | Made from | Built-in ability |
|---|---|---|
| Speed Pickaxe | Diamond pickaxe + Speed Core | Mines extremely fast |
| Bionic Pickaxe | Speed Pickaxe + Bionic Alloy | Huge durability |
| Magma Pickaxe | Bionic Pickaxe + Mutant Core | Auto-smelt, fire resistance while held |
| Quantum Pickaxe | Magma Pickaxe + Guardian Core | Vein mine (crouch + mine an ore) |
| Void Pickaxe | Quantum Pickaxe + Titan Core | 3x3 mining, magnet, night vision |
| Ultimate Pickaxe | Void Pickaxe + Quantum Heart | Everything, unbreakable, Power Mode |

**Upgrade modules** add an ability to any Bionic pickaxe: hold the module, hold the pickaxe in your other hand, right-click.
Vein Mine, 3x3 Mining, Auto-Smelt, Magnet, Durability (x3), Power Mode (right-click the pickaxe for 10 s of insane speed).

### Swords (smithing)
| Sword | Made from | Right-click |
|---|---|---|
| Mutant Cleaver | Diamond sword + Mutant Core | Roar that blasts mobs away |
| Plasma Sword | Diamond sword + Bionic Alloy | Fires a plasma bolt |
| Alien Saber | Diamond sword + Alien Core | Teleport dash + invisibility |
| Speed Blade | Diamond sword + Speed Core | Lightning dash |
| Titan Hammer | Netherite sword + Titan Core | Ground slam |
| Guardian Blade | Netherite sword + Guardian Core | Energy shield |
| Alien King's Scepter | Netherite sword + Alien King Core | Lifts every enemy around you |
| Quantum Blade | Netherite sword + Quantum Heart | Quantum blast volley |

### Enemies (spawn at night / in the dark)
| Enemy | Where | Drops |
|---|---|---|
| Mutant Zombie | Everywhere in the Overworld | Mutant Core |
| Bionic Soldier | Plains, savanna, meadows, badlands, dark forests | Bionic Alloy |
| Alien | Deserts, badlands, mushroom fields, the End | Alien Core |
| Speed Demon | The Nether | Speed Core |
| Titan | Mountains | Titan Core |
| Experiment | Swamps, dark forests, lush caves | Random cores |

### Bosses
Craft a summoning item and right-click, or very rarely meet one in the wild.
| Boss | Summoner | Wild in | Drop |
|---|---|---|---|
| The Bionic Guardian ⭐⭐⭐ | Guardian Beacon | Dark forests, dripstone caves | Guardian Core |
| The Alien King ⭐⭐⭐⭐ | Alien King Signal | The End | Alien King Core |
| The Speed Demon ⭐⭐⭐⭐ | Speed Demon Sigil | Basalt deltas, crimson forests | Speed Demon Core |
| The Titan ⭐⭐⭐⭐⭐ | Titan Reactor | Mountains | Titan Core |
| The Quantum Entity ⭐⭐⭐⭐⭐⭐ | Quantum Rift (needs all four boss cores + nether star) | Never | **Quantum Heart** |

The Quantum Heart makes the Ultimate Pickaxe, the Quantum Blade and the **Ultimate Power Core**
(Mod 1's Bionic Super Core + Quantum Heart: flight and every power from anywhere in your inventory).

### Vehicles
| Vehicle | Craft | How to drive |
|---|---|---|
| Hoverbike | 3 Bionic Alloy + Speed Core + iron block + minecart | Right-click to get in, W to go, steer with the mouse. Glides over water and lava. |
| Jet | 4 Bionic Alloy + Alien Core + elytra + firework rocket | Hold W to fly where you look, let go to hover. |
Crouch to get out. Hit a vehicle until it breaks to get the item back.

## Commands (cheats on)
| Command | Does |
|---|---|
| `/bionic give pickaxes` / `upgrades` / `swords` / `vehicles` / `summoners` / `ultimate_power_core` | Gives that set |
| `/bionic summon guardian` / `alien_king` / `speed_demon` / `titan` / `quantum_entity` | Summons a boss in front of you |

Mod 1's `/bionic` commands keep working too.

## Files
- Models: `assets/bionicexpansion/geo/entity/*.geo.json` (open them in Blockbench to edit)
- Animations: `assets/bionicexpansion/animations/entity/*.animation.json`
- Textures: `assets/bionicexpansion/textures/entity/*.png`, plus a `*_glowmask.png` for the parts that glow in the dark
