---
description: Run HogQL queries and natural language analytics
argument-hint: [question or query]
---

# Query

Use the PostHog MCP tools to run HogQL queries and answer analytics questions:

1. For natural language questions, use `posthog_generate_hogql_from_question` to convert to HogQL
2. To run a HogQL query directly, use `posthog_run_query`
3. For complex analysis, combine multiple queries to build up the answer
4. Use `posthog_query_insight` to query data in the context of an existing insight

## HogQL Tips

- HogQL is PostHog's SQL-like query language
- Common tables: `events`, `persons`, `sessions`, `groups`
- Use `properties.$property_name` to access event properties
- Use `person.properties.$property_name` to access person properties

## Example prompts

- "How many users signed up last week?"
- "What's my most triggered event?"
- "Show me the top 10 pages by pageviews"
- "Run this query: SELECT count() FROM events WHERE event = 'purchase'"
- "What countries are my users from?"
