# US College Admission Estimator MCP Server

Estimate US college admission chances in seconds -- GPA, test scores, and extracurriculars turned into safety/match/reach probabilities by your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/us-college-admission-estimator)

## Overview
**Category:** education-tools
**Tools Count:** 3

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


## Available Tools
- **estimate_admission_probability**: Estimate admission probability for universities by tier
- **calculate_applicant_score**: Use this as the first step in admission estimation.

Calculate composite academic score from GPA and standardized test scores
- **adjust_for_contextual_modifiers**: Returns an adjusted admissions score.

Apply residency and extracurricular modifiers to the composite score


## Installation & Usage

To install and use the **US College Admission Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-college-admission-estimator](https://vinkius.com/mcp/us-college-admission-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
