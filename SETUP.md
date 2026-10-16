# Publish your profile

## 1. Upload the core files

1. Sign in as **Faizalimam001**.
2. Create a **public** repository named exactly **Faizalimam001**. If it already exists, edit that repository instead.
3. Put `README.md` at the repository root and upload the `assets` folder beside it. Commit to the default branch.
4. Open https://github.com/Faizalimam001 to view your profile.

The repository should contain:

```text
README.md
assets/hero.svg
assets/hero-static.svg
.github/workflows/snake.yml    (optional)
```

Do not paste the SVG source directly into the README. The existing image reference loads it correctly. The SVG is an original vector design with native SVG animation, no JavaScript, external fonts, or external image dependencies. Its five phrases rotate every four seconds. For a motion-free version, replace `./assets/hero.svg` with `./assets/hero-static.svg`.

GitHub controls the page background and fonts. A README cannot force dark mode or apply arbitrary page CSS. The hero carries its own charcoal background; body text remains readable in either GitHub theme. On narrow screens the hero scales down; the meaningful profile text also appears as ordinary Markdown.

## 2. Optional contribution snake

1. Add `.github/workflows/snake.yml` to the default branch. If uploading in the web UI, use **Add file → Create new file**, enter that full path, and paste the supplied workflow source. This avoids missing the hidden `.github` folder when extracting/uploading.
2. Open **Actions → Generate contribution snake → Run workflow**. Enable Actions if GitHub asks.
3. Wait for success. Confirm the `output` branch contains `github-snake.svg`.
4. In README.md, remove the opening comment line beginning `<!-- OPTIONAL SNAKE:` and the closing `END OPTIONAL SNAKE -->` line. Keep the `<p>` and `<img>` block between them.
5. Commit the README. The snake now displays your real contribution grid.

The workflow runs daily at 02:23 UTC (07:53 IST), and can be run manually. It uses GitHub's automatic `GITHUB_TOKEN`; do not create or paste a personal access token. It declares `contents: write` to publish the generated image. Repository or organization restrictions may still block this; check the failed workflow log if publishing is denied.

The `output` branch is dedicated to generated assets. The workflow force-replaces that branch only; never store hand-written code there. The default branch is untouched. Scheduled runs can be delayed, and GitHub may disable schedules in public repositories after 60 days without repository activity. Re-enable the workflow if needed.

The snake starts commented out to avoid a broken image before its first successful run. No contribution data is invented or included in this download. The workflow has been checked locally for YAML structure but has not been run in your account.

## 3. Optional activity cards

The expandable activity section requests statistics, repository language breakdowns, and a recent contribution graph using **Faizalimam001**. No static numbers have been supplied. Providers can return cached data, errors, or rate-limit responses. If unavailable, remove the entire `<details>...</details>` block; direct GitHub links remain.

The public card services are optional conveniences, not uptime guarantees. GitHub Readme Stats documents self-hosting if you want greater control. Language shares reflect eligible repository code rather than ability, and these services may not include all private activity. No private-repository access is configured.

## 4. Placeholders

| Placeholder / choice | What to do |
| --- | --- |
| `YOUR_LINKEDIN_SLUG` in README.md | Replace with your real LinkedIn profile slug and uncomment that link, or leave it hidden. |
| Optional snake comment | Enable only after the first successful workflow run. |

Your name, username, and portfolio link are already filled in. No other identity placeholders need replacing. The portfolio URL is preserved exactly as provided; it could not be fetched from this environment.

## Sources and asset notes

- Profile repository requirements: https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme
- Native snake action and color options: https://github.com/Platane/snk
- GitHub Readme Stats API, top languages, limitations and self-hosting: https://github.com/anuraghazra/github-readme-stats
- Recent contribution graph API: https://github.com/Ashutosh00710/github-readme-activity-graph
- Authentic brand icons and documented colored CDN URLs: https://github.com/simple-icons/simple-icons#cdn-usage
- Scheduled workflow behavior: https://docs.github.com/en/actions/reference/workflows-and-actions/events-that-trigger-workflows#schedule

Brand icons use Simple Icons' documented CDN with the Python, FastAPI, PostgreSQL, Hugging Face, Git, and GitHub slugs. Text labels and the technology table preserve meaning if an icon service fails. Brand names and marks belong to their owners; their appearance does not imply endorsement.

No account settings or repositories were modified while creating this package.

Validation: SVG XML and workflow YAML structure were checked locally, and the static hero was rendered for visual inspection. Live GitHub rendering and the Actions run remain to be checked after upload. Direct icon requests were blocked with HTTP 403 in this environment; URLs follow the provider documentation.
