# Requirements

## Functional requirements

| ID | Requirement |
|---|---|
| FR1 | The system shall generate a Flatland rail network with a configurable number of trains. |
| FR2 | The system shall inject a configurable disruption (e.g. a train delayed for a set number of timesteps) into a simulation run. |
| FR3 | The system shall let the user select one communication strategy per run: none, periodic, full, or conflict-triggered. |
| FR4 | The system shall detect a potential shared-track conflict between two or more trains before they reach the shared section. |
| FR5 | The system shall send a coordination message between the affected trains only when a conflict is detected, under the conflict-triggered strategy. |
| FR6 | The system shall record train delay, journey completion, deadlock count, waiting time and message count for every run. |
| FR7 | The system shall export the recorded results of each run to a file (e.g. CSV) for comparison. |

## Non-functional requirements

| ID | Type | Requirement |
|---|---|---|
| NFR1 | Performance | A 25x25 simulation with 3 trains shall complete within 60 seconds on the development laptop. |
| NFR2 | Reproducibility | Running the same configuration with the same random seed shall produce identical results in 10 out of 10 repeated runs. |
| NFR3 | Usability | A new user shall be able to run a simulation using the README instructions alone, in 5 steps or fewer. |
| NFR4 | Reliability | The simulation shall complete 30 consecutive runs per strategy without crashing. |