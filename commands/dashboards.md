---
description: Manage PostHog dashboards
argument-hint: [dashboard-name]
---

# Dashboards

Use the PostHog MCP tools to help the user with dashboard management:

1. To list all dashboards, use `posthog_get_all_dashboards`
2. To get details about a specific dashboard, use `posthog_get_dashboard` with the dashboard ID
3. To create a new dashboard, use `posthog_create_dashboard`
4. To update a dashboard, use `posthog_update_dashboard`
5. To add insights to a dashboard, use `posthog_add_insight_to_dashboard`
6. To delete a dashboard, confirm first then use `posthog_delete_dashboard`

## Example prompts

- "Show me all my dashboards"
- "What insights are on the Marketing dashboard?"
- "Create a new dashboard called Product Metrics"
- "Add the signup funnel insight to the Growth dashboard"
- "Rename my Sales dashboard to Revenue Overview"
