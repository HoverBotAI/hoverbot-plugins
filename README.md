# HoverBot Agent Plugin

See what your chatbots could not answer. HoverBot is an AI chatbot platform that answers customer
questions from a company's own catalog, policies and documentation. This plugin connects AI
assistants to one HoverBot workspace through HoverBot's MCP server, so the people who run a support
bot can ask about it in plain language instead of reading dashboards.

## What it can do

- Find the questions your chatbot could not answer, and what to add to the knowledge base to close
  each gap.
- Read shopper conversations and full transcripts, and see which topics come up most.
- Search the chatbot's knowledge sources.
- See which customers are waiting for a person, and reply to them (opt-in, see below).
- List the leads your chatbots captured, and check usage against your plan.

Every tool is read-only unless you allow more while connecting: replying to customers and editing
question-and-answer pairs, text blocks and web links are each a separate box you tick. The plugin
cannot change a chatbot's settings or contact a lead.

The `hoverbot-escalations` skill tells the assistant how to handle customers waiting for a person,
including HoverBot alerts that start a run (for example a Grok Bot routine started by a HoverBot
webhook).

## Installation

### Cursor and Grok Bot

1. Open **Customize** in Cursor's sidebar, or **Connect apps** in Grok Bot.
2. Find **HoverBot** in the marketplace and select **Install**.
3. Connect HoverBot and sign in. Choose whether the assistant may also reply to customers.

Then ask, for example: "Which questions could my bot not answer this week?" or "Which customers are
waiting for a person?"

### Any other MCP client

Add a remote MCP server with the address `https://mcp.hoverbot.ai/mcp`. It signs in with OAuth and
registers the client on first use.

## Requirements

A HoverBot account with at least one chatbot: https://www.hoverbot.ai

## Privacy and access

Access is granted by signing in to HoverBot, and the grant fixes which workspace the plugin can read.
Every connection is listed in the HoverBot dashboard with the time it was last used, and revoking it
takes effect on the next request.

- Privacy policy: https://www.hoverbot.ai/privacy-policy
- Terms of service: https://www.hoverbot.ai/terms-of-service

## Support

- Guide: https://www.hoverbot.ai/guides/connect-ai-assistant
- Email: hi@hoverbot.ai

## License

MIT, see `LICENSE`. The license covers this plugin's files; the HoverBot service is governed by its
terms of service.
