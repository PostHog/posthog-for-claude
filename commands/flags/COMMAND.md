# /posthog:flags

List and manage feature flags in your PostHog project.

## Instructions

Use the PostHog MCP tools to help the user with feature flags:

1. First, call `posthog_get_all_feature_flags` to list all feature flags in the active project
2. If the user asks about a specific flag, use `posthog_get_feature_flag_definition` with the flag key
3. If the user wants to create a flag, use `posthog_create_feature_flag`
4. If the user wants to update a flag, use `posthog_update_feature_flag`
5. If the user wants to delete a flag, confirm first then use `posthog_delete_feature_flag`

## Example prompts

- "Show me all my feature flags"
- "What's the status of the beta-dashboard flag?"
- "Create a new flag called new-onboarding for 50% of users"
- "Turn off the old-checkout flag"
