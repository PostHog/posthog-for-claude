---
description: Manage PostHog A/B testing experiments
argument-hint: [experiment-name]
---

# Experiments

Use the PostHog MCP tools to help the user with A/B testing experiments:

1. To list all experiments, use `posthog_get_all_experiments`
2. To get details about a specific experiment, use `posthog_get_experiment` with the experiment ID
3. To view experiment results and statistical significance, use `posthog_get_experiment_results`
4. To create a new experiment, use `posthog_create_experiment`
5. To update an experiment, use `posthog_update_experiment`
6. To launch or stop an experiment, use the appropriate update action

## Example prompts

- "Show me all my experiments"
- "What are the results of the checkout-flow experiment?"
- "Create an A/B test for the new pricing page"
- "Which variant is winning in the signup-button experiment?"
- "Stop the homepage-hero experiment"
