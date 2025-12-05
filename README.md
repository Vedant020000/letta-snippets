# Letta Snippets for VS Code

Code snippets for the Letta SDK (TypeScript & Python). Speed up development with stateful AI agents.

## Installation

Search "Letta Snippets" in VS Code Extensions

## Usage

Type a prefix and press `Tab`:

| Prefix      | Description                     |
| ----------- | ------------------------------- |
| `la-init`   | Initialize Letta client         |
| `la-create` | Create agent with memory blocks |
| `la-msg`    | Send message to agent           |
| `la-stream` | Stream agent response           |

## All Snippets

### Client

- `letta-client-init` / `la-init` - Cloud client
- `letta-client-self-hosted` / `la-local` - Self-hosted client

### Agents

- `letta-agent-create` / `la-create`
- `letta-agent-retrieve` / `la-get`
- `letta-agent-list` / `la-list`
- `letta-agent-modify` / `la-mod`
- `letta-agent-delete` / `la-del`

### Messages

- `letta-send-message` / `la-msg`
- `letta-send-message-stream` / `la-stream`
- `letta-messages-list` / `la-msgs`
- `letta-messages-reset` / `la-reset`

### Memory Blocks

- `letta-block-create` / `lab-create`
- `letta-block-attach` / `lab-attach`
- `letta-block-detach` / `lab-detach`
- `letta-block-list` / `lab-list`

### Folders & Files

- `letta-folder-create` / `laf-create`
- `letta-folder-attach` / `laf-attach`
- `letta-file-upload` / `laf-upload`
- `letta-file-delete` / `laf-del`

### Archives

- `letta-archive-create` / `laa-create`
- `letta-archive-attach` / `laa-attach`
- `letta-passage-create` / `laa-passage`

### Tools

- `letta-tool-create` / `lat-create`
- `letta-tool-attach` / `lat-attach`

## Links

- [Letta Docs](https://docs.letta.com)
- [TypeScript SDK](https://www.npmjs.com/package/@letta-ai/letta-client)
- [Python SDK](https://pypi.org/project/letta-client/)

## License

MIT
