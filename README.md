# tannerorourke plugins

Curated set of plugins designed and developed by Tanner O'Rourke. All our supported on the Claude Code plugin marketplace, working on extending functionality to Codex and beyond.

## Plugins

| Name | What it does | Repository |
| --- | --- | --- |
| `pnw-outdoor-planner` | Researches a Pacific Northwest outdoor trip across six factor agents and returns a sourced go/no-go verdict. Weather and avalanche risk skills are available on their own. | [tannerorourke/pnw-outdoor-planner](https://github.com/tannerorourke/pnw-outdoor-planner) |
| `shopping-research` | A suite of tools and skills for finding the best product price. Product search, cross-retailer prices, Amazon price history, and community deals over free sources, with self-reported coverage on every call. Runs a local MCP server in order to utilize a Chromium window to get CamelCamelCamel price history (requires `uv`). The plugin carries the server and the skill for Claude Code; the Claude Desktop app takes the server from the repository's `.mcpb` bundle. | [tannerorourke/shopping-research-mcp](https://github.com/tannerorourke/shopping-research-mcp) |

## Installation

Add the marketplace once, then install any plugin from it:

```bash
claude plugin marketplace add tannerorourke/plugins
claude plugin install pnw-outdoor-planner@tannerorourke
claude plugin install shopping-research@tannerorourke
```

Pull new entries and versions, then validate with:

```bash
claude plugin marketplace update tannerorourke  # pull new entries
claude plugin validate .                        # validate plugins
```

> **Note on availability:** On Claude Desktop, plugins with local MCP servers take their tools from the `.mcpb` bundle in the plugin's repository, with keys entered under Settings $\rightarrow$ Extensions. Their skills still come from this marketplace; without one, the bundle's server carries only its essential instructions.
>
> On claude.ai, find the plugins tab in the lefrt sidebar (it changes) $\rightarrow$ Add $\rightarrow$ Add marketplace $\rightarrow$ enter `tannerorourke/plugins`. Skills load in chat in a browser or on a phone, with no local tools to call. Agents, hooks, and local MCP servers run only in Claude Code and Cowork.

## License

Each listed plugin carries its own MIT license.
