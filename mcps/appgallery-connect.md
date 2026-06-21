# AppGallery Connect MCP Server

Manage your AppGallery Connect apps via AI — check stats, submit builds for review, monitor ratings, and reply to user comments.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/appgallery-connect)

## Overview
**Category:** developer-tools
**Tools Count:** 11

## Description
Connect **AppGallery Connect** to your AI agent and manage your mobile app lifecycle through natural conversation.

### What you can do

- **App Management** — List all apps, view details, and check localization settings
- **Build Submission** — Get upload URLs and submit builds for review with status tracking
- **Analytics** — Access download stats, installation metrics, and performance data
- **User Feedback** — Read ratings, browse user comments, and reply directly
- **Review Pipeline** — Track submission status through the moderation process

### How it works

1. Subscribe to this server
2. Get your AGC Client ID and Secret from Users and Permissions > API Key in the console
3. Start managing your apps from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mobile Developers** — submit builds and check review status without opening the console
- **Product Managers** — monitor download and install metrics instantly
- **Support Teams** — respond to user reviews and feedback across apps


## Available Tools
- **get_app_info**: The appId can be found via list_apps.

Get detailed information for a specific application
- **get_app_language_info**: g. "en-US", "zh-CN", "pt-BR").

Get localized app information for a specific language
- **get_comments**: Get user comments and reviews for an application
- **get_download_stats**: Dates must be in YYYYMMDD format.

Get download statistics for an application
- **get_install_stats**: Dates must be in YYYYMMDD format.

Get installation statistics for an application
- **get_rating_info**: Get rating and review summary for an application
- **get_submission_status**: Check the review status of a submitted application
- **get_upload_url**: Specify the file suffix (e.g. "apk", "png").

Get a pre-signed upload URL for app binaries or assets
- **list_apps**: List all applications in the AppGallery Connect account
- **reply_to_comment**: Use get_comments to find comment IDs.

Reply to a user comment on the AppGallery
- **submit_for_review**: The app must have all required metadata and at least one valid binary uploaded.

Submit an application for review and publication


## Installation & Usage

To install and use the **AppGallery Connect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appgallery-connect](https://vinkius.com/mcp/appgallery-connect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
