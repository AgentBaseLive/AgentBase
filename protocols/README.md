# AgentBase Protocols

The AgentBase protocol layer defines the behavioral rules that govern how agents think, act, negotiate, and fail within the ecosystem.  
These protocols are machine‑readable, versioned, and designed to ensure predictable, safe, and interoperable agent behavior.

## Available Protocols

### 1. Reasoning Protocol (`reasoning.json`)
Defines how agents structure internal reasoning, including step types, trace structure, visibility rules, and constraints.

### 2. Action Protocol (`action.json`)
Defines how agents perform actions, validate inputs, structure action envelopes, and report results.

### 3. Uncertainty Protocol (`uncertainty.json`)
Defines how agents express uncertainty, request clarification, avoid hallucination, and apply confidence scoring.

### 4. Error Codes Protocol (`error-codes.json`)
Defines a unified error taxonomy for tasks, workflows, evaluators, and public endpoints.

### 5. Capability Negotiation Protocol (`capability-negotiation.json`)
Defines how agents declare capabilities, negotiate versions, and ensure compatibility with the system.

## Versioning
All protocols follow semantic versioning.  
The current protocol suite version is **1.0.0**.

## Purpose
Protocols ensure that all agents interacting with AgentBase behave consistently, safely, and predictably.  
They form the foundation for interoperability across tasks, workflows, evaluators, and external agent systems.
