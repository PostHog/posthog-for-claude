# PostHog for Claude

Official PostHog plugin for Claude Code. Access your analytics, feature flags, experiments, and error tracking directly from Claude.

## Installation

### From Claude Code

```bash
claude plugin install posthog
```

### Manual installation

1. Clone and install the plugin:
```bash
git clone https://github.com/PostHog/posthog-for-claude
claude --plugin-dir ./posthog-for-claude
```

2. Authenticate via OAuth:
```
/mcp
```
Then follow the browser prompts to log in to PostHog.

## Features

This plugin provides access to 27+ PostHog tools across these categories:

- **Feature flags** - Create, update, and manage feature flags
- **Experiments** - Run and analyze A/B tests
- **Insights** - Query analytics and create visualizations
- **Dashboards** - Manage dashboards and add insights
- **Error tracking** - View and debug errors
- **LLM analytics** - Track AI/LLM costs and usage
- **Documentation** - Search PostHog docs

## Slash Commands

- `/posthog:flags` - Manage feature flags
- `/posthog:insights` - Query analytics data
- `/posthog:errors` - View error tracking data

## Example Usage

```
> What feature flags do I have?
> Show me errors from the last 24 hours
> How many users signed up this week?
> Create a feature flag for the new checkout flow
> What are my LLM costs this month?
```

## EU Cloud

If your PostHog project is on EU Cloud, the MCP server will automatically detect this based on your API key.

## Self-hosted

For self-hosted PostHog instances, set the `POSTHOG_BASE_URL` environment variable:

```bash
export POSTHOG_BASE_URL="https://posthog.example.com"
```

## Documentation

- [PostHog MCP documentation](https://posthog.com/docs/model-context-protocol)
- [PostHog API documentation](https://posthog.com/docs/api)

## License

MIT
