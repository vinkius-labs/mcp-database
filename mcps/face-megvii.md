# Face++ / Megvii MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/face-megvii)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Leading facial recognition and computer vision platform — detect faces, compare identities, and analyze body gestures via AI.

## Description
Empower your AI agent to orchestrate your computer vision operations with **Face++** (Megvii), the dominant facial recognition platform in China. By connecting Face++ to your agent, you transform complex image analysis and identity verification into a natural conversation. Your agent can instantly detect faces, compare similarities between photos, search within face databases (FaceSets), and analyze human body skeletons or gestures without you ever needing to navigate the comprehensive web console. Whether you are conducting KYC audits or monitoring visual content, your agent acts as a real-time vision intelligence assistant, providing accurate and fast results from a single, unified source.

### What you can do

- **Face Orchestration** — Detect faces in images and retrieve detailed attributes like age, gender, and emotion.
- **Identity Verification** — Compare two images to calculate confidence that they belong to the same person.
- **FaceSet Management** — Create and manage searchable face databases for large-scale matching.
- **Body & Skeleton Analysis** — Detect human bodies and skeletons to analyze posture and movement.
- **Gesture Recognition** — Identify specific hand gestures from image data.

### How it works

1. Subscribe to this server
2. Enter your Face++ API Key and API Secret
3. Start querying vision data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security & Compliance** — automate identity verification and KYC processes through natural language queries.
- **UX Researchers** — analyze user emotions and gestures during product testing directly from your AI-powered workspace.
- **Developers** — integrate a massive library of computer vision APIs into your AI-driven daily routines.
- **Face++ Power Users** — integrate your existing vision workflows into your AI-driven daily routines.


## Available Tools (10)
- **add_face_to_faceset**: Add faces to a FaceSet
- **compare_faces**: Compare two faces for similarity
- **create_faceset**: Create a new FaceSet
- **detect_body**: Detect human bodies in an image
- **detect_face**: Detect faces in an image
- **gesture_detect**: Detect hand gestures
- **get_faceset_detail**: Get details of a FaceSet
- **remove_face_from_faceset**: Remove faces from a FaceSet
- **search_face**: Search for a face in a FaceSet
- **skeleton_detect**: Detect human skeletons


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Face++ / Megvii** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Detect faces in this image URL: [URL]."

**🤖 AI Agent:**
> I've analyzed the image. I found 2 faces. Face 1 appears to be a male around 30 years old with a happy expression. Face 2 is a female around 28 years old with a neutral expression. Would you like to see the face tokens for these results?

---

**👤 You:**
> "Compare these two images to see if they are the same person: [URL1] and [URL2]."

**🤖 AI Agent:**
> I've compared the faces. There is a 98.5% confidence that both images belong to the same person. This is well above the recommended threshold for matching identities.

---

**👤 You:**
> "Check for any human body detected in this photo: [URL]."

**🤖 AI Agent:**
> I've retrieved the body detection results. I found 1 human body in the image. Would you like to analyze the skeleton keypoints or check for any specific hand gestures?


## ❓ FAQ

**Q: How do I find my Face++ API Key and Secret?**
Log in to the [Face++ Console](https://console.faceplusplus.com.cn/), go to [Dashboard] -> [API Key], and you will find your unique Key and Secret there. Ensure you have the necessary permissions enabled.

**Q: Can I analyze images from a local file?**
This server currently supports analysis via `image_url`. To use local files, you should upload them to a public or private storage and provide the resulting URL to the tools.

**Q: What attributes can be returned during face detection?**
Common attributes include gender, age, emotion, head pose, smile, face quality, and skin status. You can specify these in the `return_attributes` parameter of the `detect_face` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/face-megvii](https://vinkius.com/mcp/face-megvii)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Face++ / Megvii** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `face-megvii` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Face++ / Megvii** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "face-megvii": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
