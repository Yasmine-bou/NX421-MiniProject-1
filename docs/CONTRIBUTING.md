# Collaboration rules

- One person owns edits to a notebook at a time; discuss changes in pull requests.
- One task = one branch such as `feature/structural-skullstrip`.
- Do not commit NIfTI datasets, large derived outputs, or confidential information.
- Run notebooks top-to-bottom on the EPFL VM and describe tested Neurodesk tool versions.
- Use relative/configured paths; document every preprocessing transform and interpolation choice.
- Git workflow:
  ```bash
  git switch main
  git pull --ff-only
  git switch -c feature/my-task
  # edit; verify code; then:
  git add .
  git commit -m "Describe change"
  git push -u origin feature/my-task
  ```
  Open a PR on GitHub, obtain a review, and merge.
- Before final submission: clear huge notebook outputs; ensure reproducibility and prepare professor-required code folder.
