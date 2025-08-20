# AI Dev Agent: Langfuse Prompt MCP Guide

## Purpose
This MCP server provides access to production-labeled prompt templates stored in Langfuse. Use it to retrieve and apply standardized prompts instead of copy/pasting into CLI.

## Available Tools

### `get-prompts`
Lists all available production prompts with pagination. Use to discover available templates.

### `get-prompt`
Retrieves specific prompt by name with variable substitution. Pass arguments as JSON object for template variables.

## When to Use
- Need standardized prompt templates for consistent AI interactions
- Want to manage prompts collaboratively through Langfuse UI
- Replacing manual copy/paste of common prompts
- Ensuring version-controlled prompt management

## Configuration Path
`/home/nole/dev/shared/mcp-servers/langfuse/build/index.js`

## Example Usage
1. `get-prompts` → discover available templates
2. `get-prompt` with name="code-review" and arguments={"language":"python"} → get compiled code review prompt