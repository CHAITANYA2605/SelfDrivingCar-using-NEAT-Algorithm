# Self-Driving Car with NEAT

A Pygame simulation in which neural networks evolve with NEAT
(NeuroEvolution of Augmenting Topologies) to drive cars around a track.

## Highlights

- Evolutionary training across generations
- Distance sensors for detecting track boundaries
- Fitness-based selection of better drivers
- Real-time visualization of cars and sensor rays
- Configurable NEAT population in `config.txt`

## Run

```bash
git clone https://github.com/CHAITANYA2605/SelfDrivingCar-using-NEAT-Algorithm.git
cd SelfDrivingCar-using-NEAT-Algorithm
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python main.py
```

## Files

| File | Purpose |
| --- | --- |
| `main.py` | Simulation, sensors, fitness evaluation, and rendering |
| `config.txt` | NEAT genome, reproduction, species, and population settings |
| `car.png` | Car sprite |
| `map1.png`, `map5.png` | Track assets |

## How learning works

Each car is controlled by a neural network generated from a NEAT genome.
Sensor values become network inputs; outputs control steering and movement.
Cars earn fitness by surviving and progressing, allowing stronger genomes to
reproduce in later generations.

## Tuning

Experiment with population size, mutation rates, sensor geometry, speed, and
the fitness function. These values strongly affect convergence and driving
behavior.
