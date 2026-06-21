# Nhost MCP Server

Manage Nhost authentication and storage — handle user sign-ins, registrations, profile management, and file uploads directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nhost)

## Overview
**Category:** developer-tools
**Tools Count:** 15

## Description
Connect your **Nhost** project to any AI agent to manage your backend services through natural language. This server provides a comprehensive interface for Nhost's Authentication and Storage services.

### What you can do

- **Authentication Flows** — Sign in users via email/password, OTP, magic links, or anonymous sessions using `signin_email_password`, `signin_otp_email`, and `signin_passwordless_email`.
- **User Management** — Register new accounts with `signup_email_password`, retrieve profiles with `get_user`, and handle password resets or email changes.
- **Session Control** — Refresh access tokens and securely sign out users from single or all devices using `refresh_token` and `signout`.
- **Cloud Storage** — Upload files directly to your Nhost buckets using the `upload_file` tool, supporting both text and base64 content.

### How it works

1. Subscribe to this server
2. Provide your Nhost Auth and Storage URLs from your project dashboard
3. Start managing users and files from Claude, Cursor, or any MCP client

### Who is this for?

- **Full-stack Developers** — manage user sessions and test auth flows directly from the IDE without switching to the browser.
- **DevOps Engineers** — automate user provisioning and file management tasks through simple conversation.
- **Support Teams** — quickly verify user profile information and account status to resolve customer issues faster.


## Available Tools
- **change_email**: Requires elevated NHOST_JWT credential.

Request to change the authenticated user email
- **delete_file**: Permanently delete a file
- **get_file_presigned_url**: Retrieve a presigned URL for a file
- **get_file**: Supports optional image transformation parameters.

Download the complete file content
- **get_user**: Requires NHOST_JWT credential.

Retrieve the authenticated user profile information
- **refresh_token**: Generate a new JWT access token using a valid refresh token
- **reset_password**: Request a password reset email
- **signin_anonymous**: Create an anonymous user session
- **signin_email_password**: Authenticate a user with email and password
- **signin_otp_email**: Initiate email-based one-time password authentication
- **signin_passwordless_email**: Initiate passwordless authentication by sending a magic link
- **signout**: Invalidate refresh tokens and end the session
- **signup_email_password**: Register a new user account
- **signup_otp_email**: Register a new user account using email OTP
- **upload_file**: Returns metadata for the processed file.

Upload a file to a bucket


## Installation & Usage

To install and use the **Nhost** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nhost](https://vinkius.com/mcp/nhost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
