# Commit subjects for public CodeMonster repositories

This convention applies to new commits in public repositories under
`codemonster-ru`. It follows the
[CodeMonster UI commit convention](https://github.com/codemonster-ru/ui/blob/main/docs/codemonster-ui-roadmap.md#how-to-use-this-roadmap).

## Write a subject

Start with an English verb in the imperative mood and capitalize the first
word. Describe the change in a concise sentence fragment. Omit Conventional
Commits prefixes and the final period. Keep established spelling for product
names and public identifiers.

Limit the full subject to 100 characters, including any GitHub pull request
suffix. Describe the change in a merge subject and omit literal commit SHAs.

- `Add a quick start for Floater.js`
- `Fix stale SSR Service links`
- `Describe Annabel package checks`
- `Release SkinCSS 1.0.0`

Use the commit body for context, compatibility notes, and issue references.
Keep GitHub's standard merge and revert subjects and the `(#123)` suffix it adds
when squashing a pull request. For squash merges, give the pull request an
imperative title. For generated split commits, apply the convention in the
source monorepo and let the publishing workflow update the mirrors.

## Check new commits

The commit-subject workflow checks formal conventions on pushes and pull
requests. The pull request check must pass before merging into the default
branch of each source repository. Review the wording and imperative verb
when reviewing a change.
