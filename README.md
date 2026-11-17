# renovate-config

Shared Renovate presets for other repos

```json
"extends": ["github>jasonpanosso/renovate-config"]
```

`default.json` holds the base settings and extends all of these presets:

| Preset             | Contents                                                                |
| ------------------ | ----------------------------------------------------------------------- |
| `:annotations`     | `# renovate: datasource=… depName=…` comments in yaml, sh and env files |
| `:autoMerge`       | Actions and the pinned Renovate CLI automerge after 3 days              |
| `:labels`          | `type/*` and `renovate/*` PR labels                                     |
| `:nix`             | Enable nix manager                                                      |
| `:semanticCommits` | Commit type by update type, scope and topic by datasource               |

List it before the repo's own presets in `extends` (later rules win)
