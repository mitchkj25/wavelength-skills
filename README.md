# Wavelength agent skills

Agent skills for [Wavelength](https://wavelengthflow.com). Wavelength turns sales calls, meeting notes, and code into live, editable process flow diagrams.

## Install

```bash
npx skills add mitchkj25/wavelength-skills
```

The skills work with Claude Code, Cursor, Codex, Gemini CLI, and other agents that read SKILL.md files.

## Connect the Wavelength MCP server

The skills call the Wavelength MCP server. Add it to your agent:

- URL: `https://wavelengthflow.com/api/mcp`
- Transport: Streamable HTTP
- Auth: OAuth. Your client opens a Wavelength sign-in page.

Claude Code example:

```bash
claude mcp add --transport http wavelength https://wavelengthflow.com/api/mcp
```

## Skills

| Skill | What it does |
| --- | --- |
| wavelength-get-started | Introduces Wavelength and makes a first flow. |
| wavelength-call-to-flow | Turns call notes or a transcript into a flow and suggests follow-up questions. |
| wavelength-map-a-process | Maps, changes, or exports a business process. |
| wavelength-send-to-tools | Sends a flow to Jira, Confluence, Notion, Salesforce, ServiceNow, HubSpot, Google Drive, or a chat channel. |
| wavelength-map-code-to-flow | Maps a function, service, or pipeline in a repo as a flow. |
| wavelength-update-flow-from-code | Updates a saved flow after the code changes. |

## Links

- Website: https://wavelengthflow.com
- MCP docs: https://wavelengthflow.com/mcp.html
- Support: support@wavelengthflow.com

## License

MIT
