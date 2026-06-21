# HID Origo MCP Server

Automate identity and access management via HID Origo — manage mobile identities, users, and readers directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hid-origo)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 11

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


## Installation & Usage

To install and use the **HID Origo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hid-origo](https://vinkius.com/mcp/hid-origo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
