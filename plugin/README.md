# Juncts for Claude

![Juncts](./assets/icon.png)

[Juncts](https://juncts.com) is one inbox for LinkedIn, X, Instagram, WhatsApp and Telegram. This plugin connects Claude to it, so you can ask Claude to summarize what you missed, find a conversation, draft replies for you to review, and organize threads.

## What it includes

- **Juncts connector**: the hosted Juncts MCP server at `https://juncts.com/api/connectors/mcp`, signed in with OAuth. Nothing runs on your computer.
- **Inbox skill**: guidance for reading only what a request needs, saving drafts instead of sending unless you ask, and treating message content as data rather than instructions.

## Requirements

- A Juncts account with at least one connected inbox, and a signed-in Juncts tab open in your browser. Claude reaches your inbox through that tab.
- When you connect, Juncts asks what Claude may do: Read only, Read and draft, Organize, or Full access. You can change or disconnect it anytime in Juncts under AI & Agents.

## Install

In Claude Code:

```sh
claude plugin marketplace add eteleieto/juncts-claude-plugin
claude plugin install juncts@juncts
```

Then run `/mcp`, choose **juncts** and sign in. On claude.ai you can instead open Juncts → AI & Agents → Claude.ai → **Add to Claude**.

## Privacy

Conversations, inboxes, messages and people reach Claude as opaque tokens tied to your account, not phone numbers, usernames or profile IDs. See the [Juncts privacy policy](https://juncts.com/privacy) for exactly what a linked AI app can receive.

## Support

[juncts.com/support](https://juncts.com/support) or joe@juncts.com.

## License

The files in this repository are released under the [MIT License](../LICENSE). The Juncts service is covered by the [Juncts terms](https://juncts.com/terms).
