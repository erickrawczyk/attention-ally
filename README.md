# Attention Ally

Documentation of building a custom GPT assistant focused on keeping you focused by managing Google Calendars and Todoist lists.

## Repository Structure

- **instructions-prompt**: Contains configuration details for setting up the initial GPT prompt.
- **todoist.yml**: Defines the action schemas for interacting with Todoist.

## Configuring a Custom GPT

To configure a custom GPT using the files in this repository, follow these steps:

- Visit [ChatGPT's Editor](https://chatgpt.com/gpts/editor) and create a new custom GPT.
- Add the content from the `prompt` file as your GPT's initial setup.
- Import `todoist.yml` using the GitHub raw URL: `https://raw.githubusercontent.com/erickrawczyk/attention-ally/main/todoist.yml` in the ChatGPT Builder Actions UI.
- Configure OAuth with Todoist:
  - Visit the [Todoist App Management Console](https://developer.todoist.com/appconsole.html).
  - Create an application and obtain the client ID and secret.
  - Set up the redirect URI for OAuth and ensure your application is authorized.

## Future Development

- **Google Calendar Integration**: Upcoming support for managing Google Calendars.

This README will be expanded as new features are added and more detailed documentation is created.
