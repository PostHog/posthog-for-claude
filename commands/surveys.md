---
description: Manage PostHog surveys
argument-hint: [survey-name]
---

# Surveys

Use the PostHog MCP tools to help the user with survey management:

1. To list all surveys, use `posthog_get_all_surveys`
2. To get details about a specific survey, use `posthog_get_survey` with the survey ID
3. To view survey responses and statistics, use `posthog_get_survey_results`
4. To create a new survey, use `posthog_create_survey`
5. To update a survey, use `posthog_update_survey`
6. To launch or stop a survey, use the appropriate update action

## Example prompts

- "Show me all my surveys"
- "What are the responses to the NPS survey?"
- "Create a feedback survey for the checkout page"
- "How many people completed the onboarding survey?"
- "Stop the beta feedback survey"
