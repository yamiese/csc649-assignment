# Problem Statement

## Problem

Rail dispatchers and operators must keep trains moving when a disruption occurs on shared track, and passengers bear the cost when they cannot. A single delayed train can hold up others that need the same track section, producing secondary delays and, in the worst case, a deadlock where trains block each other, as described in the Flatland simulation by Kopacz et al. (2022). Trains can avoid this by communicating, but constant communication adds message overhead, while too little leaves each train unaware of upcoming conflicts. It is therefore unclear when trains should coordinate during a disruption. This matters because unresolved conflicts reduce punctuality, journey completion and network capacity.

## Users and stakeholders

| Group | Role |
|---|---|
| Researchers and students of multi-agent coordination | Primary users: run experiments and compare strategies |
| Rail dispatchers and traffic controllers | Beneficiaries of better coordination ideas |
| Train operators | Affected by delays and deadlocks |
| Passengers | Affected by delays (indirect) |
| FYP supervisor and assessors | Review the work |

## Scope

**In scope**
- A small simulated rail network built in Flatland
- Injected disruptions, such as a delayed train
- Four communication strategies: none, periodic, full and conflict-triggered
- Measuring delay, journey completion, deadlocks, waiting time and message count

**Out of scope**
- Real railway data or live deployment
- Safety-certified signalling systems
- Passenger flow and ticketing
- Large-scale or real-time networks