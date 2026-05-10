# Safety Model

Edge Dog is designed around local safety authority. The robot should be able to stop, refuse, or fall back safely without depending on cloud reasoning.

## Core Safety Principle

> Cloud intelligence may advise, but local edge safety has final authority over motion.

This matters because legged robots operate near people, furniture, obstacles, and unpredictable surfaces. Safety decisions must remain close to the hardware.

## Safety Gates

The KARIOS Edge runtime is designed to gate motion through checks such as:

- calibration readiness
- motion bridge readiness
- obstacle/range checks
- balance and tilt feedback
- timeout limits
- stop command priority
- blocked-state reporting
- fallback behavior

## Motion Authority

Motion is treated as a controlled local task, not an open-ended text response.

Every useful motion primitive should have:

- a start condition
- a stop condition
- a timeout or bounded execution rule
- an interrupt path
- a result object
- a readable trace

## Safety Refusal

If Edge Dog cannot verify a safe condition, it should say so clearly and refuse or fall back.

Examples:

- "I cannot start exploration because motion is not ready."
- "I stopped because I detected unsafe tilt."
- "I stopped because an obstacle is too close."
- "I am already executing a motion task. Tell me to stop before starting another."

## Why This Is Partner-Relevant

Robotics stakeholders care less about spectacular claims and more about disciplined control. Edge Dog is intended to show that AI-driven robotics can be structured around:

- bounded execution
- explainable behavior
- hardware-aware preflight
- local safety authority
- traceable outcomes

That discipline is the foundation for more serious autonomy work.
