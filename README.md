# Enthym organization profile and contribution defaults

[`profile/README.md`](profile/README.md) is the public profile for the existing
`verifiablelabs` organization. Repository, package, import, and command names
retain Verifiable Labs identifiers; current company prose uses Enthym.

The public research scope and repository map live in
[vlabs-docs](https://github.com/verifiablelabs/vlabs-docs). Keep the profile short
and link to that maintained documentation rather than copying result tables.

## Files and scope

- [CONTRIBUTING.md](CONTRIBUTING.md): shared guidance where a repository has
  no local contribution file; each repository defines its own test commands
  and license terms.
- [.github/ISSUE_TEMPLATE/](.github/ISSUE_TEMPLATE/): general bug and proposal
  templates for repositories that inherit organization defaults.
- [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md): reviewer
  context, validation evidence, and disclosure checks.
- [SECURITY.md](SECURITY.md): existing private reporting route.

Repository-specific community files take precedence over organization defaults.
These templates change contribution prompts; they do not configure CI, required
reviews, branch protection, permissions, or release approval.

## Local review

There is no application build or runtime dependency in this repository.
Check `git diff --check`, relative links, issue-template front matter, and the
rendered Markdown. Review the profile and default-template scope with a
maintainer before publication. Keep private repository names, code, findings,
and protected evaluation material out of public additions. Preserve license
and historical attribution.
