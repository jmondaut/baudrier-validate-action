# Baudrier validate Action

Validates every `harness.yaml` and `SKILL.md` in your repository with the `baudrier` CLI, installed from PyPI.

This folder is published (once the owner has done `deploy/RUNBOOK.md` steps 8-9, after the PyPI publish) as the public repository `jmondaut/baudrier-validate-action` (the owner creates it from this
folder and tags `v1`).

```yaml
- uses: actions/checkout@v4
- uses: jmondaut/baudrier-validate-action@v1
```

## Pinning a version

The CLI version defaults to the one this action release was cut for. Pin another with the `version` input:

```yaml
- uses: jmondaut/baudrier-validate-action@v1
  with:
    version: 0.2.0
```

Pin the action itself to a release tag (or a full commit SHA).
