# HID Origo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hid-origo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hid-origo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hid-origo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Automate identity and access management via HID Origo — manage mobile identities, users, and readers directly from any AI agent.

## Description
Connect your **HID Origo** platform to any AI agent and take full control of your cloud-based identity and physical access management through natural conversation.

### What you can do

- **Mobile Identity Oversight** — List and retrieve details for all issued mobile identities (digital cards) and monitor their activation status.
- **User & Group Management** — Access lists of users and identity groups defined in your tenant to ensure correct access policies.
- **Enrollment Automation** — Send enrollment invitations for mobile identities directly from the chat interface.
- **Reader & Hardware Monitoring** — List and monitor the status of IoT readers and door controllers connected to your organization.
- **Credential Tracking** — Manage both physical and digital credentials linked to your users in a unified view.
- **Security Auditing** — Retrieve system audit logs to monitor administrative actions and access events.

### How it works

1. Subscribe to this server
2. Enter your HID Origo Client ID, Client Secret, and Organization ID
3. Start managing your access control from Claude, Cursor, or any MCP-compatible client

No more navigating complex management portals for simple identity lookups. Your AI assistant acts as a dedicated Access Control Administrator or Security Specialist.

### Who is this for?

- **Facility Managers** — instantly check the status of readers and mobile credentials across multiple sites.
- **Security Engineers** — automate the auditing of access events and identify enrollment bottlenecks.
- **IT Admins** — streamline the process of inviting users to mobile identity enrollment during onboarding.


## Available Tools
- **create_enrollment_invitation**: Pass the invitation details as a JSON string in "body_json" (requires userId and partNumber).

Send a new invitation to a user for mobile identity enrollment
- **get_audit_log_events**: Useful for security monitoring and troubleshooting enrollment issues.

Retrieve the history of administrative and access events
- **get_mobile_identity**: Get details for a specific mobile identity
- **get_organization_info**: Retrieve metadata and configuration for your HID Origo organization
- **get_user_details**: Get detailed information for a specific user ID
- **list_physical_credentials**: List physical access credentials (cards, fobs) managed in the system
- **list_identity_groups**: List identity groups used for access control policies
- **list_identity_invitations**: List all invitations sent for mobile identity enrollment
- **list_mobile_identities**: Monitor issuance and activation status.

List all issued mobile identities (digital cards)
- **list_access_readers**: List all IoT readers and door controllers connected to HID Origo
- **list_identity_users**: Use this to find the user ID for credential or mobile identity assignment.

List all users managed in the HID Origo tenant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HID Origo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active mobile identities and their status."

**🤖 AI Agent:**
> I've retrieved your mobile identities. You have 15 issued digital cards, including 12 'Activated' and 3 'Pending Enrollment'. Would you like to see the details for the pending identities to follow up with the users?

---

**👤 You:**
> "Show me the status of the access readers in the 'London Office'."

**🤖 AI Agent:**
> Accessing reader data... In the 'London Office' (ID: loc_552), all 5 HID Signo readers are currently ONLINE and reporting normal activity. Would you like to see the recent access events for these readers?

---

**👤 You:**
> "Invite user 'user_992' to enroll for a mobile identity."

**🤖 AI Agent:**
> Process started! I've initiated an enrollment invitation for user_992. I'll use your default part number for the digital card. An email will be sent to the user with instructions to activate their credential in the HID Origo app. Should I check the audit log to confirm the invite was sent?


## Installation & Usage

To install and use the **HID Origo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hid-origo](https://vinkius.com/mcp/hid-origo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
