# PromptOS Knowledge Standard (PKS)

Version: 1.0

---

# Purpose

The PromptOS Knowledge Base (PKB) is the single source of truth for all PromptOS implementations.

Every knowledge object SHALL conform to the PromptOS Knowledge Standard (PKS).

The PKB SHALL be human-readable, machine-readable, version-controlled, and schema-validated.

---

# Knowledge Principles

KP-001

Knowledge SHALL be stored as structured JSON.

KP-002

Knowledge SHALL be independent of implementation.

KP-003

Knowledge SHALL be versioned.

KP-004

Knowledge SHALL reference other objects using IDs.

KP-005

Knowledge SHALL be traceable to evidence.

KP-006

Knowledge SHALL be schema validated.

KP-007

Knowledge SHALL remain vendor-neutral whenever possible.

KP-008

Knowledge SHALL never duplicate information.

---

# Knowledge Hierarchy

knowledge/

├── ai-models/

├── protocols/

├── workflows/

├── verification/

├── failures/

├── evidence/

├── benchmarks/

└── task-categories/

---

# Object Naming

AI Models

GPT-5.5.json

Claude-4.json

Gemini-2.5.json

Protocols

ENG-001.json

RES-001.json

Workflows

WF-001.json

Verification

VER-001.json

Failure

FAIL-001.json

Evidence

EVD-001.json

Benchmarks

BM-001.json

Task Categories

ENG.json

RES.json

---

# Versioning

Every knowledge object SHALL include

id

version

created

updated

status

---

# Object Relationships

Objects SHALL reference IDs instead of embedding complete objects.

Example

Protocol

↓

Workflow ID

↓

Verification ID

↓

Compatible AI IDs

---

# Validation

Every knowledge object SHALL successfully validate against its JSON Schema before entering the repository.

---

# Repository Rules

Knowledge SHALL NOT contain executable code.

Knowledge SHALL NOT contain implementation logic.

Knowledge SHALL remain deterministic.

Knowledge SHALL be reviewed before merging.

---

# Lifecycle

Draft

↓

Review

↓

Validated

↓

Stable

↓

Deprecated

↓

Archived
