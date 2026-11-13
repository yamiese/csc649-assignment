# Technology Outline (Part C)

Technology area: Multi-agent systems

## C1. Core concepts
Agents, multi-agent systems, communication, coordination (centralised vs decentralised), partial observability.

## C2. Frameworks and tools
- Flatland: rail simulation environment
- pandas: recording and exporting run results
- Matplotlib: plotting delay, deadlock and message-count results
- (Optional) PettingZoo and PyTorch, only if learning agents are added

## C3. Fit to the problem
How multi-agent coordination supports the requirements in `requirements.md`.

## C4. Limitations
Communication overhead, event-triggered communication that may reduce coordination performance, deadlocks that coordination cannot always prevent, and the gap between simulation and real railways.

## C5. Alternative
Centralised scheduling and optimisation, compared with the multi-agent approach.