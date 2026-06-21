# Pedagogical Assessment Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pedagogical-assessment-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A curriculum listed 12 learning objectives. Every one used 'understand' — an unmeasurable verb. Pedagogical Assessment Prover forces Bloom's-aligned objectives, explicit rubrics, scaffolded instruction, and actionable feedback.

## Description
AI agents generate lesson plans and assessments that look professional but violate fundamental principles of learning science. They write learning objectives using 'understand' — a verb that cannot be observed or measured. They assess at Level 1 (recall) while claiming to teach Level 4 (analysis). They provide feedback that is empty praise rather than actionable guidance.

### The Problem It Solves

AI-generated pedagogical reasoning fails for five specific reasons:

- **Taxonomy misalignment** — The learning objective says 'analyze' but the assessment tests 'remember.' This misalignment means you're measuring the wrong cognitive level.
- **Rubric absence** — Evaluation without explicit, observable, measurable criteria. 'Grade based on quality' is subjective judgment, not assessment.
- **Scaffolding gap** — Instruction that assumes prerequisites without diagnosing or building them. Teaching above the Zone of Proximal Development causes frustration, below it causes boredom.
- **Feedback vacuum** — 'Good job' and 'needs improvement' are value judgments, not feedback. Hattie's research (d = 0.70) shows feedback is among the most powerful influences on learning — but ONLY when task-specific and forward-looking.
- **Bias blindness** — Assessment that disadvantages learners based on cultural background, language proficiency, or neurological differences without systematic review.

### Key Benefits

- **Enforces Bloom's alignment** — Every learning objective must use observable verbs at the same cognitive level as the assessment task. No more 'students will understand.'
- **Demands explicit rubrics** — Observable criteria, distinct performance levels, behaviorally anchored descriptors, shared with learners before assessment.
- **Requires scaffolded instruction** — Prior knowledge diagnosis, prerequisite mapping, graduated release (I do → We do → You do), and UDL-compliant representations.
- **Forces actionable feedback** — Feed Up (where am I going?), Feed Back (how am I doing?), Feed Forward (where to next?) per Hattie & Timperley's model.
- **Audits for bias** — Cultural relevance, linguistic accessibility, UDL Principle II compliance, accessibility, and differential item functioning.

### Pedagogical Framework Coverage

- **Bloom's Taxonomy** — Anderson & Krathwohl (2001) revision
- **Webb's Depth of Knowledge** — DOK levels 1-4
- **Understanding by Design** — Wiggins & McTighe backward design
- **Zone of Proximal Development** — Vygotsky's scaffolding theory
- **Visible Learning** — Hattie's effect size research
- **Universal Design for Learning** — CAST framework, 3 principles
- **Assessment FOR Learning** — Stiggins formative assessment


## Available Tools
- **validate_pedagogical_assessment**: You must: (1) state learning OBJECTIVES using observable Bloom's verbs at the correct cognitive level — "understand" is not observable, "evaluate" is. Verb + content + condition, (2) design ASSESSMENT tasks that match the objective's cognitive demand — if the objective says "analyze," the assessment must require analysis, not recall, (3) provide explicit RUBRIC criteria — observable, measurable, distinct performance levels, shared with learners BEFORE assessment. If students do not know how they will be graded, they cannot target their learning, (4) design SCAFFOLDING — diagnose prior knowledge, identify prerequisites, graduated release (I do → We do → You do), multiple representations per UDL, (5) plan FEEDBACK per Hattie: Feed Up + Feed Back + Feed Forward. Task-specific, process-oriented, forward-looking. Not praise, not criticism, (6) AUDIT for bias — cultural, linguistic, accessibility. Not "it is fair" — a structured analysis with specific mitigations. If rejected, the pedagogical design has a structural deficiency. Fix before implementing.

Structured reflection tool for pedagogical reasoning and assessment design — forces Bloom's taxonomy alignment, explicit rubric construction, scaffolded instruction design, Hattie-model feedback planning, and systematic bias auditing before any educational assessment, lesson plan, or instructional intervention ships. Grounded in Bloom's Revised Taxonomy, Vygotsky's ZPD, Hattie & Timperley (2007), and Universal Design for Learning (UDL). Catches Taxonomy Misalignment (objective says one cognitive level, assessment tests another — objective: "Students will EVALUATE competing hypotheses about climate change." Evaluate = Bloom's Level 5 (highest analytical level). Assessment: a 40-question multiple-choice test asking "Which gas is the primary greenhouse gas?" This tests REMEMBER (Level 1), not EVALUATE (Level 5). The students who can recall facts but cannot construct an evidence-based argument score 95%. The students who can evaluate but struggle with recall score 60%. The assessment measures the wrong skill — it is structurally invalid. If the objective says "evaluate," the assessment must require students to compare, weigh evidence, and defend a position — not select from predetermined answers), Rubric Absent (grading without shared, explicit criteria — "I'll know good work when I see it" is not assessment — it is subjectivity. Two teachers grade the same essay. Teacher A: 82%. Teacher B: 67%. Neither is wrong — they simply weighted different things. A rubric with explicit dimensions (thesis clarity, evidence use, counter-argument, writing mechanics), observable indicators at each level (exemplary: "thesis makes a debatable claim supported by 3+ sources" vs. developing: "thesis restates the prompt"), and shared with students BEFORE the assignment — that produces inter-rater reliability > 0.85 and student performance gains of d = 0.70 (Hattie). Without it, grades measure the teacher, not the student), Scaffolding Gap (teaching at the target level without bridging from prior knowledge — Vygotsky's Zone of Proximal Development: learning happens between what a student can do alone and what they can do with guidance. Teaching ABOVE the ZPD produces frustration. Teaching BELOW produces boredom. A physics teacher assigns orbital mechanics problems to students who have not yet mastered vector addition. 40% of students fail — not because they cannot learn orbital mechanics, but because they are missing the prerequisite. Graduated release: I do (model) → We do (guided) → You do (independent). Multiple representations: diagram + equation + verbal explanation + simulation), Feedback Vacuum (empty praise or criticism instead of actionable guidance — "Good job!" has an effect size of d = 0.09 — nearly zero impact on learning. "Your thesis identifies the claim but lacks the counter-argument required by the rubric. Review the opposing evidence in Source 3 and add a paragraph addressing it" — that is task-specific, process-oriented, forward-looking feedback (d = 0.70). Hattie & Timperley (2007): Feed Up (where am I going?), Feed Back (how am I doing?), Feed Forward (where to next?). "Needs improvement" answers none of these questions), and Bias Blind (assessment that systematically disadvantages specific learner groups — a science assessment uses a baseball scenario to test physics (trajectory, velocity). Students familiar with baseball (predominantly US, male, middle-class) outperform students unfamiliar with the sport — not because of physics knowledge, but because of cultural context familiarity. The assessment measures cultural exposure, not scientific understanding. Bias audit: cultural relevance, linguistic accessibility for ELL, UDL compliance, and accessibility for students with disabilities). Call once per assessment, lesson plan, or educational intervention design


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pedagogical Assessment Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a lesson plan on photosynthesis for 9th grade biology. Students should understand the process and be tested on it."

**🤖 AI Agent:**
> TAXONOMY_MISALIGNED — 'understand' is not observable. What Bloom's level do you want? If 'Analyze': 'Students will diagram the light-dependent reactions, labeling inputs (H₂O, light), outputs (O₂, ATP, NADPH), and energy transformations.' Then assess at that SAME level — not with a multiple-choice recall quiz.

---

**👤 You:**
> "Design a rubric for a persuasive essay assignment in AP English. Include criteria for argument quality, evidence use, and writing mechanics."

**🤖 AI Agent:**
> PEDAGOGY_PROVEN — Rubric has 4 dimensions (Claim/Counter-claim, Evidence Integration, Rhetorical Strategy, Conventions) × 4 levels (Exemplary/Proficient/Developing/Beginning) with behaviorally anchored descriptors. Aligned to AP English CED Skill 4.B. Shared with students via pre-assessment workshop.

---

**👤 You:**
> "Assess whether this math class provides adequate support for struggling students. The teacher says 'I give extra practice sheets.'"

**🤖 AI Agent:**
> SCAFFOLDING_GAP — Extra practice sheets are repetition, not scaffolding. Vygotsky's ZPD requires: (1) diagnostic pre-assessment to identify WHAT students don't understand, (2) targeted intervention at the point of confusion, (3) graduated release with modeling first, (4) multiple representations per UDL. More of the same ≠ better support.


## ❓ FAQ

**Q: How does the prover measure alignment with Bloom's Taxonomy?**
By verifying that learning objectives use observable verbs at the same cognitive level as the assessment tasks. It rejects unmeasurable verbs like 'understand' or 'appreciate'.

**Q: What are the scaffolding requirements?**
It demands a clear plan for diagnosing prior knowledge, sequencing prerequisite concepts, and scaffolded instruction models (like the Graduated Release of Responsibility) rather than just giving extra practice sheets.

**Q: How does it detect and audit for bias?**
It scans assessment descriptions and rubrics for cultural assumptions, language barriers, and accessibility issues, ensuring compliance with Universal Design for Learning (UDL) principles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pedagogical-assessment-prover](https://vinkius.com/mcp/pedagogical-assessment-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pedagogical Assessment Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pedagogical-assessment-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pedagogical Assessment Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pedagogical-assessment-prover": {
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
