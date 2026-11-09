---
name: wavelength-call-to-flow
description: Turn discovery call notes or a meeting transcript into a Wavelength process flow, then suggest follow-up questions. Use when the user pastes call notes, a transcript, or meeting notes and wants a process map.
---

# Turn a call into a process flow

## Setup

This skill uses the Wavelength MCP server. If the Wavelength tools are not available, tell the user to add this remote MCP server and sign in with OAuth:

- URL: https://wavelengthflow.com/api/mcp
- Transport: Streamable HTTP
- Auth: OAuth (the client opens a Wavelength sign-in page)

A free Wavelength account works. Sign up at https://wavelengthflow.com.

## Steps

1. Read the notes or the transcript that the user gives.
2. Call notes_to_flow with the text. Keep the speaker's own terms for steps and systems.
3. Show the flow and give the link.
4. If the notes have gaps, call suggest_followups and list the questions for the next call.
5. Do not invent steps, owners, or systems that are not in the notes.
