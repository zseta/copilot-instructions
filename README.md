# My list of copilot instructions & AI prompts
Within a VS Code project these should go in the `.github/instructions/copilot-instructions.md` file.

Otherwise, you can just copy-paste.

## Coding

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


## Text
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

### Tutorials / guides / docs
```md
Edit this markdown file. Check grammar. Finish sentences where neccessary.
Simplify complex phrases. No fluff.
For headings use sentence case. Add links where it's helpful.
Use "you" instead if "we" or "I".
For technical keywords, wrap it in `backticks`.
For code snippets, add the correct syntax highlight for the language.
```


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

## Random

### Starter FastAPI + AlpineJS + Tailwind
```
Run `uv init` in the current folder. Create a src/ folder and
build out a starter fastapi application in this folder.

To install stuff use uv add <package-name>.
Add a src/templates/ and src/static/ folder to FastAPI. Reference both folder relative to the main.py (which should also be in src folder) file.
Add index.html in templates and this html should include htmx alpinejs from CDN (use @latest version for both). Add tailwind from CDN.
Add static/js/app.js file with the following content:
function exampleApp() {
    return {
        count: 0,
        init() {
            console.log('App initialized');
        },
    };
}
Then reference this object in html using `x-data="exampleApp()`. And also include the js file in html of course.
Add a readme that contains minimal instructions how to install dependencies with `uv sync` and use `uv run src/main.py` as run instruction.
When done, activate the env with source .venv/bin/activate and run `python src/main.py` from the root project folder.
```
