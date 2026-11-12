# @locol23/renovate-config

[Shareable config](https://renovatebot.com/docs/config-presets/) for [Renovate](https://renovatebot.com)

![GitHub Actions](https://github.com/locol23/renovate-config/actions/workflows/test.yml/badge.svg)

## Setup

Add `github>locol23/renovate-config` to `extends` property for your renovate config

```json
{
  "extends": ["github>locol23/renovate-config"]
}
```

Note: You don't need to npm install

## Vulnerability updates

Vulnerability pull requests ignore the overnight schedule and the 7-day minimum release age. They automerge once status checks pass, and they stay open while checks are failing. A repository with no status checks has nothing to wait for, so Renovate automerges those updates on the next run.

## Required repository labels

Create these labels in each consuming repository so Renovate can attach them to PRs:

- `security`
- `CI`
- `dependencies`

## License

MIT
