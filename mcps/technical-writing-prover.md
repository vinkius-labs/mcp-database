# Technical Writing Prover MCP Server

An AI wrote API documentation for 'developers.' No expertise level. No prerequisites. A wall of text with no headings. Code examples that referenced a deprecated method — untested. Passive voice throughout: 'it is recommended that the configuration be updated.' A junior engineer followed the docs, deployed to production with the wrong config, and caused a 4-hour outage. This tool forces audience definition, task-based structure, tested examples, ambiguity elimination, and completeness verification.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/technical-writing-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI agents write documentation that reads well — and misleads in production. They write for 'developers' without specifying who. They produce walls of text with no navigation. They include untested code examples. They use passive voice that hides responsibility. They skip error handling, prerequisites, and next steps.

### The Problem

LLMs commit five technical writing failures that compound in production:

- **Undefined Audience** — Written for 'developers' — that is everyone from a CS student to a staff engineer. No expertise level stated. No prerequisites listed. A junior engineer follows senior-level docs, misses implicit assumptions, and deploys a broken config. 67% of documentation complaints cite 'assumed too much knowledge.'
- **Absent Structure** — A wall of text with no headings, no progressive disclosure. The reader cannot scan to find what they need. No Diátaxis classification — is this a tutorial, a how-to, a reference, or an explanation? The reader does not know, and neither does the author.
- **Missing or Untested Examples** — 'Something like this' followed by pseudocode that does not compile. Code referencing deprecated APIs. No expected output shown. No runtime version specified. The reader copies the example, and it fails.
- **Present Ambiguity** — 'It is recommended that the configuration be updated.' Who recommends? Which configuration? Updated how? Passive voice hides the actor. Pronouns without antecedents. Terms used before definition. The reader guesses — and guesses wrong.
- **Completeness Gaps** — No prerequisites section. No error handling ('if this fails, do X'). No edge cases. No next steps. 'Left as an exercise' and 'consult the official docs' — the documentation fails to document.

### How It Works

Technical Writing Prover validates documentation quality through 5 Decision Pivots:

1. **audienceDefined** — Specific reader with role (backend engineer, DevOps, data scientist), expertise level (junior/mid/senior), prerequisites (languages, frameworks they must know), and goal (task accomplished after reading). Not 'developers.'
2. **structurePresent** — Diátaxis classification (tutorial/how-to/reference/explanation), task-based heading hierarchy (H1→H2→H3), progressive disclosure (simple → advanced), scannable navigation. Not wall-of-text.
3. **examplesWorking** — Complete, copy-pasteable code blocks with language in fence, expected output shown, tested on stated runtime version. Not 'something like this' or pseudocode.
4. **ambiguityEliminated** — Active voice ('use X' not 'it is recommended'), clear pronoun antecedents, terms defined on first use, vague quantifiers replaced with specifics. Not 'various factors.'
5. **completenessVerified** — Prerequisites listed with version numbers, error paths documented ('if this fails, do X'), edge cases covered, next steps linked. Not 'beyond the scope.'

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| audienceDefined = false | AUDIENCE_UNDEFINED | 'Developers' is everyone. No specific reader targeted. |
| structurePresent = false | STRUCTURE_ABSENT | Wall of text. No headings, no navigation, no Diátaxis. |
| examplesWorking = false | EXAMPLES_MISSING | Pseudocode or untested code. Reader copies and fails. |
| ambiguityEliminated = false | AMBIGUITY_PRESENT | Passive voice, unclear pronouns, undefined terms. |
| completenessVerified = false | COMPLETENESS_GAPS | Missing prerequisites, error handling, or next steps. |
| All pivots pass | WRITING_PROVEN | Defined, structured, exemplified, clear, complete. |

### Why It Works

- **Tool calls are obligations.** The agent cannot skip audience definition or claim completeness without listing prerequisites and error paths. Filling the fields IS the documentation work.
- **Consistency engine catches contradictions.** If the agent claims `examplesWorking=true` but describes 'pseudocode,' the engine rejects with a specific coaching message.
- **Semantic traps detect hand-waving.** Phrases like 'developers,' 'left as an exercise,' 'it is recommended,' or 'something like this' trigger automatic rejection. Name the audience. Write the example. State the subject.


## Available Tools
- **validate_technical_writing**: You must: (1) define the SPECIFIC reader — role, expertise level, prerequisites, goal, (2) structure with Diátaxis classification, task-based headings, and progressive disclosure, (3) provide complete, copy-pasteable code examples with expected output and tested versions, (4) eliminate passive voice, undefined pronouns, and undefined terms, (5) verify prerequisites are listed, error paths documented, edge cases covered, and next steps linked. If rejected, fix the specific documentation gap the engine identifies.

Structured reflection tool that forces the LLM to prove technical documentation meets professional standards — defined audience, task-based structure, working examples, eliminated ambiguity, and verified completeness. Based on the Diátaxis framework (Daniele Procida, 2017): documentation has exactly 4 types — tutorials (learning-oriented), how-to guides (task-oriented), reference (information-oriented), and explanations (understanding-oriented). Mixing these types creates confused documents. Catches Audience Undefined (writing for "everyone" = writing for no one — a pharmaceutical label reads: "Take as needed for pain relief. May cause adverse events." "As needed" — how often? Maximum dose? Interval? "Adverse events" — what kind? Headache? Organ failure? Death? The label was written for "patients" — but a 22-year-old athlete and a 78-year-old with liver disease need fundamentally different information. For the athlete: dosing schedule and interaction with supplements. For the elderly patient: maximum daily dose, interaction with blood thinners, renal dosing adjustment. One label for both = inadequate for both. Fix: define the SPECIFIC reader — role, expertise, prerequisites, goal — BEFORE writing), Structure Absent (wall of text without task-based organization — a fire escape diagram is posted in a hotel hallway. It shows all 8 floors, all stairwells, all exits — on one diagram. No floor numbers labeled. No "YOU ARE HERE" marker. No step-by-step evacuation route. Guest at 3am, smoke in hallway: looks at diagram, cannot find their floor, cannot identify direction. Fix: ONE diagram per floor. "YOU ARE HERE" marked. Arrows showing the route to the nearest exit. Step 1: Exit room, turn LEFT. Step 2: Follow hallway to Stairwell B. Step 3: Descend to ground floor. Task-based structure: the reader has ONE task (get out alive). Every element serves that task), Examples Missing (concepts without working demonstrations — an IKEA assembly instruction shows Step 7: "Attach Part K to Frame Assembly using Cam Lock." Problem: Part K is not in the parts list. Not in the hardware bag. Not in any diagram. The customer cannot identify Part K. Step 7 is impossible to execute. The instruction assumed the reader would know what Part K is. They do not. Fix: every referenced part must appear in the parts inventory with a photograph, size, and quantity. Every step must be executable with only the materials provided. If Step 7 references Part K: Part K must exist, be identifiable, and be available), Ambiguity Present (passive voice and undefined terms causing dangerous misinterpretation — an aircraft maintenance manual reads: "The bolt should be tightened." Which bolt? (there are 47 bolts in this assembly). To what torque? "Should be" — is it mandatory or recommended? A technician interprets "tightened" as hand-tight (5 Nm). The specification requires 45 Nm. Result: bolt fails under vibration. Component separates during flight. FAA Advisory Circular AC 43.13-1B mandates specific, active-voice maintenance documentation. Fix: "Torque bolt P/N AN3-12A to 45 ± 2 Nm using calibrated torque wrench." Active voice. Specific part number. Exact specification. Measurable tolerance. Rule: if two technicians could interpret the same sentence differently, the sentence will be interpreted wrong by one of them), and Completeness Gaps (missing prerequisites, error paths, or edge cases — a vaccine consent form explains: "This vaccine may cause mild side effects." "Mild" — according to whom? "Side effects" — which ones? For how long? When to call a doctor? Complete version: "Common effects (>10% of recipients): injection site soreness (1-3 days), fatigue (1-2 days), headache (1 day). Uncommon (1-10%): low-grade fever (< 38.5°C, 1 day). Rare (<0.1%): severe allergic reaction — seek emergency care if: difficulty breathing, facial swelling, rapid heartbeat within 30 minutes of injection." Every claim has a frequency. Every symptom has a duration. Every emergency has an action. The reader knows: what to expect, when to wait, and when to seek help). Call once per documentation, guide, or technical writing review


## Installation & Usage

To install and use the **Technical Writing Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/technical-writing-prover](https://vinkius.com/mcp/technical-writing-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
