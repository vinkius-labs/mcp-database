# Epic Fhir MCP Server

Access patient records via Epic's FHIR R4 API — search patients, review encounters, pull lab results and medications from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/epic-fhir)

## Overview
**Category:** data-management
**Tools Count:** 10

## Description
Connect **Epic** electronic health records to any AI agent and query clinical data through natural conversation instead of navigating complex EHR interfaces.

### What you can do

- **Patient Search** — Find patients by name, date of birth, or medical record number across your Epic system
- **Clinical Encounters** — Review admissions, ER visits, and outpatient appointments with dates, reasons, and locations
- **Lab Results & Vitals** — Pull observations including blood work, vital signs, and social history with reference ranges
- **Diagnoses & Conditions** — List active and resolved conditions with ICD-10 codes, onset dates, and severity
- **Medications & Allergies** — View current prescriptions, dosage instructions, and documented allergic reactions
- **Appointments & Immunizations** — Check upcoming schedules and full vaccination history with lot numbers

### How it works

1. Subscribe to this server
2. Enter your FHIR Server URL, Client ID, and Access Token from your Epic App Orchard registration
3. Start querying patient records from Claude, Cursor, or any MCP-compatible client

Epic is the world's most widely used electronic health record system, serving over 305 million patients worldwide.

### Who is this for?

- **Clinical Informaticists** — extract patient cohort data and clinical metrics without writing SQL against the data warehouse
- **Care Coordinators** — quickly review a patient's full medical timeline before a care transition meeting
- **Health IT Developers** — prototype FHIR-based workflows and validate API responses interactively


## Available Tools
- **search_patients**: Returns patient demographics including name, DOB, gender, address, and identifiers.

Search patients by name, DOB, or MRN
- **list_immunizations**: Includes vaccine type (CVX code), administration date, dose, site, and lot number.

List immunizations
- **get_patient**: Returns name, DOB, gender, race, ethnicity, address, phone, email, and all identifiers.

Get patient details by ID
- **list_encounters**: Includes encounter type, period, reason, and location.

List patient encounters/visits
- **list_observations**: Filter by category: vital-signs, laboratory, social-history. Includes values, units, reference ranges, and interpretation.

List clinical observations
- **list_conditions**: Includes ICD-10 codes, clinical status, verification status, onset date, and severity.

List diagnoses and conditions
- **list_medications**: Includes medication name, dosage, frequency, route, prescriber, and status.

List medication requests
- **list_allergies**: Includes substance, reaction type, severity, and clinical status.

List allergies and intolerances
- **list_appointments**: Includes date/time, provider, location, and status.

List patient appointments
- **list_diagnostic_reports**: Includes report type, results, conclusion, and performing organization.

List diagnostic reports


## Installation & Usage

To install and use the **Epic Fhir** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epic-fhir](https://vinkius.com/mcp/epic-fhir)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
