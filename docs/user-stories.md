# User Stories

Each story links to the requirements in `requirements.md`.

## US1: Compare communication strategies

**As a** researcher, **I want** to run the same disruption under different communication strategies, **so that** I can compare their delay and message cost fairly.

**Related requirements:** FR3, FR6

**Acceptance criteria**
1. Selecting a strategy runs only that strategy in the simulation.
2. Every strategy's results use the same five metrics: train delay, journey completion, deadlock count, waiting time and message count.

## US2: Coordinate only when a conflict is detected

**As a** researcher, **I want** trains to communicate only when a conflict is detected, **so that** I can see whether coordination works with fewer messages.

**Related requirements:** FR4, FR5

**Acceptance criteria**
1. In a run with no shared-track conflicts, the message count is 0.
2. When a conflict is detected, messages are sent only between the trains involved in it.

## US3: Export results for analysis

**As a** researcher, **I want** the results of each run exported to a file, **so that** I can analyse and chart them in my FYP.

**Related requirements:** FR7

**Acceptance criteria**
1. Each run produces one file containing all five metrics.
2. The file opens correctly in a spreadsheet application.