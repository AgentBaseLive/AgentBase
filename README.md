# AgentBase v3 — Reference Implementation

AgentBase is a lightweight, standards‑driven framework for building **agent‑native websites**.  
It provides a predictable, machine‑readable surface for agents to discover capabilities, execute tasks, run workflows, and exchange structured information.

This repository contains a complete reference implementation of an AgentBase‑compatible site, including:

- public endpoints  
- task definitions  
- workflow schemas and examples  
- protocol specifications  
- JSON Schemas  
- machine‑readable discovery surfaces  

Everything is designed to be stable, minimal, and easy for both humans and agents to navigate.

---

## 📁 Repository Structure

/ ├── public-endpoints/      # Machine-facing HTTP endpoints ├── tasks/                 # Task definitions (v1) ├── workflows/             # Workflow schemas and examples (v1) ├── workflows-v2/          # Advanced workflow examples (v2) ├── schemas/               # JSON Schemas for tasks, workflows, and protocols ├── protocols/             # AgentBase protocol specifications ├── examples/              # Example tasks, workflows, errors, and agent requests └── README.md              # This file


Each directory contains its own README and a machine‑readable `directory.json` index.

---

## 🚀 What AgentBase Provides

### **1. Discoverability**
Agents can discover capabilities through:

- `/public-endpoints/`
- `/protocols/`
- `/schemas/`
- `/examples/`
- `.well-known/agentbase.json` (optional)

### **2. Tasks**
Tasks are small, atomic operations with:

- strict input/output schemas  
- deterministic behavior  
- machine‑readable metadata  

Located in: `/tasks/`

### **3. Workflows**
Workflows combine tasks into multi‑step processes.

Two versions are supported:

#### **Workflow v1**
Simple, sequential workflows.  
Location: `/examples/workflows/`

#### **Workflow v2**
Advanced workflows using Execution Semantics v2:

- parallel execution  
- conditional guards  
- race semantics  
- fallback routing  
- dependency graphs  

Location: `/examples/workflows-v2/`

---

## 📚 Protocols

The `/protocols/` directory defines the core AgentBase protocols, including:

- **Task Protocol**  
- **Workflow Protocol**  
- **Execution Semantics v2**  
- **Agent Identity Protocol**  
- **Reputation & Telemetry (optional)**  

Each protocol is:

- versioned  
- machine‑readable  
- stable  
- JSON‑based  

---

## 🧩 JSON Schemas

All tasks, workflows, and protocols are validated using the schemas in `/schemas/`.

These schemas ensure:

- strict typing  
- predictable behavior  
- compatibility across agents  
- forward‑safe evolution  

---

## 🧪 Examples

The `/examples/` directory contains small, focused examples demonstrating:

- tasks  
- workflows (v1 and v2)  
- error patterns  
- agent request envelopes  

A machine‑readable index is available at:
