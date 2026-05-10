# Partner Brief

Edge Dog is a small-scale field autonomy prototype for demonstrating the KARIOS Edge architecture.

It is intended for technical stakeholders who care about deployable autonomy, ruggedized robotics systems, edge compute, explainable behavior, and safe local control.

## One-Sentence Positioning

Edge Dog demonstrates how KARIOS Edge can run local robot intelligence, EdgeLang can define deterministic safe behavior, and KARIOS Core can provide higher reasoning without taking direct motor authority away from the robot.

## What A Robotics Partner Should Notice

- The system is designed edge-first.
- Motion is treated as a local safety-critical task.
- Cloud reasoning is separated from motor authority.
- Behavior is structured through EdgeLang instead of raw natural language.
- The operator app provides live visibility.
- The demo is honest about being an early prototype.

## Why It Is Credible

Edge Dog focuses on the hard integration layers that matter in robotics:

- sensor feedback
- balance awareness
- obstacle response
- command routing
- safe motion primitives
- traceable execution
- operator supervision
- local/cloud role separation

The project does not claim that small hardware replaces larger robotics platforms. Instead, it shows how disciplined architecture can make constrained hardware useful and extensible.

## Current Demonstration Themes

- local voice command handling
- autonomous movement attempts
- safe stop and fallback
- live video to desktop app
- EdgeLang mission structure
- KARIOS Core handoff for higher-level reasoning
- public trace/explanation of decisions

## Partner Conversation Framing

The strongest way to present Edge Dog is:

> "This is early, but it is structured correctly. The robot keeps local safety authority, uses deterministic mission semantics through EdgeLang, exposes operator visibility, and can use cloud reasoning without making the cloud responsible for real-time motor safety."

## What This Can Grow Into

Edge Dog is a prototype path toward:

- field-agent style robot behavior
- autonomous inspection workflows
- mission scripts that are readable by humans
- edge/cloud robotics orchestration
- higher-level reasoning with local safety enforcement
- teachable robot behavior from guided interaction
