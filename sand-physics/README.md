# Sand Physics Toy

A falling sand simulation with multiple interactive elements and physics.

## Elements

| Element | Behavior |
|---------|----------|
| **Sand** | Falls and piles up like real sand |
| **Water** | Flows and spreads horizontally |
| **Fire** | Rises, burns flammable materials, creates smoke |
| **Smoke** | Rises and dissipates over time |
| **Acid** | Corrodes and dissolves other materials |
| **Lava** | Flows slowly, ignites flammables, creates smoke, solidifies on water contact |
| **Plant** | Static but grows when touching water |
| **Boomer** | Explodes after a short delay or when touched by fire/lava |
| **Oil** | Flows like water, highly flammable |
| **Steam** | Rises, condenses back to water over time |
| **Powder** | Gunpowder — explodes when touching fire or lava |
| **Ice** | Static, freezes nearby water, melts on fire/lava contact |
| **Wall** | Indestructible static barrier |

## Interactions

- Fire + Water = Steam
- Lava + Water = Steam + (sometimes solidifies to wall)
- Acid dissolves most materials (except wall)
- Fire/Lava ignites Plant, Oil, and Powder
- Boomer and Powder explode with a blast radius
- Plant grows when adjacent to water
- Ice freezes adjacent water

## Controls

- **Left click/drag** — Draw selected element
- **Right click/drag** — Erase
- **Brush slider** — Adjust brush size
- **Clear** — Reset the canvas
- **Pause/Play** — Toggle simulation
