# Security policy

ZeroMark holds people's reading history, so we take reports seriously and answer them quickly.

## Reporting a vulnerability

Please **do not open a public issue** for a security problem.

Use GitHub's private reporting: **Security → Report a vulnerability** on this repository. Only the maintainers can see what you send.

Include what you found, how to reproduce it, and what an attacker could do with it. If you can, say which client you were using (Claude Code, claude.ai, ChatGPT, Gemini CLI, VS Code, Cursor).

## What to expect

| Step | When |
| --- | --- |
| We confirm we received it | Within 2 business days |
| We tell you whether we can reproduce it | Within 5 business days |
| We fix a confirmed issue | As fast as its severity calls for, and we keep you posted |

We will credit you in the changelog if you would like to be named.

## Scope

In scope:

- The connector at `https://www.zeromark.io/api/mcp` and its OAuth endpoints under `/oauth/mcp/` and `/.well-known/`.
- The files in this repository.

Out of scope: denial of service by volume, reports from automated scanners with no demonstrated impact, and social engineering of ZeroMark staff.

## Good-faith research

Research done in good faith, against your own account, without touching other people's data or degrading the service, is welcome.
