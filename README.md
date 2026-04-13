# The Vault

A personal knowledge base for research and study in **Mathematical Optimization**, **Ordinary Differential Equations (ODEs)**, and **Partial Differential Equations (PDEs)**, built with [Obsidian](https://obsidian.md).

---

## Structure

```
The Vault/
├── 00_Home.md              # Dashboard — live overview of all notes
├── Optimization MOC.md     # Map of Content for Optimization
├── ODE MOC.md              # Map of Content for ODEs
├── PDE MOC.md              # Map of Content for PDEs
│
├── 01_Concepts/            # Definitions, mathematical objects, ideas
├── 02_Papers/              # Paper reviews and reading notes
├── 03_Projects/            # Open problems and research threads
├── 04_Foundations/         # Theorems, proofs, lecture notes
├── 05_Weekly/              # Weekly review notes
├── 06_Scratch/             # Drafts and temporary notes
│
└── _assets/
    ├── templates/          # Templater templates (see below)
    └── attachments/        # Images and files
```

### Folders

| Folder | Purpose |
|--------|---------|
| `01_Concepts/` | Core definitions and mathematical concepts — one note per object |
| `02_Papers/` | Structured reviews of research papers |
| `03_Projects/` | Open problems, research questions, ongoing threads |
| `04_Foundations/` | Theorems, lemmas, proofs, lecture notes |
| `05_Weekly/` | Weekly reflections and planning (auto-created each week) |
| `06_Scratch/` | Freeform scratch space — nothing here is permanent |

---

## Templates

All templates live in `_assets/templates/` and are powered by **Templater**.

| Template | Use for |
|----------|---------|
| `concept.md` | Mathematical definitions and objects |
| `theorem.md` | Theorems, lemmas, propositions, corollaries |
| `proof.md` | Standalone proof scratch space |
| `paper_review.md` | Structured paper reading notes |
| `problem.md` | Open research problems with attempt log |
| `lecture_note.md` | Course or seminar notes |
| `weekly.md` | Weekly review and planning |
| `moc.md` | Maps of Content for new topic areas |

New notes in each folder automatically apply the correct template via **Templater folder templates**.

---

## Plugins

| Plugin | Role |
|--------|------|
| [Templater](https://github.com/SilverStripe/obsidian-templater) | Template engine for all note types |
| [Dataview](https://github.com/blacksmithgu/obsidian-dataview) | Live queries in the dashboard and MOCs |
| [Latex Suite](https://github.com/artisticat1/obsidian-latex-suite) | ~90 math snippets (Greek, operators, Sobolev spaces, optimization) |
| [QuickAdd](https://github.com/chhoumann/quickadd) | Command-palette shortcuts for creating new notes |
| [Periodic Notes](https://github.com/liamcain/obsidian-periodic-notes) | Auto-generates weekly notes in `05_Weekly/` |
| [Calendar](https://github.com/liamcain/obsidian-calendar-plugin) | Calendar sidebar linked to weekly notes |
| [Tasks](https://github.com/obsidian-tasks-group/obsidian-tasks) | Task tracking across all notes |
| [Keep the Rhythm](https://github.com/rmkane/keep-the-rhythm) | Writing streak and activity heatmap |
| [Actions URI](https://github.com/czottmann/obsidian-actions-uri) | URI-based automation hooks |
| [Terminal](https://github.com/polyipseity/obsidian-terminal) | Embedded terminal inside Obsidian |

---

## Workflow

### Creating a new note

Use **QuickAdd** (`Ctrl+P` → type the command name):

| Command | Creates |
|---------|---------|
| `New Concept` | `01_Concepts/<name>.md` |
| `New Paper Review` | `02_Papers/<name>.md` |
| `New Theorem` | `04_Foundations/<name>.md` |
| `New Proof` | `04_Foundations/<name>.md` |
| `New Problem` | `03_Projects/<name>.md` |
| `New Lecture Note` | `04_Foundations/<name>.md` |
| `New Weekly Review` | `05_Weekly/YYYY-WWW.md` |

### LaTeX shortcuts

Snippets fire automatically inside math blocks. Examples:

| Type | Expands to |
|------|-----------|
| `alpha` | `\alpha` |
| `grad` | `\nabla` |
| `pd` | `\partial` |
| `pdt` | `\frac{\partial}{\partial t}` |
| `norm` | `\left\| \right\|` |
| `argmin` | `\operatorname*{arg\,min}_{...}` |
| `prox` | `\operatorname{prox}_{...}` |
| `Lp` | `L^{p}(\Omega)` |
| `Hs` | `H^{s}(\Omega)` |
| `RR` | `\mathbb{R}` |
| `//` | `\frac{...}{...}` |
| `ali` | `\begin{align*} \end{align*}` |

---

## Note Frontmatter

All notes use consistent YAML frontmatter for Dataview queries:

```yaml
---
type: concept | theorem | proof | paper-review | problem | lecture-note | weekly | moc
area: Optimization | ODEs | PDEs
topic: "specific subtopic"
status: draft | in-progress | done | open
date: YYYY-MM-DD
---
```

---

## Opening the Vault

1. Install [Obsidian](https://obsidian.md/download)
2. Clone this repository
3. Open Obsidian → **Open folder as vault** → select the cloned directory
4. Install community plugins when prompted (Settings → Community plugins → Check for updates)
5. Start from [[00_Home]] or one of the MOCs

---

## Research Areas

- **[Optimization MOC](./Optimization%20MOC.md)** — Convex analysis, duality, proximal algorithms, optimal control
- **[ODE MOC](./ODE%20MOC.md)** — Existence/uniqueness, stability, dynamical systems
- **[PDE MOC](./PDE%20MOC.md)** — Sobolev spaces, elliptic/parabolic/hyperbolic equations, variational methods
