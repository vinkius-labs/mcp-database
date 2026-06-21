# Conda (Anaconda.org) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conda-anacondaorg)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Enable your AI agent to search packages, inspect metadata, and explore channels on Anaconda.org via the Conda API.

## Description
Connect your AI assistant to **Conda** (Anaconda.org), the open-source package and environment management ecosystem. Query package registries, inspect version metadata, and explore community channels — all from your AI chat.

### What you can do

- **Package Search** — Find any package across Anaconda.org by name, version, or platform compatibility.
- **Metadata Inspection** — Retrieve detailed information about a specific package including dependencies, maintainers, and download stats.
- **Channel Exploration** — Browse packages available in community channels like conda-forge and filter by Python version or platform.

### How it works

1. Add the Conda integration to your AI toolset.
2. Optionally provide an Anaconda API Token for access to private channels.
3. Search and explore the entire conda ecosystem via natural language.

### Who is this for?

- **Data Scientists** — Quickly check if a package version supports their Python environment before installing.
- **ML Engineers** — Discover package dependencies and compatibility without leaving their IDE.
- **DevOps Teams** — Audit which package versions are available before updating environment specs.


## Available Tools
- **search_conda_forge**: Quickly search for packages in the conda-forge channel
- **get_latest_package_version**: Retrieve the latest version string for a specific package
- **get_package_details**: Retrieve detailed information about a specific package
- **get_anaconda_user**: Retrieve profile details of the authenticated Anaconda user
- **list_my_organizations**: Retrieve a list of organizations (channels) you belong to
- **list_package_files**: Retrieve a list of distributions (files) for a specific package
- **list_user_packages**: Retrieve a list of packages owned by a specific user or channel
- **search_conda_packages**: Search for packages on Anaconda.org (Conda Cloud)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conda (Anaconda.org)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'numpy' packages on Anaconda.org."

**🤖 AI Agent:**
> I found 15 results for 'numpy' on Anaconda.org. The top results are:
1. anaconda/numpy — v1.26.4 (542M downloads)
2. conda-forge/numpy — v1.26.4 (380M downloads)
3. anaconda/numpy-base — v1.26.4
Would you like detailed info on any of these?

---

**👤 You:**
> "Show detailed info for package 'pandas' owned by 'anaconda'."

**🤖 AI Agent:**
> Package: **pandas** (anaconda)
- Latest: v2.2.1
- License: BSD-3-Clause
- Platforms: linux-64, osx-64, win-64, osx-arm64
- Dependencies: python >=3.9, numpy >=1.22, python-dateutil >=2.8.2
- Downloads: 285M total
Need anything else about this package?

---

**👤 You:**
> "Check what packages are available in the 'pytorch' channel."

**🤖 AI Agent:**
> The 'pytorch' channel contains 32 packages. The most downloaded are:
1. pytorch (95M downloads)
2. torchvision (48M downloads)
3. torchaudio (22M downloads)
Shall I list the dependencies for 'pytorch'?


## ❓ FAQ

**Q: How do I get an Anaconda API token?**
You can generate a token using the Anaconda CLI (`anaconda auth --create`) or in your profile settings on anaconda.org.

**Q: Can I install packages using this server?**
No. This integration queries the Anaconda.org API for metadata only. To install packages, use `conda` or `mamba` CLI locally.

**Q: What is conda-forge?**
Conda-forge is a community-led collection of recipes, build infrastructure, and distributions for the conda package manager. It's the largest community channel on Anaconda.org.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conda-anacondaorg](https://vinkius.com/mcp/conda-anacondaorg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conda (Anaconda.org)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `conda-anacondaorg` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conda (Anaconda.org)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conda-anacondaorg": {
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
