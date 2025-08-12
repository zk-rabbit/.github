# Pull Request Guideline

We value **clarity** and **traceability** in our codebase.
Even for small changes (e.g., timeout adjustments), if the change is **non-trivial**, please provide context and reasoning to help reviewers and future contributors understand the intent.

Keep in mind:

> A PR author is one, but reviewers are many.
> Write in a way that even a first-time visitor to the project can grasp the context.

---

## File Formatting Checklist

- [ ] Every file ends with a single newline (`\n`)
- [ ] No extra blank lines at the end of files
- [ ] No trailing whitespaces at the end of lines

---

## Code Convention

- [ ] Follow the [Google Style Guide](https://google.github.io/styleguide/)
- [ ] Code has been linted and formatted using the project’s configured tools

---

## Commit Convention

- [ ] Commit messages follow the [Commit Message Guideline](/COMMIT_MESSAGE_GUIDELINE.md)
- [ ] Commits are **atomic** and logically organized
      (e.g., style changes are not mixed with functional changes)
- [ ] **Every commit is independently buildable and testable**
- [ ] Used a **stacked PR structure** if applicable (base branch is not `main` but a previous PR branch)

---

## PR Convention

- [ ] Branch name follows the [Branch Guideline](/BRANCH_GUIDELINE.md)
- [ ] No intermediate changes within PR

---

## Clarity & Reference Checklist

- [ ] Added inline comments or PR description for **non-obvious logic or decisions**
- [ ] Included relevant links to external code or documentation

  - GitHub links should include only the first **7 characters** of the commit SHA
  - Example:

    ```cpp
    // See
    // https://github.com/Consensys/gnark-crypto/blob/43897fd/ecc/bn254/fr/vector.go#L133-L159
    ```
