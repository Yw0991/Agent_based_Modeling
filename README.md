# Agent_based_Modeling
Fish Tank Ecosystem Simulation

What it is: A closed-ecosystem simulation where fish agents navigate a virtual tank, competing for food, reproducing, and — when resources get scarce — turning on each other.

Core mechanics:

Movement — Fish swim randomly, but lock onto the nearest food (yellow patch) when they spot it
Energy system — Every tick costs 1 energy point; eating restores 50. Fish die when energy drops below 5
Hunger & color — Hunger climbs each tick. Fish display green (healthy) → red (hungry, >20 ticks without eating)
Cannibalism — When food is nearly gone (food-total < 2) and a fish is very hungry (hunger > 30), it has a 15% chance to hunt the weakest fish in range
Reproduction — Fish with >80 energy have a 5% chance per tick to hatch an offspring (splitting energy 50/50)
Auto food drop — The environment has a 20% chance each tick to spawn a new food item, simulating natural input

What you observe: Classic boom-and-bust population dynamics — the fish count plot shows how the population stabilizes, collapses, or cycles depending on your starting conditions.
Controls: One slider (initial-fish-count, 1–100), plus manual buttons to add fish or food mid-simulation.

Built with: NetLogo 6.4.0
