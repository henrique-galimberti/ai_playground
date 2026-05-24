# Ant Colony Simulator

A real-time ant colony simulation demonstrating emergent behavior through pheromone-based foraging algorithms.

## Overview

This simulator models how real ant colonies discover food sources and establish efficient foraging paths using pheromone trails. Each ant operates on simple rules, yet the colony as a whole exhibits complex, self-organizing behavior.

## How It Works

- **Pheromone Trails**: Ants deposit two types of pheromones:
  - **Blue (to-food)**: Deposited when searching for food, follows trails left by successful foragers
  - **Red (to-home)**: Deposited when carrying food, guides other ants back to the nest
- **Sensor System**: Each ant samples pheromone concentrations at three points ahead (left, center, right) and steers toward the strongest signal
- **Evaporation**: Pheromones fade over time, allowing the colony to adapt when food sources are depleted

## Controls

| Control | Description |
|---------|-------------|
| Ant Count | Number of active ants (20-800) |
| Ant Speed | Movement speed of ants |
| Sensor Range | How far ahead ants can detect pheromones |
| Turn Speed | How quickly ants can change direction |
| Pheromone Strength | Amount of pheromone deposited per step |
| Evaporation | Rate at which pheromone trails fade (0.95-0.999) |
| Food Amount | Units of food per source |

## Keyboard Shortcuts

- **Space**: Pause/Resume
- **R**: Reset simulation
- **F**: Add random food source
- **Click canvas**: Place food at cursor position

## Running

Open `index.html` in any modern browser. No build step or dependencies required.
