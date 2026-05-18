# amlmarketplaces/fireworks

Claude Code marketplace federating all `@amlplugins/fireworks-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-fireworks": {
      "source": { "source": "github", "repo": "amlmarketplaces/fireworks" }
    }
  },
  "enabledPlugins": {
      "fireworks-chat@aml-fireworks": true,
      "fireworks-images@aml-fireworks": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/fireworks`, cached under `~/.claude/plugins/cache/aml-fireworks/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (2 total)

- `fireworks-chat` — [@amlplugins/fireworks-chat](https://github.com/amlplugins/fireworks-chat)
- `fireworks-images` — [@amlplugins/fireworks-images](https://github.com/amlplugins/fireworks-images)

## Related

- npm packages: `@amlplugins/fireworks-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
