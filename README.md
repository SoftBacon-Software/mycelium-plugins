# Mycelium Plugins

Official plugin registry for [Mycelium](https://mycelium.fyi) — the distributed AI agent coordination platform.

## Available Plugins

### Integrations
- **GitHub Sync** — PR/issue sync, CI status, webhook receiver
- **Slack Bridge** — Bidirectional Slack messaging, slash commands, Discord support
- **Project Tracker Sync** — Linear/Jira bidirectional task sync

### Monitoring
- **Error Monitor** — Sentry/Bugsnag/Datadog webhook → auto-file bugs
- **Cost Tracker** — Token usage tracking, budget alerts, spend dashboards

### Governance
- **Guardrails** — Pre-action rule engine, violation log, enforcement modes

### Reporting
- **Daily Digest** — Automated swarm activity summaries

### Automation
- **Workflow Automations** — Event-driven "when X do Y" rules

### Marketing
- **Build in Public** — Auto-draft social content from milestones
- **Outreach** — YouTube discovery + personalized email campaigns
- **Social Posting** — Multi-platform social media publishing

### Content
- **Video Pipeline** — Video generation workflows
- **Steam Assets** — Steam store asset management

## For Developers

Each plugin ships with the Mycelium server in `server/plugins/`. Enable via the dashboard (Plugins page) or API.

See the [Plugin Guide](https://github.com/SoftBacon-Software/mycelium/blob/master/docs/plugin-guide.md) for building custom plugins.
