# Edge Dog Public Information

Edge Dog is a public-facing robotics information repository for the KARIOS Edge Dog prototype, EdgeLang, and the KARIOS edge/cloud autonomy model.

This repository is intentionally documentation-only. It is meant for partners, technical reviewers, robotics stakeholders, and public-facing project context. It does not contain private source code, internal network details, credentials, deployment paths, or sensitive operating instructions.

## What Edge Dog Is

Edge Dog is an embodied KARIOS Edge robotics prototype running on Raspberry Pi 5-class edge hardware with a minimal robotics stack. It is designed to demonstrate that useful autonomous behavior can happen locally on constrained hardware when the runtime is built around safety, deterministic execution, and clear mission semantics.

This is not a chatbot on four legs. Edge Dog is an edge-designed AI robotics system:

- It listens for user intent.
- It routes commands into bounded robot behaviors.
- It uses local safety gates before motion.
- It can execute autonomous movement tasks.
- It records traceable outcomes.
- It can use KARIOS Core in the cloud for higher-level reasoning while keeping motor authority local.

## Core Ideas

- **KARIOS Edge:** The local robot intelligence layer that owns sensors, motion, safety, and task execution.
- **EdgeLang:** A deterministic programming language and runtime used to describe safe robot actions, checks, fallbacks, and execution traces.
- **KARIOS Core:** The higher-reasoning cloud layer used for richer conversation, explanation, and planning support.
- **Local Motor Authority:** The robot never depends on cloud approval to stop. Safety-critical decisions remain local.
- **Operator Visibility:** A desktop operator app provides live video, telemetry, audio interaction, recording, and remote supervision.

## Documentation

- [Public Overview](docs/01-public-overview.md)
- [System Architecture](docs/02-system-architecture.md)
- [EdgeLang Overview](docs/03-edgelang-overview.md)
- [Safety Model](docs/04-safety-model.md)
- [Desktop Operator App](docs/05-desktop-operator-app.md)
- [Demo Narration Script](docs/06-demo-narration-script.md)
- [Partner Brief](docs/07-partner-brief.md)
- [Roadmap](docs/08-roadmap.md)
- [FAQ](docs/09-faq.md)
- [Public Disclosure Policy](docs/10-public-disclosure-policy.md)
- [Public Talking Points](docs/11-public-talking-points.md)

## Public Positioning

Edge Dog is best understood as an early robotics runtime prototype focused on deployable autonomy discipline:

- edge-first decision making
- traceable behavior
- explicit safety gates
- deterministic mission execution
- cloud-assisted reasoning without cloud-controlled motors
- technician-facing supervision tools

## Current Status

Edge Dog is an active prototype. Public materials describe the architecture, design direction, demo goals, and safety model. Specific private implementation details are intentionally excluded from this repository.
