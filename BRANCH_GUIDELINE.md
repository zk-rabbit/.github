# Branch Guideline

Branch names must only consist of `[a-z|A-Z|0-9|-|/]` characters and are generally in the form `<type>/<subject>`.

- `<type>` : One of the defined [Commit Types](/COMMIT_MESSAGE_GUIDELINE.md#type) we use.
- `<subject>` : Starts with an imperative verb. Explains the goal of this branch.

An example of a viable branch name is `feat/add-xyz`.

## Exception for docs-only or small-purpose repositories

In repositories that only contain documentation (e.g., `.github`) or small-purpose projects
(e.g., benchmarks, experiments), the `type` prefix in branch names **may be omitted**.
In such cases, use a clear and concise subject that still follows the rules above.
