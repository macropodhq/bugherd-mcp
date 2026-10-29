# Official BugHerd MCP

Connect [BugHerd](https://bugherd.com) to your AI coding assistant via MCP (Model Context Protocol) so you can work with projects and tasks directly from your AI tool.

This repo is maintained by the [BugHerd](https://bugherd.com) core team and will updated with the most recent links & guides for using the BugHerd MCP.

## What is BugHerd MCP?

[BugHerd MCP](https://bugherd.com) is a remote MCP server that gives AI assistants secure access to BugHerd project/task workflows.

Once connected, you can use your AI tool to help with common operations like:

- Listing projects and tasks
- Creating and updating tasks
- Adding comments
- Managing assignees, tags, and attachments
- Creatign & updating project details

To find out more, read the [Getting Started Guide](https://support.bugherd.com/en/articles/14835206-getting-started-with-the-bugherd-mcp-server), or checkout the **Install Guides** below.

## Quick Start

1. Choose your AI tool from the list below.
2. Follow the BugHerd install guide for that tool.
3. Authenticate with your BugHerd account and authorize access.
4. Start using BugHerd MCP tools from your AI workflow.

## Supported AI Tools + Install Guides

Use the guide for your preferred client:

- [Claude Code](https://support.bugherd.com/articles/14835255-bugherd-and-claude-code-set-up-the-mcp-server)
- [Claude.ai](https://support.bugherd.com/articles/14835961-bugherd-and-claude-ai-set-up-the-mcp-server)
- [ChatGPT](https://support.bugherd.com/articles/14835258-bugherd-and-chatgpt-set-up-the-mcp-server)
- [Codex CLI](https://support.bugherd.com/articles/14835262-bugherd-and-codex-cli-set-up-the-mcp-server)
- [Cursor](https://support.bugherd.com/articles/14835263-bugherd-and-cursor-set-up-the-mcp-server)
- [Gemini CLI](https://support.bugherd.com/articles/14835265-bugherd-and-gemini-cli-set-up-the-mcp-server)
- [VS Code/GitHub Copilot](https://support.bugherd.com/articles/14835268-bugherd-and-vs-code-copilot-set-up-the-mcp-server)
- [Windsurf](https://support.bugherd.com/articles/14835272-bugherd-and-windsurf-set-up-the-mcp-server)
- [Zed](https://support.bugherd.com/articles/14835274-bugherd-and-zed-set-up-the-mcp-server)
- [Antigravity](https://support.bugherd.com/articles/15092969-bugherd-and-antigravity-integration)
- [Cline](https://support.bugherd.com/articles/14835261-bugherd-and-cline-set-up-the-mcp-server)
- [Other AI Tools](https://support.bugherd.com/articles/14835255-bugherd-and-other-ai-tools-set-up-the-mcp-server)


## Agent Skills

The [`skills/`](skills) folder contains [Agent Skills](https://agentskills.io) that teach your AI tool how to get the most out of the BugHerd MCP:

| Skill | Helps your agent |
|---|---|
| [`bugherd-basics`](skills/bugherd-basics/SKILL.md) | Find the right project, and understand websites, design assets, members, clients and share links |
| [`bugherd-reading-tasks`](skills/bugherd-reading-tasks/SKILL.md) | Understand a task: the issue, the page, the element, the screenshot and attachments |
| [`bugherd-creating-feedback`](skills/bugherd-creating-feedback/SKILL.md) | Create feedback from reviews and checklists, including pinned feedback with screenshots |
| [`bugherd-triage`](skills/bugherd-triage/SKILL.md) | Review and organise feedback: statuses, assignees, tags, and flagging what needs a person |
| [`bugherd-fix-with-review`](skills/bugherd-fix-with-review/SKILL.md) | Take feedback through to a code fix, with you approving each step |
| [`bugherd-reporting`](skills/bugherd-reporting/SKILL.md) | Summarise activity for standups and client meetings |

### Install the skills

Ask your AI tool:

> Install the BugHerd agent skills from https://github.com/macropodhq/bugherd-mcp. Copy each folder inside `skills/` into your skills folder, keeping the folder names and files as they are.

Or copy the folders inside `skills/` yourself:

- **Claude Code:** `~/.claude/skills/` for all projects, or `.claude/skills/` in one project.
- **Cursor:** install the BugHerd plugin, which includes the skills, or copy them to `~/.cursor/skills/`.
- **Other tools:** check your tool's documentation for where Agent Skills go.

AI tools that support the [MCP skills extension](https://modelcontextprotocol.io/seps/2640-skills-extension) load these skills straight from the BugHerd MCP server, so there's nothing to install.

### Best results with pinned feedback

BugHerd always does its best to pin feedback to the right element and attach a screenshot. Results are most accurate when your AI tool can open the page in a browser session, run JavaScript in it, upload screenshots, and reach the page the way your visitors do. If your site needs a login, the agent's browser should be signed in.

## Security & Authentication

BugHerd MCP is a remote MCP server that supports OAuth-based authorization (via DCR or CIMD authentication), so access is tied to your account and can be revoked at any time in BugHerd settings.

## Need Help?

- Browse all help docs: [support.bugherd.com](https://support.bugherd.com/)
- Contact BugHerd support via in-app chat or [support@bugherd.com](mailto:support@bugherd.com)
