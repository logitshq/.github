# logitsHQ repository defaults

Shared contribution guidelines, security reporting instructions, and issue and pull request templates for logitsHQ repositories. Repository-specific files take precedence over these defaults.

## Repository setup

- Use `main` as the default branch and create company repositories as private unless their contents are approved for public release.
- Grant access explicitly through project teams or repository collaborators; use the lowest role needed.
- Keep at least two designated organization owners, and require two-factor authentication for members and outside collaborators.
- For public repositories, protect the default branch with pull requests, one approving review, resolved review conversations, and no force pushes or branch deletion. Organization owners may bypass review requirements within a pull request when necessary.
- On GitHub Free, private-repository branch protection and organization-wide rulesets require a paid plan. Apply the same review process by convention until protections are available.
- Prefer squash merges and automatically delete merged branches.
- Enable dependency alerts and security updates. Enable secret scanning and push protection wherever the plan supports them.
- Keep workflow tokens read-only by default. Grant write access explicitly in jobs that need it, pin actions to full commit SHAs, and approve workflows from external contributors.
- Add project-specific CI and require its checks only after they run successfully. Add a local `CODEOWNERS` file when maintainers are assigned; it is not inherited from this repository.
- Use workload identity/OIDC or narrowly scoped GitHub Apps for automation. Store credentials in repository or environment secrets, and protect production deployment environments where supported.

These are setup guidelines. Templates and documentation do not enforce settings on newly created repositories.

GitHub documentation: [default community files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file), [organization best practices](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/best-practices-for-organizations).
