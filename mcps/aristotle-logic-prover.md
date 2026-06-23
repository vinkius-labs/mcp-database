# Aristotle Logic Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aristotle-logic-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Your AI used a term without defining it. 'Platform,' 'scalable,' 'efficient' — what do these MEAN in your context? Aristotle defined every concept with genus + differentia: 'Man is a RATIONAL ANIMAL.' Category: animal. Distinguishing property: rational. This tool forces precise definition, essential vs. accidental categorization, valid syllogistic proof, teleological purpose analysis, and dialectical counterargument examination.

## Description
AI agents use terms without defining them. They confuse essential properties with accidental. They assert conclusions without valid logical structure. They describe mechanisms without understanding purpose. They never examine the strongest counterargument.

### The Problem

- **Definition Vague** — 'We need a scalable platform.' What IS a platform in your context? What category does it belong to? What distinguishes it? Aristotle: genus + differentia. 'Man is a RATIONAL ANIMAL' — genus: animal, differentia: rational.
- **Category Error** — 'It also does X, Y, and Z.' Which properties are ESSENTIAL (remove them and it becomes something else) vs. ACCIDENTAL (remove them and it remains the same thing)? Aristotle: being rational is essential to being human. Being 180cm tall is accidental.
- **Syllogism Invalid** — 'Therefore obviously this is the right approach.' 'Obviously' is assertion, not proof. Aristotle: 'All men are mortal. Socrates is a man. Therefore Socrates is mortal.' Valid syllogism — conclusion follows NECESSARILY.
- **Purpose Blind** — 'The implementation processes data through pipeline X.' That describes HOW, not WHY. Aristotle's four causes: material (resources), formal (structure), efficient (process), FINAL (telos/purpose). What is it FOR?
- **Dialectic Absent** — 'This is the only option.' Aristotle's students debated every position from BOTH sides. His 'Topics' catalogues 28 topoi for systematic dialectic.

### How It Works

1. **definitionPrecise** — Terms defined with genus + differentia.
2. **categorizedCorrectly** — Essential vs. accidental properties separated.
3. **syllogismValid** — Conclusion follows necessarily from premises.
4. **purposeIdentified** — Four causes identified, especially the telos.
5. **counterargumentExamined** — Strongest opposing argument steel-manned.

### Verdict Matrix

| Pivot | Verdict | Meaning |
|---|---|---|
| definitionPrecise = false | DEFINITION_VAGUE | Terms used without precise meaning. |
| categorizedCorrectly = false | CATEGORY_ERROR | Essential confused with accidental. |
| syllogismValid = false | SYLLOGISM_INVALID | Conclusion does not follow from premises. |
| purposeIdentified = false | PURPOSE_BLIND | Mechanism described, purpose unknown. |
| counterargumentExamined = false | DIALECTIC_ABSENT | No opposing argument examined. |
| All pass | LOGIC_PROVEN | Defined. Categorized. Proven. Purposed. Examined. |


## Available Tools (1)
- **validate_aristotle_logic**: Think like Aristotle — the father of formal logic and systematic categorization. You must: (1) DEFINE PRECISELY — every key term with genus (the broader category it belongs to) + differentia (the property that distinguishes it from other members of that genus). Aristotle: "Man is a RATIONAL ANIMAL" — genus: animal, differentia: rational. "A type of system" has no genus and no differentia, (2) CATEGORIZE CORRECTLY — separate essential properties (without which it would be a DIFFERENT thing entirely) from accidental properties (which can change without changing WHAT it is). Use Aristotle's 10 categories: substance, quantity, quality, relation, place, time, position, state, action, affection. Misclassifying accidental as essential is a category error, (3) PROVE SYLLOGISTICALLY — major premise (universal claim) + minor premise (specific case) + conclusion (necessary result). The conclusion must follow NECESSARILY from the premises. "Therefore obviously" is an assertion, not a valid inference. Test: would the conclusion hold even if the premises were hypothetically about different subjects? (4) IDENTIFY PURPOSE — Aristotle's four causes: material (what it is made of), formal (its essential structure), efficient (what process creates it), and FINAL (its telos — what it is FOR). The final cause is the most important. "How it works" answers the efficient cause. "What it is FOR" answers the final cause. Do not confuse mechanism with purpose, (5) EXAMINE THE STRONGEST COUNTERARGUMENT — dialectically. Aristotle's students debated every position from BOTH sides. Find the BEST argument against your position (steel-man, not straw-man), identify which of your premises it challenges, respond substantively, and note what residual doubt remains. If rejected, your logic has a formal deficiency — strengthen the argument.

Structured reflection tool for Aristotelian formal logic. Forces the agent to define terms with genus and differentia, classify essential vs accidental properties, prove conclusions through valid syllogisms, identify purpose through the four causes, and examine the strongest counterargument dialectically. Catches Definition Vagueness ("a type of system" — no genus, no differentia), Category Errors (treating accidental properties as essential — confusing what something IS with what it HAPPENS TO BE), Syllogism Invalidity (conclusions that do not follow necessarily from premises — "therefore obviously" masking logical leaps), Purpose Blindness (describing HOW something works without identifying WHAT it is FOR — mechanism without telos), and Dialectic Absence (no counterargument examined — claiming "there is no alternative" instead of steel-manning the strongest opposing position). Call once per classification, logical argument, or definitional analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aristotle Logic Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We need a scalable platform that is sort of like a hub for all our data. It also does reporting and analytics and additionally handles notifications. Therefore obviously we should build it as a single unified system."

**🤖 AI Agent:**
> DEFINITION_VAGUE — 'Platform,' 'scalable,' 'hub' — none of these terms are defined. Aristotle: genus + differentia. What CATEGORY does 'platform' belong to? What DISTINGUISHES it from a database, a service, or an application? 'Sort of like a hub' is not a definition. Additionally: 'it also does X, Y, Z' conflates essential and accidental properties. Is reporting ESSENTIAL (remove it and the system is no longer what it is) or ACCIDENTAL (remove it and the core thing remains)? Define first. Then categorize.

---

**👤 You:**
> "Definition: 'Order tracker' — genus: operational record-keeping system; differentia: tracks the lifecycle of customer requests from intake to delivery, distinguished from inventory systems (which track objects, not processes). Category: essential properties are (1) lifecycle tracking, (2) status transitions, (3) completion verification. Accidental: notification method (email vs. SMS), display format, report scheduling. Syllogism: All lifecycle tracking systems require status transition definitions. Our order tracker is a lifecycle tracking system. Therefore our order tracker requires status transition definitions. Purpose: Final cause (telos): ensure every customer request reaches completion within committed timelines. Material: order data, team assignments, deadline rules. Formal: sequential status pipeline with validation gates. Efficient: triggered by incoming customer request. Counterargument: Strongest counter — 'A spreadsheet achieves the same tracking with less effort.' This attacks the formal cause — is the pipeline structure necessary? Response: at <50 orders/week, a spreadsheet suffices. At our volume (380/week), manual status tracking produces 12% missed deadlines. The pipeline with validation gates reduced missed deadlines to 1.8%. Residual doubt: the 1.8% may reflect team behavior change, not the system itself."

**🤖 AI Agent:**
> LOGIC_PROVEN — Aristotelian logic complete. Definition precise: genus (operational record-keeping system) + differentia (lifecycle of customer requests), with boundary (distinguished from inventory systems). Category correct: essential (lifecycle, transitions, verification) separated from accidental (notification method, display format). Syllogism valid: major premise (all lifecycle systems need transitions), minor (our system is a lifecycle system), conclusion necessarily follows. Purpose identified through four causes, telos first (completion within timelines). Counterargument steel-manned (spreadsheet suffices at <50/week), addressed with data (380/week, 12%→1.8%), residual doubt acknowledged. This reasoning survives the Lyceum.

---

**👤 You:**
> "Definition: 'Workflow engine' — a system that automates tasks. Essential: does everything — routing, notifications, reporting, scheduling, approvals. Syllogism: Good organizations need automation. We are a good organization. This proves we need a workflow engine."

**🤖 AI Agent:**
> CATEGORY_ERROR — Definition passes partially ('automates tasks' is a start), but the category classification fails. 'Does everything — routing, notifications, reporting, scheduling, approvals' lists 5 properties as essential. Remove notifications — is it still a workflow engine? Yes. Remove reporting — still a workflow engine? Yes. Those are ACCIDENTAL properties. The ESSENTIAL property is task-state-transition management. Additionally, the syllogism is invalid: 'Good organizations need automation' is a vague major premise. What IS 'good'? What IS 'automation'? The conclusion 'this proves we need' does not follow necessarily — it follows ONLY if ALL automation is beneficial in ALL contexts, which is false.


## ❓ FAQ

**Q: How is this different from the Archimedes First Principles Prover?**
Archimedes forces DECOMPOSITION — break the problem into irreducible components. Aristotle forces FORMAL LOGIC — define terms precisely, prove conclusions through valid syllogisms, identify purpose through four causes, and examine counterarguments dialectically. Archimedes asks 'what are the components?' Aristotle asks 'is the argument VALID?'

**Q: What are Aristotle's four causes?**
Material (what is it made of?), Formal (what is its structure?), Efficient (what process made it?), Final (what is it FOR — the telos). Most people describe only the efficient cause — the mechanism. Aristotle demands the final cause first: why does this thing EXIST? What is its purpose?

**Q: Can I use this for product design, not just philosophical arguments?**
Yes. Every product decision involves definition (what IS this product — category and differentiator), categorization (which features are essential vs. nice-to-have), logical proof (does the conclusion follow from the premises), purpose (what is this product FOR — not what it does), and dialectic (what is the best argument against building this). Aristotle is not philosophy — it is the operating system of clear thinking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aristotle-logic-prover](https://vinkius.com/mcp/aristotle-logic-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aristotle Logic Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aristotle-logic-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aristotle Logic Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aristotle-logic-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
