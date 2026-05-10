# Public Roadmap

This roadmap describes the public direction of Edge Dog without exposing private implementation details.

## Phase 1: Reliable Interaction

Goal: make Edge Dog reliably hear, respond, and explain its state.

Focus areas:

- wake phrase reliability
- clean voice turn-taking
- clear spoken responses
- rejection of background audio artifacts
- local status responses
- core handoff for higher-level questions

## Phase 2: Safe Motion Primitives

Goal: make basic movement reliable and explainable.

Focus areas:

- stand
- sit
- stop
- move forward
- turn left and right
- scan
- basic recovery from balance drift
- obstacle and timeout handling

## Phase 3: EdgeLang Mission Execution

Goal: make behavior scripts readable, deterministic, and traceable.

Focus areas:

- mission parsing
- validation diagnostics
- lowered execution plans
- runtime traces
- result objects
- blocked/fallback visibility

## Phase 4: Operator Supervision

Goal: make the system observable during operation.

Focus areas:

- live video
- telemetry
- motion state
- command input
- audio interaction
- recording
- demo support

## Phase 5: Autonomous Exploration

Goal: move from basic motion to structured local autonomy.

Focus areas:

- continuous exploration
- obstacle-aware movement
- environmental memory
- human-presence greeting
- conversational clarification
- guided learning from operator feedback

## Phase 6: Higher-Reasoning Coordination

Goal: use KARIOS Core for richer reasoning while preserving local safety.

Focus areas:

- cloud-assisted conversation
- planning support
- clarification questions
- knowledge lookup
- advisory-only action proposals
- local edge approval before execution
