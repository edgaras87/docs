# 🧠 Knowledge Vault Structure

This vault is divided into **two major sections** — `cheatsheets/` and `concepts/`.

Each serves a different mindset:

- **Cheatsheets** → Quick practical reference. Short, actionable, syntax or API focused.  
  (Example: `Stream.map()` usage, `JPA annotations`, `MySQL setup for Java`)
- **Concepts** → Explanatory and theoretical. How and *why* something works.  
  (Example: `ORM concepts`, `HTTP lifecycle`, `Dependency Injection`)

Both are written in Markdown, interlinked with `[[WikiLinks]]`, and rendered via **MkDocs + Material**.

---

## 🗂 Folder Hierarchy Overview

```

docs/
│
├── README.md                 # This document
│
├── cheatsheets/              # Practical, code-focused notes
│   │
│   ├── languages/            # Syntax, language core, frameworks
│   │   ├── python/
│   │   │   ├── basics.md
│   │   │   ├── oop.md
│   │   │   └── frameworks/
│   │   │       ├── flask/
│   │   │       └── django/
│   │   └── java/
│   │       ├── core/
│   │       │   ├── collections.md
│   │       │   ├── streams.md
│   │       │   └── concurrency.md
│   │       └── frameworks/
│   │           ├── spring/
│   │           │   ├── rest-controller.md
│   │           │   ├── annotations.md
│   │           │   └── security.md
│   │           └── ...
│   │
│   ├── databases/            # DB-specific quick references
│   │   ├── sql/
│   │   │   ├── basics.md
│   │   │   ├── joins.md
│   │   │   └── performance.md
│   │   ├── mysql/
│   │   │   ├── setup/
│   │   │   │   ├── java.md
│   │   │   │   ├── python.md
│   │   │   │   └── docker.md
│   │   │   ├── queries.md
│   │   │   └── config.md
│   │   ├── orm/
│   │   │   ├── jpa-java-annotations.md
│   │   │   └── sqlalchemy-python-cheats.md
│   │   └── drivers/
│   │       ├── jdbc-java.md
│   │       └── psycopg-python.md
│   │
│   ├── networking/
│   │   ├── http/
│   │   │   ├── basics.md
│   │   │   ├── headers.md
│   │   │   └── status-codes.md
│   │   └── sockets/
│   │       └── tcp-vs-udp.md
│   │
│   └── tools/
│       ├── git.md
│       ├── docker.md
│       └── mkdocs.md
│
└── concepts/                 # Deep explanations and architecture-level notes
│
├── backend/
│   ├── rest-api.md
│   ├── http.md
│   ├── caching.md
│   └── authentication.md
│
├── databases/
│   ├── normalization.md
│   ├── indexing.md
│   ├── transactions-acid.md
│   └── orm/
│       ├── orm-concepts.md
│       └── jpa-vs-sqlalchemy.md
│
├── frameworks/
│   ├── spring-core.md
│   ├── hibernate.md
│   └── flask.md
│
├── design/
│   ├── mvc.md
│   ├── dependency-injection.md
│   ├── microservices.md
│   └── clean-architecture.md
│
└── general/
├── threading-models.md
├── error-handling.md
└── performance-tuning.md

```

---

## 📘 Conventions

**Naming**
- Use lowercase-with-hyphens for filenames (`rest-controller.md`, not `RestController.md`).
- Use descriptive names over generic ones (`sqlalchemy-python-cheats.md`, not `orm2.md`).
- Each folder can have its own `index.md` to serve as a landing page.

**Tags**
- Optionally tag pages for cross-searching:
  - `tags: [cheatsheet]`
  - `tags: [concept]`
- Combine tags for filters like `tag:cheatsheet path:mysql`.

**Links**
- Use Obsidian wikilinks: `[[cheatsheets/databases/orm/jpa-java-annotations]]`
- They’ll auto-convert to working links in MkDocs builds.

**Cross-linking**
- Cheatsheets should link “up” to related concepts:  
  `See [[concepts/databases/orm/orm-concepts]]`
- Concepts can link “down” to language implementations:  
  `Example: [[cheatsheets/databases/orm/sqlalchemy-python-cheats]]`

**Structure philosophy**
- Organize by **domain** first, **language** second.
- Avoid duplication — if knowledge spans languages (e.g., MySQL), keep it under one root and make subfolders per language/tool.
- Add new domains naturally (e.g. `frontend/`, `devops/`, `security/`) as your vault grows.

---

## 🚀 Purpose

This vault acts as a **personal developer wiki**:  
- A quick reference when coding (cheatsheets)  
- A deep knowledge archive for review and mastery (concepts)  
- A publishable site via MkDocs Material

Keep it consistent, cross-linked, and evolving.


