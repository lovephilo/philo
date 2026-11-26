# Philo – A pure-Go coding agent with durable harness

- **Pure-Go coding harness.** `philo-tui` ships as a single `philo` binary for macOS and Linux. A shared background daemon keeps sessions and submitted tasks running when you close the terminal UI.
- **Remote work with Herdr.** Launch Philo in a Herdr workspace and see which agents are working or need your attention. Reconnect from another computer, phone, or tablet over SSH, including over Tailscale. Tap to select items or expand tool output, and swipe to scroll the conversation and results. [Herdr](https://herdr.dev/)
- **Models, routing, and shared resources with Magpie.** Pick Philo’s model in Magpie, route model requests through its gateway, and assign MCP servers and skills from its Library. Philo also supports direct provider configuration. [Magpie](https://usemagpie.ai/)
- **Built-in tools.** `find` locates files and directories with `.gitignore` support. `rg` searches file contents and paginates the results. `ls`, `read`, `write`, `edit`, and `bash` cover inspection, precise edits, and shell commands. `render_ui` offers interactive questions and choices. `codemode` composes tool calls in sandboxed JavaScript. The `bg_process` plugin exists in the codebase, and the default CLI leaves it unregistered.
- **Role-based subagents.** Delegate one task with `subagent`, or run independent tasks concurrently with `subagent_group` and collect the results together. A YAML role can set the tool list, turn budget, and context policy. The reviewer role starts with fresh context (`forkContext: never`), skips project instructions, has a 48-turn budget, and is instructed to find concrete regressions without editing files.
- **Go and JavaScript plugins, plus built-in skills.** Plugins can extend tools and terminal interactions, including slash commands and `@` references. `load_skill` loads guidance on demand, including built-in skills for software architecture, domain and interface design, and refactoring.

## Quick start
Install on macOS or Linux:

```sh
curl -fsSL https://philo.love/install.sh | sh
```

Download release artifacts from [Releases](https://github.com/lovephilo/philo/releases).

## Acknowledgments

**philo** is heavily inspired by [pi](https://pi.dev). Huge thanks to its creators and maintainers for pioneering such a thoughtful design and setting the bar so high.

- [pi](https://pi.dev)
- [alma](https://alma.now/)
- [mygo](https://mygo.run/)
- [charm_](https://charm.land/)
