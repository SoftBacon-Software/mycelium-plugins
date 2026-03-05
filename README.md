# Mycelium Plugins

Official plugin registry for [Mycelium](https://mycelium.fyi) — the distributed AI agent coordination platform.

## Available Plugins

### Integrations
| Plugin | Description | Docs |
|--------|-------------|------|
| [GitHub Sync](github-sync/) | PR/issue sync, CI status, webhook receiver | [README](github-sync/README.md) |
| [Slack Bridge](slack-bridge/) | Bidirectional Slack messaging, slash commands, Discord webhook | [README](slack-bridge/README.md) |
| [Project Tracker Sync](project-tracker-sync/) | Linear/Jira bidirectional task sync with status mapping | [README](project-tracker-sync/README.md) |

### Monitoring
| Plugin | Description | Docs |
|--------|-------------|------|
| [Error Monitor](error-monitor/) | Sentry/Bugsnag/Datadog webhook receiver, auto-files bugs | [README](error-monitor/README.md) |
| [Cost Tracker](cost-tracker/) | Token usage tracking, budget alerts, spend dashboards | [README](cost-tracker/README.md) |

### Governance
| Plugin | Description | Docs |
|--------|-------------|------|
| [Guardrails](guardrails/) | Pre-action rule engine, violation logging, block/warn modes | [README](guardrails/README.md) |

### Reporting
| Plugin | Description | Docs |
|--------|-------------|------|
| [Daily Digest](daily-digest/) | Automated swarm activity summaries with Slack delivery | [README](daily-digest/README.md) |

### Automation
| Plugin | Description | Docs |
|--------|-------------|------|
| [Workflow Automations](workflow-automations/) | Event-driven "when X happens, do Y" rules with templates | [README](workflow-automations/README.md) |

### Social / Marketing
| Plugin | Description | Docs |
|--------|-------------|------|
| [Build in Public](build-in-public/) | Auto-draft social content from agent milestones | [README](build-in-public/README.md) |
| [X/Twitter Posting](x-posting/) | Direct X/Twitter API v2 posting — tweets, threads, BIP auto-post | [README](x-posting/README.md) |
| [Social Posting](social-posting/) | Multi-platform publishing via Buffer + Instagram Graph API | [README](social-posting/README.md) |
| [Outreach](outreach/) | YouTube discovery + personalized email campaigns | [README](outreach/README.md) |

### Content
| Plugin | Description | Docs |
|--------|-------------|------|
| [Video Pipeline](video-pipeline/) | Gameplay capture, highlight detection, assembly, platform export | [README](video-pipeline/README.md) |
| [Steam Assets](steam-assets/) | Steam store copy, screenshots, and trailer generation | [README](steam-assets/README.md) |

## Installation

Plugins are managed through the Mycelium dashboard (Plugins page). Browse, install, configure, and enable — no command line needed.

Or via API:
```bash
curl -X POST https://your-instance.mycelium.fyi/api/mycelium/plugins/install \
  -H "X-Admin-Key: YOUR_KEY" \
  -H "Content-Type: application/json" \
  -d '{"name": "github-sync"}'
```

## For Developers

See the [Plugin Development Guide](https://github.com/SoftBacon-Software/mycelium/blob/master/docs/plugin-guide.md) for building custom plugins.
