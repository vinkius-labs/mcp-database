# D2L Brightspace MCP Server

Manage your D2L Brightspace LMS — administer courses, track student grades, and manage enrollments directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/d2l-brightspace)

## Overview
**Category:** productivity
**Tools Count:** 33

## Description
Connect your **D2L Brightspace** environment to any AI agent to streamline learning management and administrative workflows.

### What you can do

- **Course Management** — Retrieve course details, create new offerings, and copy course content between org units using `get_course` and `copy_course`.
- **User Administration** — List system users, create new accounts, and manage roles and permissions with `list_users` and `create_user`.
- **Grade Tracking** — Access grade lists and update individual student grades for specific assignments using `get_user_grade` and `update_user_grade`.
- **Content & Communication** — Explore course modules, manage discussion forums, and create new topics or posts via `list_root_modules` and `create_post`.
- **Assessments** — Monitor quizzes, surveys, and assignment submissions, and provide direct feedback using `list_submissions` and `provide_feedback`.

### How it works

1. Subscribe to this server
2. Provide your Brightspace Host URL and Access Token
3. Start managing your educational ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Instructors** — Quickly check student progress, provide feedback on assignments, and manage course content without navigating complex menus.
- **LMS Administrators** — Automate user creation, enrollment management, and organizational unit structuring.
- **Academic Researchers** — Extract course data and assessment metrics for analysis through natural language queries.


## Available Tools
- **copy_course**: Initiate a course copy job
- **create_course**: Create a course offering
- **create_enrollment**: Enroll a user in an org unit
- **create_lti_deployment**: Create an LTI Advantage tool deployment
- **create_org_unit**: Create custom org units
- **create_post**: Create a post in a discussion topic
- **create_topic**: Create a discussion topic in a forum
- **create_user**: Create a new user
- **delete_enrollment**: Unenroll a user from an org unit
- **get_course_template**: Retrieve course template info
- **get_course**: Retrieve course details
- **get_org_unit**: Retrieve org unit properties
- **get_user_grade**: Retrieve user grades for a specific grade object
- **list_assignment_folders**: List assignment folders (dropboxes)
- **list_forums**: List discussion forums in a course
- **list_grades**: List grade objects for a course
- **list_legacy_lti_links**: List legacy LTI 1.1 links
- **list_lti_registrations**: List LTI Advantage tool registrations
- **list_my_eportfolio_objects**: List current user ePortfolio objects
- **list_my_enrollments**: List current user enrollments
- **list_org_unit_children**: List child units of an org unit
- **list_quiz_attempts**: List attempts for a specific quiz
- **list_quizzes**: List quizzes in a course
- **list_roles**: Retrieve system roles
- **list_root_modules**: List root modules of course materials
- **list_submissions**: List submissions for an assignment folder
- **list_surveys**: List surveys in a course
- **list_users**: Search or page through users
- **provide_feedback**: Provide feedback for an assignment submission
- **update_user_grade**: Update a user grade
- **update_user**: Update user data
- **upload_eportfolio_artifact**: Upload a file artifact to ePortfolio
- **get_whoami**: Retrieve current user context


## Installation & Usage

To install and use the **D2L Brightspace** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/d2l-brightspace](https://vinkius.com/mcp/d2l-brightspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
