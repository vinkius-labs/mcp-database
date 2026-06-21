# Qualified.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qualifiedio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/qualifiedio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/qualifiedio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate technical hiring and coding assessments — manage assessments, invite candidates, and track test results directly from your AI agent.

## Description
Connect your **Qualified.io** account to any AI agent to streamline your technical recruitment and engineering assessment workflows through natural conversation.

### What you can do

- **Assessment Management** — List, create, and manage the lifecycle of your coding assessments, including publishing and archiving.
- **Candidate Invitations** — Send assessment invitations to candidates and manage active invites directly through the API.
- **Result Tracking** — Retrieve detailed assessment results and streamlined exhibits to evaluate candidate performance instantly.
- **Lifecycle Control** — Terminate active results or schedule retries for candidates who need another attempt.
- **Cohort Analysis** — List and organize assessment cohorts to manage groups of candidates effectively.

### How it works

1. Subscribe to this server
2. Enter your Qualified.io API Key
3. Start managing your technical hiring pipeline from Claude, Cursor, or any MCP-compatible client

No more jumping between your ATS and assessment platform to check if a candidate has finished their test. Your AI acts as a technical recruiting coordinator.

### Who is this for?

- **Engineering Managers** — quickly review candidate scores and code exhibits without leaving the dev environment.
- **Technical Recruiters** — automate the process of inviting candidates and checking status updates.
- **Talent Operations** — manage large cohorts and assessment versions with simple natural language commands.


## Available Tools
- **archive_assessment**: Archive an assessment
- **cancel_invitation**: Cancel an assessment invitation
- **create_assessment_result_review**: Create a review for an assessment result
- **create_assessment**: Create a new assessment
- **get_assessment_result_exhibit**: Retrieve streamlined exhibit data for an assessment result
- **get_assessment_result**: Retrieve a specific assessment result
- **get_assessment**: Retrieve a specific assessment
- **get_challenge**: Retrieve a specific challenge
- **invite_candidates**: Invite candidates to take an assessment
- **invite_candidates_via_cohort**: Invite candidates via a cohort
- **list_assessment_cohorts**: List assessment cohorts
- **list_assessment_results**: List assessment results
- **list_assessments**: List assessments
- **list_challenges**: List challenges
- **publish_assessment**: Publish an assessment
- **schedule_retry_assessment_result**: Schedule a retry (reopen/retake) for an assessment result
- **terminate_assessment_result**: Terminate an assessment result
- **unarchive_assessment**: Unarchive an assessment
- **unpublish_assessment**: Unpublish an assessment
- **update_assessment_result_review**: Update a review for an assessment result


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qualified.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active assessments and their IDs."

**🤖 AI Agent:**
> I've retrieved your assessments. You have 3 active ones: 'Senior Fullstack Engineer' (ID: asmt_123), 'Junior Frontend' (ID: asmt_456), and 'Python Data Science' (ID: asmt_789).

---

**👤 You:**
> "Invite candidate 'John Doe' (john@example.com) to the 'Senior Fullstack' assessment."

**🤖 AI Agent:**
> I've sent the invitation to John Doe for the Senior Fullstack assessment (ID: asmt_123). The invitation ID is inv_987.

---

**👤 You:**
> "Show me the performance exhibit for result ID res_555."

**🤖 AI Agent:**
> For result res_555, the candidate scored 85%. They excelled in 'Algorithm Efficiency' but struggled slightly with 'Unit Test Coverage'. Would you like to see the full metadata?


## Installation & Usage

To install and use the **Qualified.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qualifiedio](https://vinkius.com/mcp/qualifiedio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
