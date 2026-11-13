# Role templates

Placeholders install.sh fills, in these exact formats:

- `{{OWNER}}`: the owner's name, as plain text
- `{{EMAIL}}`: the owner's email address
- `{{OWNER_ID}}`: the owner's Swarm user id, `@id:server`, from the `owner`
  field of `swarm accounts add`'s JSON
- `{{COMPANY}}`: the company's name
- `{{ROOM}}`: the room the engineering sous answers in, `#room:server`
- `{{ACCOUNT}}`: the sous's own Swarm account, `@name:server`

Each agent's `CLAUDE.md` is `base.md` followed by its role file, joined into
one file:

| Agent | `CLAUDE.md` |
|---|---|
| Engineering | `base.md` + `eng.md` |
| Chief of staff | `base.md` + `cos.md` |

These are owner-neutral starting points for a customer's machine. The
operator's own roles live in the folders beside this one.
