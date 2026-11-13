# tannerorourke plugins

Claude Code plugin marketplace, all products designed and developed by Tanner O'Rourke.

## Plugins

| Name | What it does | Repository |
| --- | --- | --- |
| `pnw-outdoor-planner` | Researches a Pacific Northwest outdoor trip across six factor agents and returns a sourced go/no-go verdict, with weather and avalanche skills usable on their own. | [tannerorourke/pnw-outdoor-planner](https://github.com/tannerorourke/pnw-outdoor-planner) |
| `tre` | Runs a three-agent ML research lab (Research Scientist, Tech Lead, Developer) over a git repository: start workflow runs, watch them to their exit line, and answer human gates. Its local MCP server needs `uv` on PATH. | [tannerorourke/tre-the-research-team](https://github.com/tannerorourke/tre-the-research-team) |

## Installation

Add the marketplace once, then install any plugin from it:

```bash
claude plugin marketplace add tannerorourke/plugins
claude plugin install pnw-outdoor-planner@tannerorourke
```

On claude.ai, Settings $\rightarrow$ Plugins $\rightarrow$ Add, $\rightarrow$ Add marketplace, enter `tannerorourke/plugins`. Skills from the plugin load in chat; agents, hooks, and local MCP servers run only in Claude Code and Cowork.

Pull new entries and versions, then validate with:

```bash
claude plugin marketplace update tannerorourke  # pull new entries
claude plugin validate .                        # validate plugins
```

## License

Each listed plugin carries its own MIT license.
