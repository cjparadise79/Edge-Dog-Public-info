# Edge Dog Public Overview

Edge Dog is a KARIOS Edge robotics prototype built to demonstrate local autonomy on minimal hardware. It runs on Raspberry Pi 5-class edge compute and uses a lightweight robotics stack to connect voice interaction, local decision routing, motion control, sensors, safety checks, and operator visibility.

The purpose of Edge Dog is not to make a novelty robot that talks. The purpose is to show a disciplined robotics architecture where an AI system can operate at the edge, explain what it is doing, and remain safe even when higher-level cloud reasoning is unavailable.

## What Makes It Different

Many AI robotics demonstrations begin with conversation and then attach movement as an afterthought. Edge Dog is built the other way around:

- Local safety authority comes first.
- Motion commands are bounded and traceable.
- Sensor checks can stop or block unsafe behavior.
- Language is routed into deterministic robot actions.
- Cloud reasoning is advisory, not motor-authoritative.

This makes Edge Dog closer to an edge autonomy runtime than a chatbot with servos.

## Hardware Direction

The prototype is intentionally constrained:

- Raspberry Pi 5-class local compute
- minimal onboard robotics hardware
- local camera/video stream
- onboard audio input/output
- legged robot motion platform
- sensor feedback for range and balance
- technician-facing desktop supervision app

The constraint is part of the demonstration. If meaningful autonomy can run on minimal edge hardware, the architecture can scale up to more rugged platforms.

## Public Demo Goal

The public demo goal is simple:

1. Edge hears a spoken command.
2. Edge interprets the command locally.
3. Edge checks safety gates.
4. Edge performs a bounded action or autonomous behavior.
5. Edge explains what it is doing.
6. Edge streams video and telemetry to the operator app.
7. Edge can hand off higher-level questions to KARIOS Core.
8. Edge stops locally if told to stop or if safety requires it.

## Key Message

Edge Dog demonstrates a practical edge autonomy pattern:

> Local robot authority for safety and action. Cloud reasoning for deeper thought. Deterministic behavior language for traceable execution.
