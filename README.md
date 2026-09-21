# SeaFlow

**Public informational entry point for the SeaFlow project.**

SeaFlow is a research-oriented evidence runtime designed to coordinate
traceable legal, textual and tabular evidence workflows. Its aim is that every
statement a consumer can act on is backed by evidence that can be re-checked
against the artifact it came from — and that anything which cannot be
established is reported as loss, ambiguity or refusal rather than guessed.

This repository is **documentation only**. It contains no runtime code.

---

## Repository map

| Repository | What it is | Access |
| --- | --- | --- |
| **SeaFlow** (this repository) | Public informational entry point | Public |
| [**ShanHai**](https://github.com/HuDeyi-66/Shan_Hai_Code_Skill) | Legal-text evidence Skill | Public, open source |
| [**LuoHai**](https://github.com/HuDeyi-66/Luo_Hai_Tables_Skill) | Tabular evidence Skill | Public, open source |
| SeaFlow base runtime | Core runtime and application integration | Private |

---

## The two public Skills

ShanHai and LuoHai are **independent open-source components**, and this is the
most important thing on this page:

> ShanHai and LuoHai are independently usable open-source components. SeaFlow
> can integrate them as official Skills, but neither project requires the SeaFlow
> runtime for standalone use.

Each one can be cloned, installed, invoked, tested and integrated into other
software entirely on its own terms. Neither imports the SeaFlow base, and
neither needs it present in any form.

**ShanHai — legal and textual evidence**
[github.com/HuDeyi-66/Shan_Hai_Code_Skill](https://github.com/HuDeyi-66/Shan_Hai_Code_Skill)

Reads UTF-8 legal text, detects legal structure, and emits evidence units with
exact character, byte and line spans. It reconstructs citations that can be
re-checked against the artifact, and reports structural problems — an empty
document, a missing or malformed article marker, a numbering gap, a duplicated
marker, an encoding failure — as distinct, inspectable outcomes. Where a
location is ambiguous it returns every candidate and selects none.

**LuoHai — structured and tabular evidence**
[github.com/HuDeyi-66/Luo_Hai_Tables_Skill](https://github.com/HuDeyi-66/Luo_Hai_Tables_Skill)

Reads OOXML workbooks with the standard library, detects table regions, and
records worksheet and table context. It emits cell and range evidence, keeps
raw and rendered values distinct, and compares declared table metadata against
what was actually observed instead of treating either as authoritative.
Ambiguity and loss are reported, never resolved by first match.

When SeaFlow **is** available, the two Skills operate as its official
Skills/plugins. That integration is implemented inside SeaFlow, which adapts the
Skills' public interfaces; the Skills themselves carry no SeaFlow dependency.

---

## The SeaFlow base runtime

**The SeaFlow base runtime is currently maintained in a private repository and
is not part of the public distribution.** This repository serves as the public
informational entry point for the project.

At a high level, the base is responsible for coordinating evidence workflows
across independent components. Its responsibilities include:

* **Evidence and runtime coordination** — sequencing a request end to end and
  keeping the result inspectable at every step.
* **Source and artifact handling** — registering sources and artifacts, and
  verifying artifact integrity before anything is read from them.
* **Skill orchestration** — running independent Skills and composing what they
  return without flattening their distinct semantics into one another.
* **Query and evidence routing** — deciding which Skill is eligible for a given
  request, with machine-readable reasons for every eligibility decision.
* **Citation and refusal handling** — binding every answer to re-verified native
  citations, and refusing — in typed, inspectable ways — when the evidence
  cannot support a conclusion.
* **Integration of independent Skills** — adapting each Skill's own public
  interface into the runtime's internal model, so the dependency runs from the
  private side into the public components and never the other way round.

This is a deliberately high-level description. The base's internal design and
implementation are not published here.

### What the private base is not

It is not a hosted service, and it is not required in order to use either public
Skill. Neither Skill calls into it, and neither will fail or degrade without it.

---

## Licensing

The **documentation in this repository** is licensed under the MIT License; see
`LICENSE` and `NOTICE.md`.

The two public Skills are licensed under the MIT License, with the notice
`Copyright (c) 2026 Peng Wang (Hu Deyi)`.

**The license here and in the Skills does not extend to the SeaFlow base
runtime.** The base is separately maintained private software, and no license is
granted to it by this repository or by the Skills. See `NOTICE.md`.

---

## Status and scope

This page is an informational overview, not a release announcement. SeaFlow is
research software under active development. Nothing here is a commitment about
future availability, and the presence of this page should not be read as one.
