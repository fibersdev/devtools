# fibersdev plugins

A Claude Code plugin marketplace: small open-source plugins from the team behind [fibers](https://github.com/fibersdev), a board that shows which coding-agent sessions are running where.

Add the marketplace once, then install whichever plugins you want.

## Plugins

- **[storybook-preview-mcp-app](https://github.com/fibersdev/storybook-preview-mcp-app)** shows a Storybook story live in the chat, with your project's real CSS, fonts and Storybook decorators, without a Storybook dev server running. The preview is an MCP App, a small page Claude can draw inside the chat. For Storybook 10 with React and Vite.

Each plugin has a separate repository for its code, tests and issues. This repository is the list.

## Install

In a Claude Code terminal session, add the marketplace, then install a plugin from it (storybook-preview-mcp-app here):

```
/plugin marketplace add fibersdev/plugins
/plugin install storybook-preview-mcp-app@fibersdev
```

Or from a shell:

```bash
claude plugin marketplace add fibersdev/plugins
claude plugin install storybook-preview-mcp-app@fibersdev
```

In the Claude desktop app (as of November 2026): click + next to the prompt box, then Plugins, Add marketplace with `fibersdev/plugins`, then pick a plugin.

## Adding a plugin

Add an entry to `.claude-plugin/marketplace.json` that points at the plugin's repository, then run `claude plugin validate .` before opening a pull request.

MIT licence.
