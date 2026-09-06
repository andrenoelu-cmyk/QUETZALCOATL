````

---

# `docs/AI.md`

Este es todavía más importante porque aquí vamos a controlar **qué demonios puede hacer Ollama**.

```markdown
# QUETZALCOATL — AI Specification

## 1. Purpose

QUETZALCOATL uses a local Ollama model as its natural-language interpretation
and reasoning layer.

The AI exists to understand what the user wants and translate natural-language
requests into controlled operations supported by QUETZALCOATL.

The AI is not the system itself.

The AI does not own the computer.

The AI does not have unrestricted access to the operating system.

---

# 2. Core principle

QUETZALCOATL follows this principle:

> The AI interprets. The application decides. The tools execute.

Ollama may propose an action.

QUETZALCOATL Core determines whether that action is valid and permitted.

A tool performs the actual operation.

Conceptually:

```text
USER
  │
  ▼
OLLAMA
  │
  │ structured intent
  ▼
QUETZALCOATL CORE
  │
  ├── validate intent
  ├── validate parameters
  ├── validate permissions
  ├── request confirmation if required
  │
  ▼
TOOL
  │
  ▼
RESULT
  │
  ▼
OLLAMA / USER
````

```
READ
```

If it needs to modify a file:

```
WRITE
```

If an operation is dangerous:

```
NOT AVAILABLE
```

Do not grant broader permissions for convenience.

---

# 28. Version 0.1 scope

The AI layer only needs to support:

1. Natural-language task management.
2. Natural-language date interpretation.
3. File classification and organization proposals.
4. File renaming proposals.
5. Basic system/NAS queries.
6. Natural-language interpretation of system results.
7. Controlled tool calling.

The following are OUT OF SCOPE:

- autonomous agents;
- web browsing;
- email;
- WhatsApp;
- calendar synchronization;
- external AI APIs;
- long-term conversational memory;
- autonomous background actions;
- unrestricted shell access;
- advanced monitoring;
- complex workflow automation.

---

# 29. Final principle

QUETZALCOATL is not an AI with a computer.

It is a computer application that uses AI.

The AI is one component of the system, not the authority over it.

The architecture must preserve this distinction at all times.

```

### Una observación importante

Con estos dos documentos ya estamos fijando una decisión arquitectónica **muy buena**: SQLite y las herramientas del sistema son deterministas; Ollama queda como **capa de interpretación**. Eso significa que si mañana cambias de modelo —por ejemplo, de uno pequeño a uno mucho mejor— **QUETZALCOATL no debería necesitar ser reescrito**.

Y hay otra cosa que deliberadamente dejé fuera: **no he elegido todavía el framework de TUI, ORM, estructura exacta de Python ni modelo de Ollama**. Eso lo decidimos en `ARCHITECTURE.md`, porque todavía no conviene contaminar la especificación funcional con decisiones de implementación.
```
[[IDENTITY]]