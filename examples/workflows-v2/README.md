# Workflow Examples (v2)

This directory contains examples demonstrating the advanced execution features introduced in **Workflow Schema v2** and **Execution Semantics v2**.  
Each file is a small, self‑contained workflow illustrating one capability at a time.

## Included Examples

### `parallel.json`
Shows how multiple steps can run at the same time when they have no dependency relationship.

### `conditional.json`
Demonstrates guard‑based execution, where steps only run if a boolean expression evaluates to true.

### `race.json`
Illustrates race semantics: multiple steps run concurrently and the workflow continues as soon as one completes.

### `fallback.json`
Shows how to route execution to a fallback step when a primary step fails.

### `dependencies.json`
Demonstrates explicit dependency graphs (DAGs), including fan‑out and fan‑in patterns.

## Purpose

These examples are designed to be:

- **minimal** — each file focuses on one concept  
- **schema‑valid** — fully compatible with Workflow Schema v2  
- **safe** — small enough to inspect, diff, and extend  
- **illustrative** — showing how to combine tasks, state, and execution modes  

Use these as reference patterns when building more complex workflows.
