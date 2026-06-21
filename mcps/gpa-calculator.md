# GPA Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gpa-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gpa-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gpa-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate weighted GPA for US (4.0) and Brazilian (10.0) scales, including honors classification.

## Description
The GPA Calculator MCP provides a specialized engine for determining weighted Grade Point Averaged across different academic grading systems. It allows users to calculate the single-period weighted average using `compute_weighted_gpa`, evaluate performance trends between semesters with `compare_semesters`, and normalize grades between scales via `convert_grade_scale`. Perfect for students and educators managing US 4.0 and Brazilian 10.0 academic records.


## Available Tools
- **compare_semesters**: Evaluates the performance trend between two different academic periods
- **compute_weighted_gpa**: Returns weighted GPA, honors status, and total credits.

Calculates the single-period weighted average and determines if the student qualifies for academic honors
- **convert_grade_scale**: A utility to normalize a grade from one academic system to another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GPA Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my GPA for this semester: Math (Grade 4.0, 3 credits) and History (Grade 3.0, 2 credits) on the US scale."

**🤖 AI Agent:**
> Your weighted GPA is 3.6, which qualifies you for Cum Laude honors.

---

**👤 You:**
> "Compare my performance: Current semester (Grade 8.0, 4 credits) vs Previous semester (Grade 7.0, 4 credits) on the BR scale."

**🤖 AI Agent:**
> Your GPA increased by 1.0, showing an Improved performance trend.

---

**👤 You:**
> "Convert a grade of 8.5 from the Brazilian scale to the US scale."

**🤖 AI Agent:**
> A grade of 8.5 on the Brazilian scale is equivalent to 3.4 on the US scale.


## Installation & Usage

To install and use the **GPA Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gpa-calculator](https://vinkius.com/mcp/gpa-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
