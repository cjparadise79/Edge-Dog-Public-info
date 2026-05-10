# FAQ

## Is Edge Dog just a chatbot on a robot platform?

No. Edge Dog is designed as an edge autonomy runtime. Conversation is one interface, but the core focus is local decision routing, safety gates, motion control, sensor feedback, traceable execution, and operator supervision.

## Why use Raspberry Pi 5-class hardware?

The prototype intentionally runs on constrained edge hardware to prove that the architecture does not require a large server to perform every local behavior. Larger systems can be added later, but safety-critical robot authority should remain close to the hardware.

## What is EdgeLang?

EdgeLang is a deterministic mission and behavior language for KARIOS Edge. It helps define what a robot should check, do, stop, refuse, or report during a mission.

## What does KARIOS Core do?

KARIOS Core is the higher-reasoning cloud layer. It can help with conversation, broad knowledge, planning support, and clarification. It does not directly control motors.

## Why keep motor authority local?

Physical robots need fast and reliable safety decisions. If the network fails or cloud reasoning is uncertain, the robot still needs to stop safely.

## What does the desktop app do?

The desktop operator app provides live video, telemetry, command input, recording, and supervision so a technician can observe what the robot is doing.

## Is Edge Dog finished?

No. Edge Dog is an active prototype. Public materials describe the architecture, demo direction, safety model, and intended development path.

## Does this public repository include source code?

No. This repository is for public documentation only.
