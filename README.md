# Attention Ally

Documentation of building a custom GPT assistant focused on keeping you focused by managing Google Calendars and Todoist lists.

[![Live Demo](https://custom-icon-badges.demolab.com/badge/-Live%20Demo-blue?style=for-the-badge&logo=link-external&logoColor=white)](https://chatgpt.com/g/g-XmOKnlm7k-attention-ally)

## Repository Structure

- **instructions-prompt**: Contains configuration details for setting up the initial GPT prompt.
- **actions/todoist.yml**: Defines the action schemas for interacting with Todoist.
- **actions/google-calendar.yml**: Defines the action schemas for interacting with Google Calendar.

## Configuring a Custom GPT

To configure a custom GPT using the files in this repository, follow these steps:

- Visit [ChatGPT's Editor](https://chatgpt.com/gpts/editor) and create a new custom GPT.
- Add the content from the `instructions-prompt` file as your GPT's initial setup.
- Import `todoist.yml` using the GitHub raw URL: `https://raw.githubusercontent.com/erickrawczyk/attention-ally/main/todoist.yml` in the ChatGPT Builder Actions UI.
- Import `google-calendar.yml` using the GitHub raw URL: `https://raw.githubusercontent.com/erickrawczyk/attention-ally/main/google-calendar.yml` in the ChatGPT Builder Actions UI.
- Configure OAuth with Todoist:
  - Visit the [Todoist App Management Console](https://developer.todoist.com/appconsole.html).
  - Create an application and obtain the client ID and secret.
  - Set up the redirect URI for OAuth and ensure your application is authorized.
- Configure OAuth with Google Calendar:
  - Visit the [Google Cloud Console](https://console.cloud.google.com/).
  - Create or select a project and navigate to `APIs & Services` > `Credentials`.
  - Set up an OAuth 2.0 Client ID and note the client ID and secret.
  - Specify the necessary scopes (e.g., `https://www.googleapis.com/auth/calendar`, `https://www.googleapis.com/auth/calendar.events`).
