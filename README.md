# INCOSE Requirements Workbench

<div align="center">

![Version](https://img.shields.io/badge/version-2.0-blue)
![License](https://img.shields.io/badge/license-Free%20%26%20Open-green)
![INCOSE](https://img.shields.io/badge/INCOSE-GtWR%20v4-purple)
![Standard](https://img.shields.io/badge/ISO-29148%20%7C%2015288-orange)

**Write better requirements. Free forever.**

[🚀 Launch Tool](https://ssaleem74.github.io/incose-requirements-workbench/incose-workbench.html) · [📥 Example Project](https://ssaleem74.github.io/incose-requirements-workbench/test-case-shss.json) · [📄 Quick Reference PDF](https://ssaleem74.github.io/incose-requirements-workbench/quick-reference-card.pdf)

</div>

---

## 📋 Table of Contents

| Section | Description | Time |
|:--------|:------------|:----:|
| [Quick Start](#-quick-start) | Get running in 5 minutes | 5 min |
| [Interface Overview](#-interface-overview) | Learn the 7 views | 10 min |
| [Writing Requirements](#-writing-requirements) | Create quality requirements | 15 min |
| [Quality Analysis](#-quality-analysis) | Understand scores and rules | 10 min |
| [AI Improvement](#-ai-improvement) | Auto-fix violations | 5 min |
| [Traceability](#-traceability) | Build parent-child links | 10 min |
| [Export & Import](#-export--import) | DOORS, CSV, JSON | 5 min |
| [Best Practices](#-best-practices) | Tips from experts | 10 min |
| [INCOSE Rules Reference](#-incose-rules-reference) | All 42 rules | Reference |

---

## 🚀 Quick Start

> **⏱️ Time needed: 5 minutes**

### Step 1: Open the Tool

Go to **[ssaleem74.github.io/incose-requirements-workbench](https://ssaleem74.github.io/incose-requirements-workbench/)** and click **"Launch Workbench"**.

### Step 2: Start a New Project

Click **"+ Start New Project"** on the welcome screen.

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│                         [RE]                                   │
│               INCOSE Requirements Workbench                    │
│                                                                │
│     ┌──────────────────────────────────────────────────┐      │
│     │         ▶ Continue Previous Session              │      │
│     └──────────────────────────────────────────────────┘      │
│                                                                │
│     ┌──────────────────────────────────────────────────┐      │
│     │  ★        + Start New Project           ★        │ ◄────── Click here
│     └──────────────────────────────────────────────────┘      │
│                                                                │
│         📁 Drop a saved project file here to load             │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

### Step 3: Create Your First Requirement

Click **"+ New"** in the header, then type your requirement:

```
The system shall respond to user input within 500 ± 50 ms.
```

### Step 4: Check Your Quality Score

Look at the right panel — you should see **85%+ (Grade B or A)**.

### Step 5: Save Your Work

Click **"💾 Save Project"** — a JSON file downloads to your computer.

<details>
<summary>📺 <b>See it in action (diagram)</b></summary>

```
    ┌─────────────────────────────────────────────────────────────────────────┐
    │  [RE] INCOSE Requirements Workbench    [Dashboard][Author][Register]... │
    │                                                                         │
    │  ┌─[+ New]──────────────────────────────────────────[💾 Save Project]─┐ │
    │  │                                                                     │ │
    │  │  Requirement Statement                      │   Quality Score       │ │
    │  │  ┌───────────────────────────────────────┐  │   ┌─────────────┐    │ │
    │  │  │ The system shall respond to user      │  │   │     85      │    │ │
    │  │  │ input within 500 ± 50 ms.             │  │   │   Grade: B  │    │ │
    │  │  └───────────────────────────────────────┘  │   │  ✓38 ✕2 ⚠2  │    │ │
    │  │                                             │   └─────────────┘    │ │
    │  │  [Basic] [Conditional] [Performance]        │                       │ │
    │  │                                             │   Rule Analysis       │ │
    │  │  Attributes                                 │   ✓ R1 Structure      │ │
    │  │  ┌─────────┐ ┌─────────┐ ┌─────────┐       │   ✓ R2 Active Voice   │ │
    │  │  │Type: Fn │ │Level:Sys│ │Pri: Med │       │   ✕ R14 Punctuation   │ │
    │  │  └─────────┘ └─────────┘ └─────────┘       │   ...                  │ │
    │  └─────────────────────────────────────────────────────────────────────┘ │
    └─────────────────────────────────────────────────────────────────────────┘
```

</details>

---

## 🖥️ Interface Overview

The workbench has **7 views** accessible from the navigation bar:

```
┌──────────────────────────────────────────────────────────────────────────────┐
│  [RE]  │ [◉ Dashboard] [✎ Author] [☰ Register] [⊞ Trace] [✓ V&V] [⚙ Rules] [📖 Glossary] │
└──────────────────────────────────────────────────────────────────────────────┘
            ▲            ▲           ▲            ▲         ▲        ▲          ▲
            │            │           │            │         │        │          │
         Overview    Write/Edit   Table View   Traceability  V&V   42 Rules   Terms
```

### View Descriptions

| View | Icon | Purpose | When to Use |
|:-----|:----:|:--------|:------------|
| **Dashboard** | ◉ | Project overview, statistics, patterns | Starting point, check progress |
| **Author** | ✎ | Write and edit requirements | Main workspace |
| **Register** | ☰ | Table view with filtering | Review all requirements |
| **Trace** | ⊞ | Parent-child relationships | Build traceability |
| **V&V** | ✓ | Verification planning | Plan testing approach |
| **Rules** | ⚙ | INCOSE rules reference | Learn the 42 rules |
| **Glossary** | 📖 | Project dictionary | Define terms |

---

## ✍️ Writing Requirements

### The Editor View

When you click **"✎ Author"**, you see the main editing workspace:

```
┌─────────────────────────────────────────┬─────────────────────────┐
│                                         │                         │
│  ┌─ Requirement Tabs ─────────────────┐ │    QUALITY SCORE        │
│  │ [REQ-0001] [REQ-0002] [REQ-0003] + │ │    ┌─────────────┐      │
│  └────────────────────────────────────┘ │    │             │      │
│                                         │    │     92      │      │
│  ┌─ Editor Card ──────────────────────┐ │    │   Grade: A  │      │
│  │  REQ-0001        [Duplicate][Delete]│ │    │             │      │
│  │                                     │ │    └─────────────┘      │
│  │  Requirement Statement              │ │    ✓ 40  ✕ 0  ⚠ 2      │
│  │  ┌─────────────────────────────────┐│ │                         │
│  │  │                                 ││ │  ┌─ Rule Analysis ────┐ │
│  │  │  Type your requirement here...  ││ │  │ ✓ R1 Structure     │ │
│  │  │                                 ││ │  │ ✓ R2 Active Voice  │ │
│  │  └─────────────────────────────────┘│ │  │ ✓ R7 No Vague      │ │
│  │                                     │ │  │ ⚠ R4 Check Terms   │ │
│  │  Patterns: [Basic][Cond][Perf][Int] │ │  │ ...                │ │
│  └─────────────────────────────────────┘ │  └────────────────────┘ │
│                                         │                         │
│  ┌─ AI Improvement Panel (if needed) ──┐│                         │
│  │ ⚡ 3 violations detected            ││                         │
│  │           [⚡ AI IMPROVE NOW]       ││                         │
│  └─────────────────────────────────────┘│                         │
│                                         │                         │
│  ┌─ Attributes ────────────────────────┐│                         │
│  │ Type: [Functional    ▼]             ││                         │
│  │ Level: [System Req   ▼]             ││                         │
│  │ Priority: [Medium    ▼]             ││                         │
│  │ Parent: [STK-0001    ▼]             ││                         │
│  │ Rationale: [________________]       ││                         │
│  └─────────────────────────────────────┘│                         │
└─────────────────────────────────────────┴─────────────────────────┘
```

### Using Patterns

Patterns give you INCOSE-compliant templates. Click a pattern button to insert it:

| Pattern | Template | Best For |
|:--------|:---------|:---------|
| **Basic** | `The [entity] shall [action] [object].` | Simple statements |
| **Conditional** | `When [condition], the [entity] shall [action].` | Triggered behaviours |
| **Performance** | `The [entity] shall [action] within [X ± Y].` | Measurable targets |
| **Interface** | `The [entity] shall [send/receive] [data] via [interface].` | Data exchange |

> 💡 **Pro Tip:** Start with a pattern, then customize it. This ensures good structure from the beginning.

### Example: Writing a Good Requirement

<table>
<tr>
<td width="50%">

**❌ Bad Requirement**
```
The system should be fast and reliable.
```

**Problems:**
- ❌ "should" instead of "shall"
- ❌ "fast" is vague (R7)
- ❌ "reliable" is vague (R7)
- ❌ No measurable criteria (R34)
- ❌ Missing period (R14)

**Score: 35% (Grade F)**

</td>
<td width="50%">

**✅ Good Requirement**
```
The Data_Processor shall process each 
sensor input within 200 ± 20 ms with 
MTBF ≥ 5000 hours.
```

**Why it's good:**
- ✅ Uses "shall"
- ✅ Specific entity name
- ✅ Measurable timing with tolerance
- ✅ Measurable reliability
- ✅ Ends with period

**Score: 94% (Grade A)**

</td>
</tr>
</table>

---

## 📊 Quality Analysis

### Understanding Your Score

The quality score is calculated by checking your requirement against **42 INCOSE rules**:

```
                    ┌─────────────────┐
                    │                 │
                    │       85        │ ◄─── Score (0-100%)
                    │    Grade: B+    │ ◄─── Letter grade
                    │                 │
                    │   ✓ 38  ✕ 2  ⚠ 2│ ◄─── Passed, Failed, Warnings
                    │                 │
                    └─────────────────┘
```

### Grade Scale

| Grade | Score | Meaning | Action |
|:-----:|:-----:|:--------|:-------|
| **A+ / A** | 90%+ | Excellent | ✅ Ready for review |
| **B+ / B** | 80-89% | Good | Minor improvements possible |
| **C+ / C** | 70-79% | Acceptable | Review failed rules |
| **D** | 60-69% | Needs Work | Use AI Improvement |
| **F** | <60% | Poor | Significant rewriting needed |

> 🎯 **Target:** Aim for **80% or higher (Grade B)** on all requirements before formal review.

### Rule Categories

The 42 rules are organized into **14 categories**:

```
┌──────────────────────────────────────────────────────────────────┐
│                        42 INCOSE RULES                           │
├──────────────┬──────────────┬──────────────┬────────────────────┤
│ Accuracy     │ Concision    │ Non-Ambiguity│ Singularity        │
│ R1-R9        │ R10-R11      │ R12-R17      │ R18-R23            │
│ ████████░░   │ ██░░░░░░░░   │ ██████░░░░   │ ██████░░░░         │
├──────────────┼──────────────┼──────────────┼────────────────────┤
│ Completeness │ Realism      │ Conditions   │ Uniqueness         │
│ R24-R25      │ R26          │ R27-R28      │ R29-R30            │
│ ██░░░░░░░░   │ █░░░░░░░░░   │ ██░░░░░░░░   │ ██░░░░░░░░         │
├──────────────┼──────────────┼──────────────┼────────────────────┤
│ Abstraction  │ Quantifiers  │ Tolerance    │ Quantification     │
│ R31          │ R32          │ R33          │ R34-R35            │
│ █░░░░░░░░░   │ █░░░░░░░░░   │ █░░░░░░░░░   │ ██░░░░░░░░         │
├──────────────┴──────────────┼──────────────┴────────────────────┤
│ Uniformity   R36-R40        │ Modularity   R41-R42              │
│ █████░░░░░                  │ ██░░░░░░░░                        │
└─────────────────────────────┴───────────────────────────────────┘
```

---

## ⚡ AI Improvement

When your requirement has quality issues, a purple panel appears:

```
┌─────────────────────────────────────────────────────────────────┐
│  ⚡ AI Requirement Improver                                      │
│                                                                 │
│  4 INCOSE violations detected — AI can fix: R2, R7, R8, R10    │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │               ⚡ AI IMPROVE NOW                           │  │ ◄─── Click this!
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
│  [R7: Vague "fast"] [R8: Escape clause] [R10: "be able to"]    │
└─────────────────────────────────────────────────────────────────┘
```

### What AI Fixes

| Rule | Before | After |
|:-----|:-------|:------|
| R2 Passive | "shall be processed" | "shall process" |
| R7 Vague | "fast" | "within [X] seconds" |
| R7 Vague | "reliable" | "with MTBF ≥ [X] hours" |
| R8 Escape | "where possible" | "[specify condition]" |
| R10 Superfluous | "shall be able to" | "shall" |
| R14 Punctuation | (missing period) | Adds "." |
| R26 Absolutes | "always" | "in each operational scenario" |
| R35 Temporal | "immediately" | "within [X] ms" |

> ⚠️ **Important:** AI uses `[X]` placeholders where you need to fill in actual values.

### Before & After Example

```
BEFORE (Score: 32%)                      AFTER (Score: 89%)
┌────────────────────────────┐          ┌────────────────────────────┐
│ The system should be able  │          │ The system shall process   │
│ to process data quickly    │   ──►    │ data within [X] seconds    │
│ and reliably, where        │          │ with MTBF ≥ [X] hours.     │
│ possible.                  │          │                            │
└────────────────────────────┘          └────────────────────────────┘

Fill in the [X] values:
┌────────────────────────────┐
│ The system shall process   │
│ data within 200 seconds    │  Score: 94% ✓
│ with MTBF ≥ 5000 hours.    │
└────────────────────────────┘
```

---

## 🔗 Traceability

### Why Traceability Matters

Traceability links requirements across levels:

```
    Stakeholder Need         "Users need to monitor their home remotely"
           │
           ▼
    System Requirement       "System shall provide mobile app for iOS/Android"
           │
           ▼
    Subsystem Requirement    "Mobile_App shall display status within 2 seconds"
           │
           ▼
    Component Requirement    "Display_Module shall refresh at ≥ 30 Hz"
```

### The Trace View

Click **"⊞ Trace"** to see the traceability matrix:

```
┌─ Stakeholder Need (4) ─────────────────────────────────────────────────────┐
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐   │
│  │  STK-0001    │  │  STK-0002    │  │  STK-0003    │  │  STK-0004    │   │
│  │  95% A       │  │  92% A       │  │  88% B+      │  │  90% A       │   │
│  │  ↓ SYS-0003  │  │  ↓ SYS-0001  │  │  ↓ SYS-0005  │  │  ↓ SYS-0004  │   │
│  │    SYS-0006  │  │    SYS-0002  │  │    SYS-0006  │  │    SYS-0008  │   │
│  └──────────────┘  └──────────────┘  └──────────────┘  └──────────────┘   │
└────────────────────────────────────────────────────────────────────────────┘

┌─ System Requirement (8) ───────────────────────────────────────────────────┐
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐                     │
│  │  SYS-0001    │  │  SYS-0002    │  │  SYS-0003    │  ...                │
│  │  88% B+      │  │  92% A       │  │  85% B       │                     │
│  │  ↑ STK-0002  │  │  ↑ STK-0002  │  │  ↑ STK-0001  │  ◄── Parent link   │
│  │  ↓ SUB-0001  │  │  ↓ SUB-0003  │  │  ↓ SUB-0005  │  ◄── Child links   │
│  │    SUB-0002  │  │    SUB-0004  │  │    SUB-0006  │                     │
│  └──────────────┘  └──────────────┘  └──────────────┘                     │
└────────────────────────────────────────────────────────────────────────────┘

┌─ ⚠️ Orphan Requirements (2) ───────────────────────────────────────────────┐
│  These requirements have no parent — add traces or review their level:     │
│  [ORPH-0001] [ORPH-0002]                                                   │
└────────────────────────────────────────────────────────────────────────────┘
```

### Setting Up Traces

1. Open a requirement in the **Author** view
2. Find the **Parent** dropdown in Attributes
3. Select the higher-level requirement it derives from

```
┌─ Attributes ───────────────────────────────────────────┐
│                                                        │
│  Parent: [ Select parent requirement    ▼]             │
│          ┌─────────────────────────────────────────┐   │
│          │ (None)                                  │   │
│          │ STK-0001 — Users need to...            │   │
│          │ STK-0002 — System shall detect...      │ ◄── Select this
│          │ STK-0003 — System shall operate...     │   │
│          │ STK-0004 — System shall protect...     │   │
│          └─────────────────────────────────────────┘   │
└────────────────────────────────────────────────────────┘
```

---

## 📤 Export & Import

### Saving Your Project

| Method | Format | Use For |
|:-------|:-------|:--------|
| **💾 Save Project** | JSON | Backup, continue later, share with colleagues |
| **↓ Export > CSV** | CSV | Excel, Google Sheets, reports |
| **↓ Export > ReqIF** | XML | IBM DOORS, DOORS NG, Polarion |

### Export Button Location

```
┌────────────────────────────────────────────────────────────────────────────┐
│  [RE] INCOSE Requirements Workbench                                        │
│                                                                            │
│  [◉ Dashboard] [✎ Author] [☰ Register] ...                                │
│                                                                            │
│                    [+ New] [💾 Save Project] [📂 Load] [↓ Export ▾] [⚡]   │
│                                                         │                  │
│                                              ┌──────────┴─────────┐        │
│                                              │ CSV Spreadsheet    │        │
│                                              │ ReqIF (DOORS)      │        │
│                                              │ JSON Archive       │        │
│                                              │ ─────────────────  │        │
│                                              │ ↑ Import Document  │        │
│                                              └────────────────────┘        │
└────────────────────────────────────────────────────────────────────────────┘
```

### Importing from Documents

If you have requirements in a Word document or text file:

1. Click **"↓ Export ▾"** → **"↑ Import Document"**
2. Paste your text
3. Click **"Import Requirements"**

The parser extracts all lines containing "shall" and auto-classifies them.

```
┌─ Import from Document ──────────────────────────────────────────────────────┐
│                                                                             │
│  Paste document text. All lines containing 'shall' will be extracted.       │
│                                                                             │
│  ┌─────────────────────────────────────────────────────────────────────┐   │
│  │ REQ-001: The system shall process data within 500 ms.               │   │
│  │ 3.2.1 The subsystem shall interface via RS-422.                     │   │
│  │ • The component shall weigh less than 100 g.                        │   │
│  └─────────────────────────────────────────────────────────────────────┘   │
│                                                                             │
│  3 'shall' statements detected                    [Cancel] [Import ✓]      │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 💡 Best Practices

### ✅ DO

| Practice | Example |
|:---------|:--------|
| Start with entity name | `The Navigation_Module shall...` |
| Use "shall" for obligations | `shall process` (not "should", "will", "must") |
| Be specific and measurable | `within 100 ± 10 ms` |
| One thought per requirement | Split compound statements |
| Use active voice | `shall process` (not "shall be processed") |
| End with a period | `...within 5 seconds.` |
| Add tolerances | `12 ± 1 m` (not just "12 m") |
| Use defined terms | Add entities to the Glossary |

### ❌ DON'T

| Avoid | Why | Fix |
|:------|:----|:----|
| Vague terms: "fast", "reliable" | Not measurable | Use numbers: "within 100 ms" |
| Escape clauses: "where possible" | Creates loopholes | Make explicit or remove |
| Absolutes: "always", "never", "100%" | Unrealistic | Use "≥ 99.9%", "in each scenario" |
| Pronouns: "it", "they", "this" | Ambiguous | Use entity names |
| Implementation: "MySQL", "Python" | Solution-specific | Describe what, not how |
| Purpose phrases: "in order to" | Belongs in rationale | Move to rationale field |
| Passive voice: "shall be processed" | Unclear responsibility | Use active voice |

### Workflow Diagram

```
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│   START     │    │   AUTHOR    │    │   ANALYZE   │    │   TRACE     │
│             │───►│             │───►│             │───►│             │
│ Stakeholder │    │ Write reqs  │    │ Check score │    │ Link parent │
│ Needs       │    │ Use patterns│    │ Fix issues  │    │ Find orphans│
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
                                             │
                                             ▼
┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│   EXPORT    │    │   REVIEW    │    │   IMPROVE   │
│             │◄───│             │◄───│             │
│ Save JSON   │    │ All ≥ 80%?  │    │ AI Improve  │
│ Export CSV  │    │ Check trace │    │ Bulk fix    │
│ Export DOORS│    │             │    │             │
└─────────────┘    └─────────────┘    └─────────────┘
```

---

## 📚 INCOSE Rules Reference

<details>
<summary><b>Accuracy Rules (R1-R9)</b></summary>

| Rule | Name | Description |
|:-----|:-----|:------------|
| R1 | Structured Statements | Use agreed patterns (When/If/The + shall) |
| R2 | Active Voice | Avoid passive voice ("shall be Xed") |
| R3 | Subject-Verb | Subject should be the system, not users |
| R4 | Defined Terms | All terms should be in glossary |
| R5 | Definite Articles | Use "the" not "a/an" for specific entities |
| R6 | Units of Measure | Include units with all numbers |
| R7 | Vague Terms | Avoid: fast, reliable, user-friendly, etc. |
| R8 | Escape Clauses | Avoid: where possible, as appropriate |
| R9 | Open-Ended | Avoid: etc., including but not limited to |

</details>

<details>
<summary><b>Concision Rules (R10-R11)</b></summary>

| Rule | Name | Description |
|:-----|:-----|:------------|
| R10 | Superfluous Infinitives | Avoid: "shall be able to", "shall be capable of" |
| R11 | Separate Clauses | Keep conditions and actions distinct |

</details>

<details>
<summary><b>Non-Ambiguity Rules (R12-R17)</b></summary>

| Rule | Name | Description |
|:-----|:-----|:------------|
| R12 | Grammar | Use correct grammar |
| R13 | Spelling | Use correct spelling |
| R14 | Punctuation | End with period, use proper punctuation |
| R15 | Logical Expressions | Use [X AND Y] or [X OR Y] notation |
| R16 | Use of "Not" | Avoid negatives, write positively |
| R17 | Oblique "/" | Avoid "/", use "and" or "or" |

</details>

<details>
<summary><b>Singularity Rules (R18-R23)</b></summary>

| Rule | Name | Description |
|:-----|:-----|:------------|
| R18 | Single Thought | One "shall" per requirement |
| R19 | Combinators | Avoid: and shall, or shall, however |
| R20 | Purpose Phrases | Move "in order to" to rationale |
| R21 | Parentheses | Avoid long parenthetical text |
| R22 | Enumeration | List items explicitly |
| R23 | Diagrams | Reference diagrams where helpful |

</details>

<details>
<summary><b>Other Rules (R24-R42)</b></summary>

| Rule | Name | Description |
|:-----|:-----|:------------|
| R24 | Pronouns | Avoid: it, they, this, that |
| R25 | Headings | Requirements should be self-contained |
| R26 | Absolutes | Avoid: always, never, 100%, all |
| R27 | Explicit Conditions | State conditions clearly |
| R28 | Multiple Conditions | Use AND/OR for multiple conditions |
| R29 | Classification | Classify by type |
| R30 | Unique Expression | No duplicate requirements |
| R31 | Solution Free | Describe what, not how |
| R32 | Quantifiers | Use "each" not "all/any/every" |
| R33 | Tolerances | Specify ranges (± X) |
| R34 | Measurable | Include measurable criteria |
| R35 | Temporal | Avoid vague timing words |
| R36-40 | Uniformity | Consistent terms, style, format |
| R41-42 | Modularity | Group related requirements |

</details>

---

## 📥 Downloads

| Resource | Description |
|:---------|:------------|
| [🚀 Launch Tool](https://ssaleem74.github.io/incose-requirements-workbench/incose-workbench.html) | Open the workbench |
| [📥 Example Project (JSON)](https://ssaleem74.github.io/incose-requirements-workbench/test-case-shss.json) | Smart Home Security System with 30 requirements |
| [📄 Quick Reference Card (PDF)](https://ssaleem74.github.io/incose-requirements-workbench/quick-reference-card.pdf) | Printable A3 cheat sheet |
| [🧪 Test Plan](TEST-PLAN.md) | QA test procedures |

---

## ❓ FAQ

<details>
<summary><b>Does this tool use real AI like ChatGPT?</b></summary>

No. The "AI Improvement" feature uses rule-based pattern matching, not a large language model. This means:
- ✅ Works 100% offline
- ✅ Your data stays private
- ✅ No API costs
- ⚠️ Limited to known patterns (can't rewrite complex sentences)

</details>

<details>
<summary><b>Where is my data stored?</b></summary>

**Your data never leaves your computer.** The tool runs entirely in your browser:
- No server, no database, no cloud
- Auto-save uses browser localStorage (temporary)
- Permanent saves go to JSON files on your machine

</details>

<details>
<summary><b>Can I use this for commercial projects?</b></summary>

Yes! The tool is free for any use — personal, academic, or commercial.

</details>

<details>
<summary><b>How do I import into IBM DOORS?</b></summary>

1. Export your project as **ReqIF (DOORS)**
2. In DOORS: File → Import → ReqIF
3. Select the .reqif file
4. Map attributes as needed

</details>

---

## 🙏 Credits

- **INCOSE** for the Guide to Writing Requirements v4
- **ISO/IEC/IEEE** for standards 29148 and 15288
- **OMG** for the ReqIF specification

---

<div align="center">

**Built for systems engineers, by systems engineers.**

[🚀 Launch Tool](https://ssaleem74.github.io/incose-requirements-workbench/incose-workbench.html) · [Report Issue](https://github.com/ssaleem74/incose-requirements-workbench/issues)

</div>
