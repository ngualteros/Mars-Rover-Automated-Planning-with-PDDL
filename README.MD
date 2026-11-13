
# Mars Rover Automated Planning with PDDL

## Overview

This project explores automated planning techniques for autonomous Mars rover missions using the Planning Domain Definition Language (PDDL).

Developed as part of my Master's degree in Artificial Intelligence at Universidad Internacional de La Rioja (UNIR), the project focuses on modeling planning domains, defining exploration objectives, extending existing scenarios, and evaluating the behavior of automated planners.

The experiments involve autonomous rovers performing exploration tasks, navigating between waypoints, collecting samples, and coordinating activities under predefined planning constraints.

The project demonstrates practical concepts in symbolic Artificial Intelligence, knowledge representation, automated reasoning, and classical planning.

## Project Objectives

- Understand automated planning using PDDL.
- Model actions, predicates, initial states, and goals.
- Extend an existing Mars rover planning domain.
- Introduce new exploration locations and objectives.
- Explore planning scenarios involving multiple rovers.
- Modify domain actions to represent additional constraints.
- Analyze planner behavior and solution feasibility.
- Compare planning scenarios based on generated plans and execution characteristics.

## Technologies and Concepts

**Artificial Intelligence**
- Symbolic AI
- Automated Planning
- Knowledge Representation
- Classical Planning
- Automated Reasoning

**Planning Tools**
- PDDL (Planning Domain Definition Language)
- Delfi Automated Planner

**Planning Concepts**
- Domain Modeling
- Actions and Predicates
- Preconditions and Effects
- Initial States and Goal States
- Multi-Agent Planning Scenarios
- Plan Feasibility Analysis

## Project Structure

```text
mars-rover-automated-planning/
├── README.md
├── .gitignore
│
├── pddl/
│   ├── base/
│   │   ├── domain.pddl
│   │   └── problem.pddl
│   │
│   ├── waypoint-extension/
│   │   └── problem.pddl
│   │
│   ├── multi-rover/
│   │   └── problem.pddl
│   │
│   └── terrain-preparation/
│       ├── domain.pddl
│       └── problem.pddl
│
└── docs/
    └── experiment_results.md
```

## Planning Methodology

### 1. Base Planning Domain

The initial scenario uses an existing PDDL domain representing autonomous rover operations.

The domain defines the actions, conditions, and effects required for rover exploration tasks.

The corresponding problem file specifies the available objects, initial conditions, and mission objectives.

Files:
- `pddl/base/domain.pddl`
- `pddl/base/problem.pddl`

### 2. Waypoint Extension

The first extension introduces an additional exploration location (`waypoint4`) and modifies the problem definition to incorporate new exploration objectives.

This experiment demonstrates how changes in objects, initial conditions, and goals affect the planning problem.

File:
- `pddl/waypoint-extension/problem.pddl`

### 3. Multi-Rover Planning

The second scenario introduces an additional rover to explore planning behavior involving multiple autonomous agents.

The experiment examines how rover capabilities, task allocation, and planning constraints influence the feasibility of a solution.

The original academic experiment encountered difficulties obtaining a complete solution for the initial multi-rover configuration.

A reduced set of objectives was subsequently used to validate a more manageable planning scenario.

File:
- `pddl/multi-rover/problem.pddl`

### 4. Terrain Preparation

This scenario extends the original planning domain with additional actions related to terrain preparation.

The objective is to explore how new action definitions, preconditions, and effects influence the planning process.

Unlike the previous scenarios, this experiment modifies both the domain and problem definitions.

Files:
- `pddl/terrain-preparation/domain.pddl`
- `pddl/terrain-preparation/problem.pddl`

## Automated Planning Workflow

The general workflow followed in this project includes:

1. Define the planning domain using PDDL.
2. Specify the initial state and mission objectives.
3. Introduce modifications to the planning scenario.
4. Execute the domain and problem using a compatible automated planner.
5. Inspect generated plans or planner failures.
6. Analyze feasibility, planning complexity, and execution characteristics.
7. Compare the behavior of the different scenarios.

## How to Run

### Requirements

A PDDL-compatible automated planner is required.

The original academic experiments used Delfi.

No Python dependencies are required for the PDDL files themselves.

### 1. Clone the Repository

```bash
git clone https://github.com/ngualteros/Mars-Rover-Automated-Planning-with-PDDL.git
```

### 2. Select a Planning Scenario

For example, the base scenario uses:

```text
pddl/base/domain.pddl
pddl/base/problem.pddl
```

### 3. Execute the Planner

Load the corresponding domain and problem files into a compatible PDDL planner.

For the waypoint extension and multi-rover scenarios, use the base domain together with the corresponding problem file.

For the terrain preparation scenario, use its modified domain and problem files.

The exact execution command depends on the selected planner and its installation method.

### 4. Analyze the Results

Inspect the generated plan and verify whether the mission objectives were satisfied.

Depending on the planner output, analyze:

- Plan feasibility.
- Number of actions.
- Planning time.
- Generated action sequence.
- Effects of domain and problem modifications.

## Experiments and Observations

The academic work explored progressively more complex planning scenarios.

### Base Scenario

Used to understand the existing rover planning domain and validate the initial planning setup.

### Extended Waypoint

Introduced new exploration objectives requiring modifications to the planning problem.

### Multi-Rover Scenario

Explored planning with an additional rover.

The complete initial configuration presented planning difficulties, and a reduced scenario was used to obtain a feasible solution.

### Terrain Preparation

Extended the planning domain with additional action definitions and constraints.

Detailed numerical results and generated action sequences should be added after reproducing the experiments.

## Limitations

- The project extends an existing academic PDDL domain rather than implementing an automated planner from scratch.
- Some multi-rover configurations were not successfully solved.
- Planner execution depends on external PDDL-compatible software.
- The reorganized scenarios must be validated after publication.
- Execution metrics have not yet been independently reproduced in the repository.

## Future Improvements

- Validate all scenarios using a reproducible planner configuration.
- Add automated PDDL validation.
- Document generated plans for each scenario.
- Compare additional planning algorithms.
- Analyze planning time and plan cost across scenarios.
- Create Python scripts to automate planner execution.
- Visualize rover movement and mission progression.

These improvements are proposed future work.

## Academic Context

**Course:** Automated Reasoning and Planning  
**Degree:** Master's in Artificial Intelligence  
**University:** Universidad Internacional de La Rioja (UNIR)

The project was developed as part of an academic laboratory focused on automated planning for Mars rover exploration.

The original planning domain was provided as part of the academic exercise. The project includes modifications and experiments involving exploration objectives, multiple rovers, and domain extensions.

## Author

**Nicolás Gualteros Pérez**

Systems Engineer | Master's in Artificial Intelligence

AI Engineering | Machine Learning | Symbolic AI | Automation

LinkedIn: https://www.linkedin.com/in/nicogualteros
