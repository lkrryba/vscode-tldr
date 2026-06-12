name: vscode-tldr

description: Parse VS Code release notes and produce a whimsical, emoji-rich, max-10-line summary of what's new — in a way user will actually want to read. Use this skill whenever user pastes VS Code release notes and asks for a summary, digest, TL;DR, or "what's new in VS Code". Also trigger if she says anything like "make this readable", "animal edition", or "translate these release notes". The output is always delivered directly in the chat, never as a file.

---
 
# VS Code TLDR
 
Turn dense VS Code release notes into a punchy, whimsical, max-10-line summary with thematic emojis and personality. Output goes directly in the chat.
 
## Your job
 
Read the release notes provided and extract the genuinely interesting or useful changes. Ignore contributor lists, deprecated features with no replacement, minor typo fixes, and enterprise admin stuff unless it's genuinely notable.
 
## Output format
 
- Max 10 bullet points
- Each line gets one emoji chosen for a specific reason — behavioural, visual, or conceptual. Animals are preferred when a behaviour fits (penguins queue, frogs jump, crabs move sideways). Non-animal emojis are fine when they're more apt (📖 for reading, 🤖 for autopilot, 🥳 for sarcastic celebration). The connection should always be explainable. This reasoning is internal — do not write it out.
- Never add parentheticals. No emoji explanations, no jokes in brackets, nothing in parentheses. Just the emoji and the feature description.
- No emoji repeats across the whole summary
- Plain, punchy language — write like you're texting a friend who codes
- One line = one idea (don't cram two features into one bullet)
- Lead with the most interesting/impactful change
- End with a one-line vibe check: what's the overall theme of this release? (e.g. "Basically: VS Code got a memory." or "TL;DR: they made agents less annoying.")
- No headers, no bold, no markdown formatting beyond the bullets themselves
- No em dashes
## Tone
 
Dry wit is the default. Enthusiasm is fine if earned. Don't oversell minor stuff. Sarcasm is appropriate for enterprise/admin features ("thrilling if you are an enterprise admin").
 
## What to look for
 
Prioritise in this order:
1. Things that change how you actually use the editor day-to-day
2. Agent/AI workflow improvements
3. New keyboard shortcuts or navigation features
4. Browser or integrated tool improvements
5. Anything with a setting name that sounds genuinely useful
## Example output style (not content — don't reuse this)
 
🐧 Background session queuing means you can fire off requests without waiting for the last one to finish

🧟‍♀️ Sessions now restore after a reload, layout and all, so you land exactly where you left off

🐦 New keyboard picker lets you search and hop between sessions with ⌃R

🤖 Agents now use a utility model to decide when they're actually done instead of just stopping

🐸 New shortcuts to step forward and back through sessions and jump by position

📖 Browser URL bar now suggests pages from your history as you type

🧐 Single-file diff setting so you can focus on one change without the noise

🦀 Chevron in the editor title bar collapses the sidebar to widen your view

🥳 Enterprise plugin policies sync from one config file now, thrilling if you are an enterprise admin
 
TL;DR: This one's all about making agent sessions feel less like chaos and more like a workflow.
