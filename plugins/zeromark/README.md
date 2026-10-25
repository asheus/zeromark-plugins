# ZeroMark for Claude Code

> **Coming soon.** The connector is not live on zeromark.io yet. Installing it now has nothing to connect to, and the connector guide is not published.

Read the posts you saved on X, and your ZeroMark Living Memory, from Claude Code.

## Install

```
/plugin marketplace add asheus/zeromark-plugins
/plugin install zeromark@zeromark
```

Then run `/mcp`, pick `zeromark`, and sign in. A ZeroMark page asks you to
approve read-only access. That is the whole setup: no key to copy.

Prefer a key? Make one in ZeroMark, Settings, "Connect to Claude, ChatGPT or
Gemini", and add the server yourself instead of the plugin:

```
claude mcp add --transport http --scope user zeromark https://www.zeromark.io/api/mcp \
  --header "Authorization: Bearer zm_mcp_YOUR_KEY"
```

## What it can do

Eight read-only tools: `library_overview`, `search_saves`, `get_save`,
`list_by_stage`, `get_memory`, `weekly_question`, and `search` / `fetch`.
It cannot mark anything Done, let anything go, edit or delete, in ZeroMark or
on X. Disconnect it any time in ZeroMark's Settings.

The bundled skill, `zeromark-library`, tells Claude which tool fits which
question and how to cite what it finds.

The connector guide will be published when this ships. The site is https://www.zeromark.io.
