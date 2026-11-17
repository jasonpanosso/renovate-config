# renovate-config

Shared Renovate presets for other repos

| Preset                                | Contents                                                                |
| ------------------------------------- | ----------------------------------------------------------------------- |
| `github>jasonpanosso/renovate-config` | Base settings (`default.json`)                                          |
| `:annotations`                        | `# renovate: datasource=… depName=…` comments in yaml, sh and env files |
| `:autoMerge`                          | Actions and the pinned Renovate CLI automerge after 3 days              |
| `:labels`                             | `type/*` and `renovate/*` PR labels                                     |
| `:nix`                                | Enable nix manager                                                      |
| `:semanticCommits`                    | Commit type by update type, scope and topic by datasource               |

List these before the repo's own presets in `extends` (later rules win)
