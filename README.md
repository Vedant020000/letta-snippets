# Letta SDK Snippets

<div align="center">
<img src="https://raw.githubusercontent.com/Vedant020000/letta-snippets/refs/heads/master/images/preview.png" alt="Letta SDK Snippets Preview" width="100%" />

**Speed up your AI agent development with 30+ snippets for the Letta SDK.**

</div>

## 🚀 Features

- **⚡ Fast Coding**: Use short aliases like `la-create` to generate complex agent configurations instantly.
- **🛡️ Type Safe**: Snippets include TypeScript interfaces and Python type hints matching SDK v1.0.
- **🌍 Multi-Language**: Full support for both **TypeScript** (`@letta-ai/letta-client`) and **Python** (`letta`).
- **🧠 Comprehensive**: Covers Agents, Memory Blocks, Messaging, Archival Storage, and Tools.

## 📦 Installation

Open VS Code and search for **"Letta SDK Snippets"** in the Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X`).

## ⚡ Snippet Cheatsheet

Type the **Prefix** or **Alias** and press `Tab` to insert the snippet.

### 🤖 Agent Management

| Operation           | Full Prefix                  | Short Alias | Description                           |
| :------------------ | :--------------------------- | :---------- | :------------------------------------ |
| **Create Agent**    | `letta-agent-create`         | `la-create` | Create new agent with memory & models |
| **Create (Simple)** | `letta-agent-create-minimal` | `la-quick`  | Minimal agent creation                |
| **Get Agent**       | `letta-agent-retrieve`       | `la-get`    | Retrieve agent details by ID          |
| **List Agents**     | `letta-agent-list`           | `la-list`   | List all agents (paginated)           |
| **Update Agent**    | `letta-agent-modify`         | `la-mod`    | Modify system prompt or models        |
| **Delete Agent**    | `letta-agent-delete`         | `la-del`    | Delete an agent                       |

### 💬 Messaging

| Operation          | Full Prefix                        | Short Alias    | Description                   |
| :----------------- | :--------------------------------- | :------------- | :---------------------------- |
| **Send Message**   | `letta-send-message`               | `la-msg`       | Send user message to agent    |
| **Stream Message** | `letta-send-message-stream`        | `la-stream`    | Stream agent response (SSE)   |
| **With Identity**  | `letta-send-message-with-identity` | `la-msg-id`    | Send message as specific user |
| **List Messages**  | `letta-messages-list`              | `la-msg-list`  | Get conversation history      |
| **Clear History**  | `letta-messages-reset`             | `la-msg-reset` | Wipe agent context window     |

### 🧠 Memory & Storage

| Operation          | Full Prefix            | Short Alias  | Description                    |
| :----------------- | :--------------------- | :----------- | :----------------------------- |
| **Create Block**   | `letta-block-create`   | `lab-create` | Create reusable memory block   |
| **Attach Block**   | `letta-block-attach`   | `lab-attach` | Add block to agent core memory |
| **Create Archive** | `letta-archive-create` | `laa-create` | Create semantic vector store   |
| **Add Passage**    | `letta-passage-create` | `laa-add`    | Add text to semantic memory    |
| **Create Folder**  | `letta-folder-create`  | `laf-create` | Create file storage folder     |
| **Upload File**    | `letta-file-upload`    | `laf-upload` | Upload document to folder      |

### 🛠️ Client & Tools

| Operation           | Full Prefix                | Short Alias   | Description                   |
| :------------------ | :------------------------- | :------------ | :---------------------------- |
| **Init Client**     | `letta-client-init`        | `la-init`     | Initialize Cloud client       |
| **Init Local**      | `letta-client-self-hosted` | `la-local`    | Initialize Self-hosted client |
| **Create Tool**     | `letta-tool-create`        | `lat-create`  | Define custom Python tool     |
| **Create Identity** | `letta-identity-create`    | `la-identity` | Create user identity profile  |

## 📝 Example Usage

### TypeScript

```typescript
// Type 'la-init'
const client = new LettaClient({
  apiKey: "YOUR_API_KEY",
  projectId: "YOUR_PROJECT_ID",
});

// Type 'la-create'
const agent = await client.agents.create({
  name: "support-bot",
  memory_blocks: [
    { label: "persona", value: "You are a helpful support agent." },
  ],
  model: "openai/gpt-4",
});
```

### Python

```python
# Type 'la-init'
client = LettaClient(
    api_key='YOUR_API_KEY',
    project_id='YOUR_PROJECT_ID'
)

# Type 'la-create'
agent = client.agents.create(
    name='support-bot',
    memory_blocks=[
        {'label': 'persona', 'value': 'You are a helpful support agent.'}
    ],
    model='openai/gpt-4'
)
```

## 🔧 Requirements

This extension contains snippets only. You must install the Letta SDK separately:

**Node.js / TypeScript**

```bash
npm install @letta-ai/letta-client
```

**Python**

```bash
pip install letta
```

## 🤝 Contributing

Issues and pull requests are welcome! Please check the [GitHub repository](https://github.com/Vedant020000/letta-snippets) for contribution guidelines.

## 📄 License

MIT License © 2025

Made With ❤️ By [Vedant0200](https://github.com/Vedant0200)
