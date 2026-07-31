# Adversarial Trajectory Graphs

**External Adversarial Supervision for Long-Horizon Autonomous AI**

Adversarial Trajectory Graphs (ATG) is a working architectural hypothesis for supervising the project-level course of long-horizon autonomous AI systems. The proposed layer sits outside an existing agent or multi-model orchestration system, observes its aggregate project state, and compares its actual course against a versioned, human-authorized trajectory contract.

The architecture uses two independent supervisory loops:

- a **mission adversary** protecting objective fidelity, scope, priority, and completion;
- an **integrity adversary** protecting constraints, evidence, dependencies, and truthful status.

Their findings are reconciled into bounded actions such as continue, warn, redirect, defer, pause, halt, or escalate. The controlled system remains internally unchanged.

## Paper

- [Working thesis in Markdown](paper/ADVERSARIAL_TRAJECTORY_GRAPHS_THESIS.md)
- [Working thesis in PDF](paper/ADVERSARIAL_TRAJECTORY_GRAPHS_THESIS.pdf)

## Research status

- Working Thesis v1.0.1
- Conceptual and engineering proposal
- Not peer reviewed
- Empirical validation pending
- Originating concept and project direction: **Sam Flynn**
- Research program: **Dark Science Division**

This repository does not claim that ATG creates consciousness, sentience, artificial general intelligence, guaranteed alignment, or guaranteed safety. The thesis specifies falsifiable hypotheses, failure conditions, and an experimental program intended to determine whether ATG materially reduces long-horizon project drift without suppressing productive exploration.

## Core contribution

The proposed contribution is not adversarial debate by itself. It is the separation of two control levels:

1. **Internal adversarial reasoning**, which challenges claims, plans, artifacts, and local decisions.
2. **External adversarial trajectory regulation**, which challenges whether the project as a whole remains directed toward the operator-authorized end state.

## Repository contents

```text
paper/
  ADVERSARIAL_TRAJECTORY_GRAPHS_THESIS.md
  ADVERSARIAL_TRAJECTORY_GRAPHS_THESIS.pdf
  figures/
    original_concept_sketch.jpg
    atg_architecture.png
    atg_control_cycle.png
    atg_corridor.png
    *.dot
CITATION.cff
CHANGELOG.md
LICENSE.md
SHA256SUMS.txt
```

## Citation

Flynn, Sam. *Adversarial Trajectory Graphs: External Adversarial Supervision for Long-Horizon Autonomous AI*. Working Thesis v1.0, Dark Science Division, July 2026.

## Licensing

Copyright (c) 2026 Sam Flynn. Licensed under **CC BY-NC-ND 4.0** (Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International). The work may be shared in unmodified form with attribution; commercial use and derivatives require written permission. See [LICENSE.md](LICENSE.md).
