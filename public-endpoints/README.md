AgentBase Public Endpoints
This folder contains the public, machine‑native API surface for AgentBase.
Everything here is designed to be:
• 	JSON‑first
• 	schema‑driven
• 	stable and predictable
• 	easy for agents and humans to introspect
The goal is to provide a reference implementation that external agents can rely on when interacting with your platform.

📁 Files in this directory

The root descriptor for the public API surface.
It points to the full endpoint directory and declares the version of this reference implementation.

A machine‑readable index of all available public endpoints.
Each entry includes:
• 	description
• 	HTTP method
• 	path
• 	schema location
• 	example request/response files
This is the primary discovery surface for agents.

The JSON Schema defining the contract for the  endpoint.
Agents use this to validate their request payloads before sending them.

A minimal, valid example of how an agent calls the  endpoint.

A canonical example of the structured output returned by the endpoint.

🚀 The  Endpoint
The  endpoint is the core of the public API.
It allows external agents to:
• 	specify a task
• 	provide validated input
• 	receive structured output
This endpoint is intentionally simple and stable so that agents can integrate with minimal friction.

🧭 How agents should use this directory
1. 	Read  to locate the directory.
2. 	Load  to discover available endpoints.
3. 	Fetch the schema for the endpoint they want to call.
4. 	Validate their request against the schema.
5. 	Use the example files as guidance for formatting.
This mirrors how modern API ecosystems operate, but in a pure JSON, agent‑native form.

📌 Notes for implementers
• 	This directory is not a server implementation.
• 	It is a reference contract that any backend can implement.
• 	Additional endpoints can be added without breaking existing integrations.
