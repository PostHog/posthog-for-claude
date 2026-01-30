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

- `/posthog:flags` - List and manage feature flags
- `/posthog:insights` - Query analytics and create visualizations
- `/posthog:errors` - View and debug error tracking data
- `/posthog:experiments` - Manage A/B testing experiments
- `/posthog:dashboards` - Create and manage dashboards
- `/posthog:surveys` - Create and manage user surveys
- `/posthog:query` - Run HogQL queries and natural language analytics
- `/posthog:logs` - Query application logs
- `/posthog:llm-analytics` - Track AI/LLM costs and usage
- `/posthog:docs` - Search PostHog documentation
- `/posthog:actions` - Manage PostHog actions
- `/posthog:search` - Search across all PostHog entities
- `/posthog:workspace` - Manage organizations and projects

## Example Usage

```
> What feature flags do I have?
> Create a feature flag called new-onboarding for 50% of users

> Show me errors from the last 24 hours
> Which errors are affecting the most users?

> How many users signed up this week?
> What's the conversion rate for the checkout funnel?

> Show me all my experiments
> What are the results of the checkout-flow experiment?

> Create a new dashboard called Product Metrics
> Add the signup funnel insight to the Growth dashboard

> What are the responses to the NPS survey?
> Create a feedback survey for the checkout page

> What's my most triggered event?
> Show me the top 10 pages by pageviews
```

## EU Cloud

If your PostHog project is on EU Cloud, set the `POSTHOG_MCP_URL` environment variable:

```bash
# Add to your ~/.zshrc or ~/.bashrc
export POSTHOG_MCP_URL="https://mcp-eu.posthog.com/mcp"
```

Then restart Claude Code or open a new terminal session.

> **Note:** The `?region=eu` query parameter does not work due to a [known Claude Code OAuth issue](https://github.com/anthropics/claude-code/issues/2034). You must use the `mcp-eu.posthog.com` subdomain instead.

## Self-hosted

For self-hosted PostHog instances, set the `POSTHOG_MCP_URL` environment variable to point to your instance:

```bash
export POSTHOG_MCP_URL="https://mcp.your-posthog-instance.com/mcp"
```

## Documentation

- [PostHog MCP documentation](https://posthog.com/docs/model-context-protocol)
- [PostHog API documentation](https://posthog.com/docs/api)

## License

MIT
