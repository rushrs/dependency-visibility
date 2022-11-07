# Raising Dependency Visiblity

## Usage

You can copy the workflows found in `dependency-visibility/examples` to your .github/workflows folder within your repo. You need to update the `create-jira-ticket-on-pr-open.yaml` on lines 20 and 21 to include your Project name and an appropraite issue type respectively.

These actions require the following secrets set on the github repository.
- JIRA_BASE_URL
- JIRA_USER_EMAIL
- JIRA_API_TOKEN

The values of which can be produced from your Atlassian account in the developer settings.

Note that there is scope to remove the use of User API tokens and authenticate with App tokens but it that authentication method is still a WIP - feel free to PR the solution in.
