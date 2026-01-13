# My list of copilot instructions & AI prompts
Within a VS Code project these should go in the `.github/instructions/copilot-instructions.md` file.

Otherwise, you can just copy-paste.

## General

### Chat session for docs with Context7
AlpineJS example:
```md
in this session use context7 /websites/alpinejs_dev for all responses
```
Go to https://context7.com for docs link. [Context7 MCP Server](https://marketplace.visualstudio.com/items?itemName=Upstash.context7-mcp) is needed.

### `.github/copilot-instructions.md`
Use [Context7 MCP Server](https://marketplace.visualstudio.com/items?itemName=Upstash.context7-mcp).
```md
* Always use Context7 MCP when I need library/API documentation, code generation, setup or configuration steps without me having to explicitly ask.
* When I ask for code snippets, ensure they are complete and functional, including the minimum code needed to run them.
* No fluff, be simple

```


### Text
```md
---
applyTo: '**/*.md'
---
No fluff, no emojis.
No emdash. Simple sentences.
Casual tone.
```

Optional:
```
For headings use sentence case. Short sentences.
```

## Agentic

### Technical content idea
```md
Help me create a new educational content idea in markdown format.
Use the following structure: The problem, possible solutions and approaches,
Recommendation or conclusion. Now I will give you the code snippets, notes,
or other information needed to generate this markdown. No fluff, no emojis.
No emdash. Simple, short sentences. Casual tone. For headings use sentence case.
Markdown should include metadata: relevant tags (max 3), status, today's date.
Create the file in ideas folder.
```
