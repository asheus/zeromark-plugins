# ZeroMark for Claude Code

Other connectors give Claude what you saved. ZeroMark gives it your taste in X: what you kept, what you let go, and what you concluded, from Claude Code.

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

Eleven read-only tools. The one that matters most is `get_taste`: what you
decided, one save at a time (kept and let go, per field and per voice, and what
your notes stopped believing). The rest read your saves (`search_saves`,
`get_save`, `list_by_stage`, `library_overview`, `search` / `fetch`), your
Living Memory (`get_memory`), your Map (`get_map`), your podcast
(`get_podcast`) and a weekly suggestion (`weekly_question`). It cannot mark
anything Done, let anything go, edit or delete, in ZeroMark or on X: you
decide, your assistant reads. Disconnect it any time in ZeroMark's Settings.

The bundled skill, `zeromark-library`, tells Claude which tool fits which
question and how to cite what it finds.

Guide: https://www.zeromark.io/docs/connector
