## Step 2 — Clone and create feature branches

All three students now work from the **same shared repository**. Do not use forks.

Each person clones the repository locally:

```bash
git clone <repository-url>
cd <repository-folder>
git status
```

Then create the assigned branch:

```text
Owner / Maintainer → feature-html
Collaborator A     → feature-css
Collaborator B     → feature-javascript
```

Example:

```bash
git switch -c feature-css
```

Each role owns exactly one source file:

```text
feature-html       → index.html
feature-css        → style.css
feature-javascript → script.js
```

Do not edit the other two role files. The checker verifies the three branch names and later verifies file ownership from the Pull Request diffs.
