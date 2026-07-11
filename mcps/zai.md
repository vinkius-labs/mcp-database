# Z.AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access the full Z.AI platform from any AI agent — chat completions with GLM models, image and video generation, audio transcription, OCR, web search, and agent tools.

## Description
Connect your **Z.AI** API key to any AI agent and unlock the full power of the Z.AI platform through natural conversation.

### What you can do

- **Chat Completions** — Generate AI responses using GLM-5.2, GLM-4.7, GLM-4.7-flash, and other models with support for multimodal inputs (text, images, audio, video, files), tool use, and streaming
- **Image Generation** — Create high-quality images from text prompts using GLM-Image or CogView-4 models, with synchronous and asynchronous modes
- **Video Generation** — Generate videos from text or images using CogVideoX-3 or Vidu models, with optional audio, quality modes, and resolution control
- **Audio Transcription** — Convert speech to text using the GLM-ASR-2512 model with hotword support and streaming output
- **OCR & Layout Parsing** — Extract text from images and PDFs using the GLM-OCR model, with detailed layout information and visualization
- **Web Search** — Search the web with Z.AI's LLM-optimized search engine, returning titles, URLs, summaries, and favicons
- **Web Reader** — Read and parse any web page URL into clean markdown or text with metadata extraction
- **Tokenization** — Count tokens for messages to estimate costs and manage context windows
- **Agent Tools** — Run translation (40+ languages), slide/poster generation, and special effects video agents
- **Conversation History** — Retrieve prior conversation results from slide/poster agent sessions

### How it works

1. Subscribe to this server
2. Enter your Z.AI API key (create one at https://z.ai/manage-apikey/apikey-list)
3. Start generating content from Claude, Cursor, or any MCP-compatible client

Your AI acts as a gateway to the entire Z.AI multimodal AI platform — generate text, images, videos, transcribe audio, parse documents, and search the web without writing a single line of code.

### Who is this for?

- **Developers** — integrate Z.AI capabilities into your apps via natural language instead of reading API docs
- **Content Creators** — generate images, videos, and slides from text prompts directly in your AI chat
- **Data Teams** — transcribe audio, parse documents with OCR, and search the web for research
- **Product Teams** — prototype AI features quickly by asking your agent to call Z.AI APIs


## Available Tools (12)
- **agent_chat**: AI agents including: general_translation (multilingual translation with 40+ languages, auto-detection, glossary support), slides_glm_agent (one-click slide/poster generation from natural language), and vidu_template_agent (special effects video generation). Pass the full agent request body as JSON including agent_id and messages.

Run Z.AI agents for translation, slide generation, or poster creation
- **audio_transcription**: AI's ASR model. Supports .wav and .mp3 files up to 25MB and 30 seconds. Can provide hotwords for domain-specific vocabulary and context prompts for long-form transcription. Supports streaming output.

Transcribe audio files to text using the GLM-ASR-2512 model
- **chat_completion**: 2, GLM-4.7, or other available models. Supports multimodal inputs (text, images, audio, video, files), configurable parameters (temperature, max_tokens, tools), and both streaming and non-streaming modes. Pass the full request body as JSON including model, messages, and optional parameters.

Generate AI chat completions using Z.AI GLM models
- **get_conversation_history**: Only supports slides_glm_agent. Use the conversation_id from a prior agent_chat response.

Retrieve the conversation history for a Z.AI slide agent session
- **generate_image_async**: Use get_async_result with the task ID to check status and retrieve the generated image. Only supports glm-image model. Use this for long-running generation tasks.

Generate images asynchronously — returns a task ID for later retrieval
- **generate_image**: Returns image URLs (temporary, expire after 30 days). Specify model, prompt, and optional size/quality. GLM-Image recommended sizes: 1280x1280, 1568x1056, 1056x1568, 1472x1088, 1088x1472, 1728x960, 960x1728.

Generate high-quality images from text prompts using GLM-Image models
- **generate_video**: Supports text-to-video, image-to-video, and first/last frame-to-video. Returns a task ID — use get_async_result to check status and retrieve the video URL. Specify model, prompt, and optional quality/size/fps/duration.

Generate videos from text prompts or images using CogVideoX or Vidu models
- **get_async_result**: Returns task_status (PROCESSING, SUCCESS, FAIL) and the generated image or video URLs when complete. Use this after generate_image_async or generate_video returns a task ID.

Retrieve the result of an asynchronous image or video generation task
- **layout_parsing**: Returns recognized text in Markdown format, detailed layout information (bounding boxes for text, images, formulas, tables), and optional visualization results. Supports PDF, JPG, PNG formats. PDF up to 50MB/30 pages, images up to 10MB.

Parse document layouts and extract text using the GLM-OCR model
- **tokenize**: Returns prompt_tokens, image_tokens, video_tokens, and total_tokens. Useful for text length evaluation, model input estimation, context truncation, and cost calculation. Supports glm-4.6, glm-4.6v, and glm-4.5 models.

Count tokens for given messages using Z.AI models
- **web_reader**: Supports markdown and text output formats, cache control, image retention, and optional summaries for images and links.

Read and parse the content of a web page URL
- **web_search**: Supports filtering by domain whitelist and time range (oneDay, oneWeek, oneMonth, oneYear, noLimit). Returns up to 50 results per search.

Search the web using Z.AI's LLM-optimized search engine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Z.AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an image of a futuristic city with flying cars at sunset."

**🤖 AI Agent:**
> Generating image with GLM-Image model... Done! Here's your image: https://example.com/generated/image_001.png. The image shows a futuristic skyline with flying vehicles against a warm sunset sky. The temporary link expires in 30 days — would you like me to save it or generate variations?

---

**👤 You:**
> "Search the web for the latest news about AI breakthroughs in 2026."

**🤖 AI Agent:**
> Searching the web... Found 10 results. Top stories: 'OpenAI Announces GPT-6 with 10T Parameters' (TechCrunch), 'Z.AI Releases GLM-5.2 with Native Multimodal Support' (VentureBeat), and 'Google DeepMind Achieves AGI Milestone' (The Verge). Would you like me to read any of these articles in full?

---

**👤 You:**
> "Transcribe this audio recording and tell me what was said."

**🤖 AI Agent:**
> Transcribing audio with GLM-ASR-2512... The transcription is: 'Good morning everyone, today we'll be discussing the quarterly results and our roadmap for Q3. Please note that all projections are preliminary and subject to board approval.' The audio was 15 seconds long and detected as English. Would you like me to translate this to another language?


## ❓ FAQ

**Q: How do I get my Z.AI API key?**
Visit the [Z.AI API Keys page](https://z.ai/manage-apikey/apikey-list) to create or manage your API key. Once created, copy it and paste it into the API key field in the setup wizard. The key is used as a Bearer token in the Authorization header for all API requests.

**Q: Which Z.AI models are available?**
The MCP supports all Z.AI models: **GLM-5.2**, GLM-5.1, GLM-5-Turbo, GLM-4.7, GLM-4.7-flash, GLM-4.6, GLM-4.5 series for chat; **GLM-Image** and CogView-4 for image generation; **CogVideoX-3** and Vidu for video generation; **GLM-ASR-2512** for audio transcription; **GLM-OCR** for layout parsing; and **search-prime** for web search.

**Q: Can my AI generate images and videos?**
Yes! Use `generate_image` for synchronous image generation (returns URLs immediately), or `generate_image_async` for long-running tasks (returns a task ID — use `get_async_result` to retrieve). For video, use `generate_video` which always runs asynchronously — call `get_async_result` with the returned task ID to check status and get the video URL when complete.

**Q: Does the Z.AI MCP support multimodal inputs?**
Yes. The `chat_completion` tool supports multimodal inputs including text, images (image_url), video (video_url), and files (file_url) when using vision models like GLM-5V-Turbo. Pass the full messages array as JSON with the appropriate content types. The `layout_parsing` tool also supports both image and PDF inputs for OCR.

**Q: What is the base URL for Z.AI API calls?**
All Z.AI API calls are sent to `https://api.z.ai/api`. The engine automatically appends the correct path prefix (e.g. `/paas/v4/` for platform APIs, `/v1/` for agent APIs). When using the GLM Coding Plan, you may need to configure a dedicated endpoint — refer to the Z.AI documentation for details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zai](https://vinkius.com/mcp/zai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Z.AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Z.AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zai": {
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
