# Traffic Light Controller Design

A Logisim-based digital circuit design for an intelligent traffic light controller. The system manages traffic flow at a two-way intersection and handles pedestrian crossing requests using a Finite State Machine (FSM).

## Project Overview

The controller regulates traffic at the intersection of North-South (NS) and East-West (EW) roads, incorporating a pedestrian crossing cycle triggered by a push button.

### Key Components
* **FSM State Memory:** A subcircuit that determines the next state based on the current state, a timer counter, and the pedestrian request button latch.
* **Output Logic:** A combinational logic subcircuit that decodes the active state into signals for the traffic lights (Red, Yellow, Green) and the pedestrian walk indicator.
* **Controller Implementation:** Built using D Flip-Flops for state registers, a 4-bit counter for timing states, and basic logic gates.

## Repository Contents

* **comp1_design.circ:** The Logisim circuit file containing the main simulation, `StateMemory`, and `OutputLogic` subcircuits.
* **Traffic Light Controller Design.pptx:** Presentation slides detail the state diagram, state transition tables, truth tables, and Boolean equations.
* **20-13-26.mp4:** A screen recording demonstrating the simulation run, showing the cycle transition and pedestrian request handling.

## Running the Simulation

To run and test the circuit:
1. Open `comp1_design.circ` in [Logisim](http://www.cburch.com/logisim/).
2. Enable automatic clock ticks by selecting **Simulation > Ticks Enabled** (Ctrl + K) in the menu.
3. Use the **Poke Tool** (hand icon) to press the pedestrian button and trigger the crossing cycle.
4. Adjust simulation speed if needed under **Simulation > Tick Frequency**.
