# vibe-engineering

Personal [Claude Code](https://docs.claude.com/en/docs/claude-code) plugin marketplace.

A thin index — it doesn't host plugin code, it points at upstream repos. Plugin content is fetched from each `source` on update.

## Plugins

| Plugin | Source | What it is |
|---|---|---|
| `mattpocock-skills` | [`mattpocock/skills`](https://github.com/mattpocock/skills) | Matt Pocock's engineering + productivity skills |

## Usage

Add the marketplace:

```
/plugin marketplace add areeshzakir/vibe-engineering
```

Install a plugin:

```
/plugin install mattpocock-skills@vibe-engineering
```

## Updating

```
/plugin marketplace update vibe-engineering   # refresh this index (rarely changes)
/plugin update mattpocock-skills              # pull latest skills from upstream
```

`/plugin update` re-fetches from each plugin's `source`, so you stay in sync with the upstream repos automatically.

## Adding more plugins

Add an entry to `.claude-plugin/marketplace.json` and push.
