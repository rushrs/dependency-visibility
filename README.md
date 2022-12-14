# Increasing Dependency Visiblity

Associated medium article can be found [here](https://rushrs.medium.com/increasing-visibility-for-code-dependencies-1238efb97df6) - outlining how i've implemented these practices at RVU and the benefits it's brought to my team and the wider organisation
## Usage

You can copy the workflows found in `dependency-visibility/examples` to your .github/workflows folder within your repo. You need to update the `create-jira-ticket-on-pr-open.yaml` on lines `20` and `21` to include your JIRA Project name and an appropriate JIRA Issue type respectively.

These actions require the following secrets set on the github repository.
- JIRA_BASE_URL
- JIRA_USER_EMAIL
- JIRA_API_TOKEN

The values of which can be produced from your Atlassian account in the developer settings.

Note that there is scope to remove the use of User API tokens and authenticate with App tokens but it that authentication method is still a WIP - feel free to PR the solution in.
