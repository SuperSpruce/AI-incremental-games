# Particle Clicker - Game Design Document

## Game Overview
A prestigious incremental game about manipulating particles to generate energy, with multiple prestige layers and deep progression mechanics.

## Core Concept
Players click to generate particles, upgrade to get generators, and eventually unlock paradigm shifts that multiply their progress by resetting with bonuses.

## Main Progression Layers

### Layer 1: Particle Generation (Baseline)
- **Manual**: Click button to generate 1 particle
- **Generators**: 
  - Emitters (1 particle/sec) - cost scales by exponential
  - Resonators (10 particles/sec) - higher tier
  - Accelerators (100 particles/sec) - even higher
- **Upgrades**: Improve click power, generator efficiency
- **Threshold**: 1 trillion particles
- **Paradigm Shift 1**: Quark Conversion
  - Reset to 0 particles
  - Unlock Quarks (prestige currency)
  - Players gain Quarks based on particles earned
  - Quarks provide permanent multiplier to particle generation

### Layer 2: Quark Mastery (First Prestige)
- **Goal**: Accumulate multiple Quark levels
- **New Generators**: 
  - Quark Collectors (generate particles faster with Quarks)
  - Tensor Matrices (unlock new mechanics)
- **Upgrades**: Quark efficiency multipliers
- **Threshold**: 100 Quarks
- **Paradigm Shift 2**: Dimensional Fold
  - Reset Quarks to 0
  - Unlock Dimensions (second prestige currency)
  - Dimensions provide base multiplier to all other resources

### Layer 3: Dimensional Power (Second Prestige)
- **Goal**: Unlock the true endgame
- **New Mechanics**: Synergies
  - Certain upgrades give bonuses when you have both particle generators AND high Quarks
  - Dimensions unlock special passive effects
- **Challenges**: Mini-achievements that test playstyle
- **Final Content**: With high Dimensions, enable a third paradigm shift for true "endgame"

### Layer 4: Quantum Entanglement (Endgame)
- **Goal**: Reach high quantum levels through repeating prestige cycles
- **Mechanics**: Exponential growth through synergies
- **The Grand Achievement**: Get to 1000 Quantum levels (easily achievable with endgame mechanics)

## Achievement System

### Early Game (0-20% progress)
1. "First Steps" - Generate 100 particles
2. "Builder" - Buy your first generator
3. "Mass Producer" - Generate 1M particles total

### Mid Game (20-60% progress)
4. "Exponential Thinking" - Have all 3 base generator types active
5. "Paradigm Shift" - Reach Quark Conversion (Paradigm Shift 1)
6. "Quark Master" - Accumulate 50 Quarks
7. "Synergy Unlocked" - Use a synergy bonus (special upgrade)
8. "Dimensional Breakthrough" - Reach Dimensional Fold (Paradigm Shift 2)

### Late Game (60-100% progress)
9. "Dimension Collector" - Accumulate 10 Dimensions
10. "True Quantum State" - Reach Quantum Entanglement (Paradigm Shift 3)
11. "Infinity Reached" - Reach 1000 Quantum levels (easy endgame grind)

## Game Balance Philosophy
- Each prestige layer should feel like starting fresh but with multiplicative bonuses
- Upgrades should feel impactful (never buy something that doesn't feel good)
- Time to each prestige should take:
  - Layer 1→2: 5-10 minutes
  - Layer 2→3: 10-15 minutes
  - Layer 3→4: 15-20 minutes
  - Layer 4+: Repeating cycles, each ~10 minutes but exponentially more rewarding

## Technical Implementation
- Single HTML file with embedded CSS and JS
- Save system: localStorage with JSON serialization
- Export: JSON string to copy/paste
- Import: Paste JSON to load
- No external libraries

## File Structure
- `index.html` - Main game file with all HTML, CSS, and JS
- `Planning.md` - This design document

## Development Checklist
- [ ] Core game loop (clicking, basic particles)
- [ ] Generator system (Emitters, Resonators, Accelerators)
- [ ] Upgrade system with balanced costs
- [ ] First prestige layer (Quark Conversion)
- [ ] Second prestige layer (Dimensional Fold)
- [ ] Third prestige layer (Quantum Entanglement)
- [ ] Synergy system (stat bonuses from combinations)
- [ ] Achievement system (11 achievements)
- [ ] Save/Load system
- [ ] Export/Import system
- [ ] UI polish and balance
- [ ] Playtesting and tuning
