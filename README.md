# Slack Bot Experiment Repo

This repo holds manifests and setup for two Slack bots as part of the spoonlabs-ai experiment:
- One for project ideation (#all-spoonlabs-ai channel).
- One for overnight/lab project updates (#lab-v001 channel).

## Manifests
- `project-ideator-bot.json`: JSON manifest for the ideation bot.
- `overnight-helper-bot.json`: JSON manifest for the lab/overnight bot.

Import these into Slack at https://api.slack.com/apps via "Create from an app manifest" (select JSON format).

## Setup Notes
- Duplicate and tweak scopes/names as needed.
- After creation, install to workspace and add bots to channels with `/invite @BotName`.
- For event handling, set up a server or use Socket Mode.

Generated on 2026-02-27.