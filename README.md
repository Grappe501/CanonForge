# CanonForge

> Institutional knowledge system for **CHRONOFORGE** — the recursive adventure novel project.
> Codename: CHRONOFORGE · Repo: `Grappe501/CanonForge` · Local truth: `H:\CanonForge`

**Version:** see [VERSION](VERSION) · **CanonForge:** 1.7.0 · **BUILD-019:** v1.0 · **Concepts:** 430

---

## What this is

CanonForge is the **Knowledge OS** and live instance of the **Composer's Blueprint** — the machine that produces CHRONOFORGE, not documentation about the story.

```txt
knowledge/     ← raw entries + concept registry (institutional memory)
canon/         ← derived constitution (locked principles only)
architecture/  ← how the book will be built (Story Engine, phases, locks)
ingest/        ← machine-readable manifest for retrieval automation
```

**Phase 14 prose is explicitly out of scope until directives arrive.**

---

## Quick retrieval

| Question | Go to |
|---|---|
| What is the BUILD layer? | [canon/build/BUILD_INDEX.md](canon/build/BUILD_INDEX.md) |
| What is the roadmap? | [architecture/MASTER_BUILD_ROADMAP.md](architecture/MASTER_BUILD_ROADMAP.md) |
| What is the law? | [canon/CONSTITUTION.md](canon/CONSTITUTION.md) |
| What is the First Law? | [canon/RULE_BOOK.md](canon/RULE_BOOK.md) |
| What concepts exist? | [knowledge/CONCEPT_REGISTRY.md](knowledge/CONCEPT_REGISTRY.md) |
| What's still undecided? | [knowledge/OPEN_QUESTIONS.md](knowledge/OPEN_QUESTIONS.md) |
| Where did an idea come from? | [knowledge/INGEST_INDEX.md](knowledge/INGEST_INDEX.md) → `entries/` |
| What did we lock today? | [knowledge/DECISION_LOG.md](knowledge/DECISION_LOG.md) |
| What is the build system? | [architecture/COMPOSERS_BLUEPRINT.md](architecture/COMPOSERS_BLUEPRINT.md) |
| What is the production workflow? | [architecture/PRODUCTION_PHILOSOPHY.md](architecture/PRODUCTION_PHILOSOPHY.md) |
| What is the master score? | [architecture/THE_SCORE.md](architecture/THE_SCORE.md) |
| What is the typographic language? | [architecture/VISUAL_GRAMMAR.md](architecture/VISUAL_GRAMMAR.md) |
| How is the book scored? | [architecture/RHYTHM_BIBLE.md](architecture/RHYTHM_BIBLE.md) |
| How will the book be built? | [architecture/WATCHMAKER_PHASES.md](architecture/WATCHMAKER_PHASES.md) |

---

## Ingest model

1. **Layer 1 — Raw entries** (`knowledge/entries/`): verbatim upload text, never overwritten
2. **Layer 2 — Concept Registry**: stable IDs, categories, locked/open status
3. **Layer 3 — Derived canon** (`canon/`): synthesized principles, conflicts resolved via Decision Log
4. **Layer 4 — Retrieval** (`INGEST_INDEX.md` + `ingest/manifest.json`)

Future uploads append new numbered entries and bump [VERSION](VERSION).

---

## Governance

| Rule | Detail |
|---|---|
| **Local truth** | `H:\CanonForge` only |
| **Remote backup** | Private GitHub — audit trail, not public surface |
| **Commit cadence** | One logical step → one commit → push |
| **Security** | Private until author opens; no secrets in repo |
| **Prose gate** | No `manuscript/` until Phase 14 |

---

## Directory map

```
H:\CanonForge\
├── README.md                 ← you are here
├── VERSION · CHANGELOG.md
├── canon/                    ← MASTER_CANON · RULE_BOOK · BOOK_OF_SECRETS
├── knowledge/                ← entries · registry · glossary · decisions
├── architecture/             ← Story Engine · phases · validation
├── ingest/                   ← manifest.json · concepts.json · schema.json
└── BUILD_LOG/                ← step-by-step build trace
```

---

## Adding a new upload

1. Append entry to `knowledge/entries/NNN-slug.md` with header metadata
2. Register new concepts in `CONCEPT_REGISTRY.md` and `ingest/concepts.json`
3. Update `INGEST_INDEX.md`, `manifest.json`, bump `VERSION`, log in `CHANGELOG.md`
4. Commit and push

---

*Built 2026-07-05 · BUILD-019 v1.0 · 57 entries · 430 concepts*
