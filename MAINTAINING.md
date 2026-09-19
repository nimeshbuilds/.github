# Keeping Nimesh Builds useful and easy to find

## Where things live

| Change | Location |
| --- | --- |
| Organization bio, avatar, and public links | Organization Settings → General |
| Organization landing content | `profile/README.md` |
| Project status | `ROADMAP.md` and `projects/` |
| Shared community defaults | Root community files and `.github/ISSUE_TEMPLATE/` |
| Community conversations | Organization Discussions, backed by this repository |
| Repository search metadata | Repository About → description, website, and topics |
| Repository share card | Repository Settings → General → Social preview |
| Brand source and exports | `assets/` |

## For each new software repository

1. Use a short name and a one-sentence description explaining the real use case.
2. Add a small set of accurate topics. GitHub allows up to 20; filling all slots is unnecessary.
3. Put the problem, current status, working demo, and quickest verified setup near the top of the README.
4. Include an explicit license, supported versions, required permissions, and cleanup instructions. A license is not inherited from this `.github` repository.
5. Enable private vulnerability reporting before accepting security reports. Override the shared policies or templates when the project needs more specific instructions.
6. Upload a readable share image, link the real docs, and pin the most useful repositories on the organization profile. GitHub supports up to six pins.
7. Label `good first issue` only when the task is small, described, and ready for a new contributor. Use `help wanted` for work you actually want help completing.

## When there is meaningful progress

- Update the roadmap when a milestone has evidence.
- Publish a short announcement: the problem, what changed, a demo or reproduction, known limits, and the next step.
- Release working versions with notes and migration information when needed.
- Keep contributor acknowledgements accurate. Answer useful questions and turn recurring ones into docs.
- Share a launch in relevant communities only after there is something people can try and in line with each community's rules.

## Discovery and measurement

GitHub provides the profile and repository pages. This setup uses clear descriptions, readable Markdown, real topic tags, useful internal links, and a repository share image. It does not give maintainers control over GitHub's HTML metadata or search-engine indexing schedule.

Review repository **Insights → Traffic** for views, clones, and available referrers. Also track useful discussions, reproducible feedback, contributors, and repeat use. These show whether people are getting value; stars alone do not.

If a separate website is added later, it can have its own page titles, descriptions, canonical URLs, social metadata, sitemap, and search-engine verification. Add only public links and contact details the owner has approved.

No metadata setting guarantees search rankings, trending placement, or stars. A small tool with a convincing demo and responsive maintenance is the next important milestone.

## Official references

- [Customize an organization profile](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile)
- [Repository topics](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics)
- [Default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [Repository social previews](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/customizing-your-repositorys-social-media-preview)
