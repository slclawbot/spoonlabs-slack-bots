# Slack Bot Experiment Repo

This repo holds manifests and setup for two Slack bots as part of the spoonlabs-ai experiment:
- dataKnife: General brainstorming and polling bot (add to ideation channels).
- systemFork: Task monitoring and status bot (add to project/lab channels).

## Manifests
- `dataknife-bot.json`: JSON manifest for the brainstorm/polling-focused bot.
- `systemfork-bot.json`: JSON manifest for the monitoring/helper bot.

Import these into Slack at https://api.slack.com/apps via "Create from an app manifest" (select JSON format). Based on Slack's Bolt Python AI Chatbot template for compatibility.

## Setup Notes
- After creation, install to workspace (OAuth & Permissions) and copy Bot User OAuth Token (xoxb-...) and App-Level Token (xapp-... with connections:write).
- Add bots to channels: `/invite @dataKnife` or `/invite @systemFork`.
- For running the bots: Use @slack/bolt-python (see https://github.com/slack-samples/bolt-python-ai-chatbot for inspiration). Set env vars: SLACK_BOT_TOKEN, SLACK_APP_TOKEN (for Socket Mode).
- Socket Mode enabled—no public URL needed. Events/interactivity via WebSocket.
- Test slash commands like /brainstorm after adding to channel.

Generated on 2026-02-27. For AI integration or custom backend, extend with Bolt framework.