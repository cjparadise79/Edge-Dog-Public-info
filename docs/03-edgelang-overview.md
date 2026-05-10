# EdgeLang Overview

EdgeLang is the deterministic programming language and runtime used by KARIOS Edge to describe robot actions in a safety-aware way.

The goal of EdgeLang is not to replace general-purpose programming languages. The goal is to give embodied AI systems a small, readable layer for mission intent, safety gates, action sequencing, fallback behavior, and traceable execution.

## Why EdgeLang Exists

Natural language is powerful, but it is not precise enough to directly control a robot. A robot needs clear execution semantics:

- What action is being requested?
- What must be true before it starts?
- What should stop it?
- What happens if a sensor blocks the action?
- What trace should be emitted?
- What result should be returned?

EdgeLang provides this structure.

## What EdgeLang Does

EdgeLang can describe:

- missions
- context checks
- sensor gates
- movement primitives
- wait and scan steps
- fallback behavior
- blocked execution
- result summaries
- readable traces

In the Edge Dog prototype, EdgeLang is used to make robot behavior explainable and bounded instead of open-ended and fragile.

## Example Mission Flow

An EdgeLang-style behavior can be described publicly as a simple mission flow:

- confirm the robot is ready
- confirm motion is calibrated
- watch for obstacles
- stand before moving
- move forward until stopped or blocked
- turn away from obstacles when safe
- fall back to stop when uncertain
- emit a trace and result summary

## Why It Matters On Minimal Hardware

On small edge hardware, heavy reasoning loops can be slow or unreliable. EdgeLang helps by making the robot's immediate behavior deterministic:

- The robot does not need a large model to know how to stop.
- The robot does not need cloud access to enforce safety.
- The robot can emit readable traces from a small runtime.
- The robot can separate "thinking" from "acting."

## Relationship To KARIOS Core

KARIOS Core can help interpret broad user intent or answer higher-level questions. EdgeLang turns approved local behavior into a structured mission that the edge runtime can execute safely.

In short:

- KARIOS Core can help reason.
- KARIOS Edge decides what is safe.
- EdgeLang defines how safe behavior executes.
