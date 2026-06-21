# Doctolib MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doctolib)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doctolib-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doctolib-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage medical appointments via Doctolib — search practitioners by specialty and city, track availabilities, and book consultations directly from any AI agent.

## Description
Connect your **Doctolib** partner account to any AI agent and take full control of your healthcare scheduling and practitioner research through natural conversation.

### What you can do

- **Practitioner Discovery** — Search for doctors and specialists by specialty and city, identifying bounded office locations and member approximations natively
- **Availability Tracking** — Identify bounded routing spaces verifying absolute time availability slots attached directly matching the targeted doctor
- **Appointment Management** — List complex mappings evaluating exactly scheduled times and identifying physical reservations active within your account
- **Live Booking** — Commands the backend orchestrating real-time database locks inserting explicit reservation parameters structurally binding to an exact time slot
- **Visit Motive Identification** — Read available reason categories explicitly supported by a given Practitioner required for slot lock verification
- **Practice Navigation** — Perform structural extraction of localized entity bounds configuring the raw office locations active within the application
- **Specialty Mapping** — Enumerate explicitly attached structured roles defining valid medical specialties and practitioner targets globally

### How it works

1. Subscribe to this server
2. Enter your Doctolib Partner API Key and API URL (e.g., https://api.doctolib.fr)
3. Start managing your healthcare appointments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Patients** — search for specialists and book appointments without navigating the web interface
- **Healthcare Coordinators** — manage schedules for multiple patients and verify doctor availability in real-time
- **Medical Software Vendors** — test and debug Doctolib integrations and appointment booking flows through natural conversation
- **Administrative Assistants** — audit scheduled visits and manage appointment logs using natural language


## Available Tools
- **rechercher_praticiens**: Restricts search to explicit city boundaries natively bypassing local lists.

Rechercher des praticiens par spécialité et ville
- **consulter_praticien**: Consulter le profil d'un praticien
- **lister_specialites**: Lister toutes les spécialités médicales disponibles
- **disponibilites**: Vérifier les créneaux disponibles pour un praticien
- **lister_rendez_vous**: Lister les rendez-vous pris
- **prendre_rendez_vous**: Prendre un rendez-vous médical
- **lister_cabinets**: Lister les cabinets médicaux
- **motifs_consultation**: Lister les motifs de consultation d'un praticien


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Doctolib** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for general practitioners in Paris"

**🤖 AI Agent:**
> I found 5 general practitioners in Paris. Top results include 'Dr. Martin' (75001) and 'Dr. Lefebvre' (75008). Would you like to check their available slots for this week?

---

**👤 You:**
> "What are the available slots for Dr. Martin (ID: 123) tomorrow?"

**🤖 AI Agent:**
> Dr. Martin has 3 slots available tomorrow: 10:00 AM, 11:30 AM, and 2:00 PM. Would you like to book one of these using your registered email?

---

**👤 You:**
> "List my upcoming medical appointments"

**🤖 AI Agent:**
> Retrieving appointments... You have 1 upcoming consultation: 'Dr. Martin' on Wednesday at 10:00 AM. I can provide the practice address and motive for you.


## Installation & Usage

To install and use the **Doctolib** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doctolib](https://vinkius.com/mcp/doctolib)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
