# vscode-tldr
**Never slog through endless lines of release notes again. Instead, have them presented my a menagerie of whimsy animals in an easy-to-read format. 🐳🦁🐢🦊🦉🐧🦄🐙🐝🦋🐞🐸🦥🐼🦜🐬🦔🦒🦘🐨🦩**

As a developer friend once told me: "_Do I read VS Code release notes? God no! If I read all that I'd never get anything done._"

Well now, you don't have to.

This is a Claude skill that takes VS Code release notes and turns them into a max 10-line summary you'll actually read. Each item gets an emoji chosen for a reason (penguins queue 🐧, frogs jump 🐸, crabs go sideways 🦀), dry wit where earned, and a one-line vibe check at the end.

**Example output**

From VS Code 1.124:

🐧 Background sessions: queue up your next agent request before the current one finishes, no waiting around

🧟‍♀️ Sessions now fully restore after a reload, layout and all, so you land exactly where you left off

🐦 New sessions picker (⌃R / ⌘R) lets you search by title or folder and jump straight to what you need

🤖 Autopilot is on by default, and a utility model now reads the conversation to decide if the task is genuinely done

🐸 New keyboard shortcuts to step forward/back through sessions and jump to a session by position with ⌃1 to ⌃9

📖 Browser URL bar now suggests pages from your history as you type, manageable with ⌘H

🧐 New setting to always open a single-file diff instead of the whole noisy multi-file view

🦀 A chevron in the editor title bar now collapses the sidebar so you can widen the editor without hunting through menus

🥳 Enterprise plugin policies can sync from one config file now, thrilling if you are an enterprise admin

TL;DR: This release is mostly about agent sessions finally feeling like something you can use rather than ignore.


## Installation (not scary)
 
### Claude Code (VS Code)
 
Make sure you have the [Claude Code extension](https://marketplace.visualstudio.com/items?itemName=Anthropic.claude-code) installed in VS Code first.
 
Then run these three commands in your terminal:
 
```bash
# 1. Create the skills directory
mkdir -p ~/.claude/skills/vscode-tldr
 
# 2. Download the skill
curl -o ~/.claude/skills/vscode-tldr/SKILL.md https://raw.githubusercontent.com/lkrryba/vscode-tldr/main/SKILL.md
 
# 3. Restart Claude Code in VS Code
```
 
## Usage
 
Paste VS Code release notes into your chat and ask for a summary. Works with any of these:
 
- "summarise these release notes"
- "what's new in VS Code"
- "tldr this"
- "make this readable"
The skill auto-triggers on the content. You don't need a specific command.
 
## Built with
 
Built iteratively using the Claude skill creator in [claude.ai](https://claude.ai), with a few rounds of very specific feedback about emoji philosophy 🏛️
 
