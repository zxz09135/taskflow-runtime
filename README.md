# Async Task Network (ATN)

A lightweight async execution system designed to handle complex tasks through state-driven task units and dynamic capability routing.

---

## 🚀 Overview

This project explores a different approach to AI-driven automation:

Instead of relying on fixed agents, tasks are decomposed into independent **Task Units**, each carrying its own state and execution context.

The system dynamically routes each unit to available capabilities (e.g., code generation, error analysis, patching), enabling:

- incremental execution
- localized retries
- adaptive task flow

---

## 🧩 Core Concepts

### Task Unit
A minimal execution block with:
- unique id
- state (pending / running / blocked / resolved)
- context snapshot

### Capability Routing
Execution is not role-based.  
Each task unit is dispatched to a capability:

- `code-gen`
- `error-detect`
- `patch-apply`
- `result-check`
- `data-clean`

---

### State Transitions


