# US College Admission Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-college-admission-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education-tools](../categories/education-tools.md)

Estimate US college admission chances in seconds -- GPA, test scores, and extracurriculars turned into safety/match/reach probabilities by your AI agent.

## Description
Connect your **US College Admission Estimator** to any AI agent and stop guessing which schools are actually realistic. Your AI client gains a scoring engine that runs GPA, test scores, residency status, and extracurricular depth through real benchmarks -- not vague advice.

### The Problem It Solves

Students and families waste hours scrolling college websites, reading acceptance rates that say nothing about *their* odds. High stats on paper don't tell you if a school is a safety, a match, or a reach. What you need is a quick number -- not a 40-page guide.

### How It Works

The estimator runs in three steps. Your AI agent handles each one:

1. **Calculate the composite score** -- Use the `calculate_applicant_score` query with your weighted GPA (0-5.0) and optional SAT/ACT scores. It returns a 0-100 composite score.
2. **Apply context** -- Feed that score into `adjust_for_contextual_modifiers` along with residency status (In-State, Out-of-State, International) and extracurricular level (Exceptional, Strong, Average). You get back an adjusted admissions score.
3. **Get tier-specific probabilities** -- Pass the adjusted score to `estimate_admission_probability`, pick a university tier (Elite Private, Flagship Public State, or Mid-Sized Private), and receive safety/match/reach admission percentages for real schools in that group.

### The Verdict Matrix

| Score Range | Elite Private | Flagship Public | Mid-Sized Private |
|-------------|---------------|-----------------|-------------------|
| 0-59 | Reach (low %) | Match or Safety | Mostly Safety |
| 60-74 | Reach | Match | Safety |
| 75-85 | Reach or Match | Match or Safety | Safety |
| 86-100 | Possible Match | Safety | Safety |

### Why It Works

- **Weighted scoring actually reflects admissions logic** -- GPA carries more weight than test scores, which mirrors how real admissions offices evaluate profiles
- **Residency matters** -- state residents get a fair bump the way public universities factor that in
- **No fluff** -- you get numbers, not platitudes about "following your passion"

Simple. You have the score. Here's where it puts you.


## Available Tools (3)
- **estimate_admission_probability**: Estimate admission probability for universities by tier
- **calculate_applicant_score**: Use this as the first step in admission estimation.

Calculate composite academic score from GPA and standardized test scores
- **adjust_for_contextual_modifiers**: Returns an adjusted admissions score.

Apply residency and extracurricular modifiers to the composite score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US College Admission Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 3.8 weighted GPA, scored 1420 on the SAT, and I'm an in-state applicant with strong extracurriculars. What are my chances at flagship public universities?"

**🤖 AI Agent:**
> Let me run those numbers through the estimator...

Step 1: Your composite score from GPA and SAT is 78.
Step 2: After applying in-state residency and Strong extracurricular adjustments, your adjusted score comes to 84.
Step 3: At Flagship Public State tier, you're looking at roughly 70-85% probability -- solidly in the Match zone. Consider adding one Elite Private reach school with that profile too.

---

**👤 You:**
> "My daughter has a 4.5 weighted GPA but no test scores yet. She's international and plans to apply as an Exceptional extracurricular candidate. Should we target elite private schools?"

**🤖 AI Agent:**
> Right. So -- let me calculate with just her GPA first, since test scores are optional...

Her composite score from a 4.5 GPA alone lands at around 82. After adjusting for International status and Exceptional extracurriculars, the score dips slightly to about 76.

At Elite Private tier, that puts her in the reach zone with roughly 10-15% odds. I'd recommend pairing it with Mid-Sized Private schools where she'd be a safety/match (70%+ probability) to keep options open.

---

**👤 You:**
> "I scored 32 on the ACT and have a 3.4 weighted GPA. I'm applying as an out-of-state student with average extracurricular activities. What tier should I target?"

**🤖 AI Agent:**
> Here's the breakdown:

Composite score: 64 (weighted GPA + ACT 32)
Adjusted for Out-of-State + Average extracurriculars: 58

At Mid-Sized Private tier, that's a comfortable Safety zone -- you're looking at solid admission odds. Even at Flagship Public State, you'd land in the Match-to-Safety range with decent probabilities. Don't waste time applying to Elite Private schools; the odds there will be thin.


## ❓ FAQ

**Q: Do I need both SAT and ACT scores to get an estimate?**
No. The `calculate_applicant_score` tool accepts either your SAT composite (400-1600) or your ACT total (1-36), or even just your weighted GPA alone. It weights everything into a 0-100 score so you get a solid baseline no matter what data you have.

**Q: How does residency status change my admission odds?**
Public universities heavily favor in-state applicants. When you pass your composite score through the `adjust_for_contextual_modifiers` tool with In-State residency, the adjusted score goes up. Out-of-State gets a smaller bump, and International status applies a slight reduction. This mirrors how real admissions committees weigh state residency.

**Q: Can I estimate chances at specific named universities?**
Not by individual school name -- not yet. The `estimate_admission_probability` tool groups schools into three tiers: Elite Private, Flagship Public State, and Mid-Sized Private. You get percentages for real universities within each tier, which gives you a practical safety/match/reach breakdown to plan your application list.

**Q: What counts as my weighted GPA?**
Your weighted GPA factors in AP, IB, or honors class rigor. It can go up to 5.0 (or even higher at some schools). Just enter whatever your high school reports -- the `calculate_applicant_score` tool normalizes it into a fair composite that plays well with both tested and test-optional profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-college-admission-estimator](https://vinkius.com/mcp/us-college-admission-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US College Admission Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-college-admission-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US College Admission Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-college-admission-estimator": {
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
