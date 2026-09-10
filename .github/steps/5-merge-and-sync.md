## Step 5 — Merge and sync `main`

Once the collaborator PRs are ready, the **Owner / Maintainer** merges the approved work. The Owner also merges the self-checked HTML PR.

All three feature Issues should close through the `Closes #...` references in the Pull Requests.

After all three PRs are merged, **each of the three participants** runs locally:

```bash
git switch main
git pull
git rev-parse --short HEAD
```

Then each person posts a separate comment in this Exercise Issue using exactly:

```text
SYNCED SHORT_SHA
```

Example:

```text
SYNCED a1b2c3d
```

The checker verifies the commenter identity, that the proof was posted after the final merge, and that the SHA matches the current remote `main` head. It also verifies that the Owner performed the merges.
