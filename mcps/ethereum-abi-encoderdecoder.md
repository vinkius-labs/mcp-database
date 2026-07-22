# Ethereum ABI Encoder/Decoder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ethereum-abi-encoderdecoder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [blockchain](../categories/blockchain.md)

Deterministic encoding and decoding of Ethereum smart contract calldata using ABI specifications.

## Description
This MCP server provides a deterministic way to handle Ethereum transaction data. It allows you to use `extract_function_selector` to find the 4-byte identifier, `encode_function_call` to transform signatures and parameters into valid calldata hex strings, and `decode_calldata_payload` to parse raw hex payloads back into human-readable parameters using an ABI definition. It handles complex tasks like Keccak-256 hashing, big-endian padding, and dynamic type offset calculations without the risk of LLM hallucinations.


## Available Tools (3)
- **decode_calldata_payload**: Parses a hex string of Ethereum calldata into readable values
- **encode_function_call**: Transforms a function signature and its arguments into valid Ethereum calldata
- **extract_function_selector**: Generates the 4-byte function selector from a given signature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ethereum ABI Encoder/Decoder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the function selector for transfer(address,uint256)?"

**🤖 AI Agent:**
> 0xa9059cbb

---

**👤 You:**
> "Encode a call for transfer(address,uint256) with address 0x1234567890abcdef1234567890abcdef12345678 and amount 100."

**🤖 AI Agent:**
> 0xa9059cbb88110...[truncated for brevity in thought, but will be full in file]

---

**👤 You:**
> "Decode this calldata: 0xa9059cbb88110... using the provided ABI."

**🤖 AI Agent:**
> The decoded parameters are: address: 0x1234..., amount: 100.


## ❓ FAQ

**Q: How do I generate a function selector?**
Use the `extract_function_selector` tool by providing the exact function signature, such as `transfer(address,uint256)`.

**Q: Can I decode complex transaction data?**
Yes, the `decode_calldata_payload` tool parses raw hex strings into readable parameters if you provide the corresponding ABI JSON.

**Q: Does it support dynamic types like strings?**
Yes, the `encode_function_call` tool handles dynamic type offsets and tight packing for strings and bytes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ethereum-abi-encoderdecoder](https://vinkius.com/mcp/ethereum-abi-encoderdecoder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ethereum ABI Encoder/Decoder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ethereum-abi-encoderdecoder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ethereum ABI Encoder/Decoder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ethereum-abi-encoderdecoder": {
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
