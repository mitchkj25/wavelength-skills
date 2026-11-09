---
name: wavelength-get-started
description: Introduce Wavelength and help a new user make their first process flow. Use when the user first connects Wavelength or asks what Wavelength can do.
---

# Get started with Wavelength

## Setup

This skill uses the Wavelength MCP server. If the Wavelength tools are not available, tell the user to add this remote MCP server and sign in with OAuth:

- URL: https://wavelengthflow.com/api/mcp
- Transport: Streamable HTTP
- Auth: OAuth (the client opens a Wavelength sign-in page)

A free Wavelength account works. Sign up at https://wavelengthflow.com.

## Steps

1. Tell the user in one or two sentences that Wavelength turns calls, notes, and descriptions into editable process flow diagrams.
2. Ask the user for a process to map, or offer an example such as "Map our invoice approval process."
3. When the user gives a process, call create_flow_from_text with the description.
4. Show the flow and give the link that the tool returns.
5. Tell the user that they can ask to change steps, summarize the flow, or export it as Mermaid.
