# /posthog:insights

Query and analyze PostHog insights and analytics data.

## Instructions

Use the PostHog MCP tools to help the user with insights and analytics:

1. To list existing insights, use `posthog_get_all_insights`
2. To view a specific insight, use `posthog_get_insight` with the insight ID
3. To run a custom query, use `posthog_query_insight` or `posthog_run_query`
4. For natural language questions, use `posthog_generate_hogql_from_question` to convert to HogQL first
5. To create new insights, use `posthog_create_insight`

## Example prompts

- "Show me my top insights"
- "How many users signed up last week?"
- "What's the conversion rate for the checkout funnel?"
- "Create an insight showing daily active users"
- "Query pageviews by country for the last 30 days"
