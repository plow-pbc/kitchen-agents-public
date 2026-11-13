# kitchen-agents-public

Owner-neutral role templates for a [kitchen](https://github.com/srosro/kitchen)
of Claude Code agents: an engineering sous and a chief of staff sous that run
on their owner's machine and talk to people in Swarm.

Each agent's `CLAUDE.md` is `templates/base.md` followed by its role file
(`templates/eng.md` or `templates/cos.md`), joined into one file, with these
placeholders filled in:

| Placeholder | Value |
|---|---|
| `{{OWNER}}` | the owner's name |
| `{{EMAIL}}` | the owner's email address |
| `{{OWNER_ID}}` | the owner's Swarm user id, `@id:server` |
| `{{COMPANY}}` | the company's name |
| `{{ROOM}}` | the room the engineering sous answers in, `#room:server` |
| `{{ACCOUNT}}` | the sous's own Swarm account, `@name:server` |

Only the owner, and delegates the owner names by exact id in their own
message, can direct an agent's actions. See `templates/README.md` for details.

MIT licensed.
