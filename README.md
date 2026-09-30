# .github

Quicko's organisation-wide defaults for GitHub community files.

These are standardised **issue templates** so every repo gets the same "Bug Report" and "Story" forms without having to duplicate them.

## What's here

```
ISSUE_TEMPLATE/
├── bug-report-template.yml   # Structured bug report form
└── story-template.yml        # Structured user story form
```

## How it applies to other repositories

Any repository in the `org-quicko` organization that does **not** have its own `.github/ISSUE_TEMPLATE` directory will automatically show these templates. Repositories that need repo-specific templates can still define their own — a local `ISSUE_TEMPLATE` directory takes precedence over this one.

## Adding or updating a template

1. Add or edit a `.yml` file under `ISSUE_TEMPLATE/` using [GitHub's issue form schema](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms).
2. Keep `name`, `description`, and `labels` accurate — they control how the template appears in the "New Issue" picker.
3. Open a pull request. Since this repo is org-wide, changes affect issue creation across all repositories that don't override the template, so get a review before merging.
