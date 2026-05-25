# AI Playground

A repository for AI experiments. Each experiment lives in its own folder at the root level.

## Project Structure

```
ai_playground/
├── index.html             # Landing page (GitHub Pages)
├── AGENTS.md              # This file
├── .vscode/               # Editor settings
├── <experiment-name>/     # Individual experiment folder
├── ...
```

## Creating a New Experiment

1. Create a new folder at the root level with a descriptive name (e.g., `prompt-chaining`, `rag-prototype`, `agent-simulation`)
2. Inside the folder, include at minimum:
   - `README.md` – describe the experiment's goal, setup, and results
   - Source code / scripts for the experiment
3. Keep experiments self-contained so they can be run independently

## Guidelines

- **One experiment per folder** – don't mix unrelated experiments
- **Self-documenting** – each folder should have a README explaining what the experiment tests and how to run it
- **Clean and isolated** – avoid shared dependencies between experiments where possible
- **Iterate in place** – improvements to an experiment stay in its folder
- **Update index.html** – when creating a new experiment, add a link to it in the root `index.html` landing page so it appears on GitHub Pages
- **High quality deliverables** – no shortcuts. Deliver polished, well-crafted work.
- **Never commit or push** – only commit or push changes when the user explicitly asks for it
- **Validate with Playwright** – after building a web experiment, test it in the browser:
  - Serve with `npx --yes serve -p <port>` from the project root
  - Navigate to the experiment URL and verify it loads and works
  - Check console messages with `playwright_browser_console_messages` for errors
  - Take screenshots to visually confirm rendering
  - Clean up all Playwright artifacts (`.playwright-mcp/`, screenshots) before finishing
