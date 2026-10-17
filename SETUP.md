# Enable your contribution snake

1. Open your public profile repository: https://github.com/night-owldev/night-owldev
2. Replace README.md with the supplied README.md. Keep dark.svg and light.svg in the repository root.
3. Create `.github/workflows/snake.yml` using Add file → Create new file, then paste the supplied snake.yml contents. Commit it to the default branch (normally main). If uploading the extracted folder, make sure the hidden `.github` directory is included. Do not upload the ZIP itself.
4. Open Actions → Generate Contribution Snake → Run workflow. If GitHub asks you to enable Actions, enable them first.
5. After a successful run, the separate `output` branch will contain github-snake.svg and github-snake-dark.svg. The README links point there. Until this first run succeeds, the snake image will not load.

The workflow requests contents: write for its generation job. If publishing fails with a permissions error, check repository/organization Actions policies and any rules protecting the output branch. No personal access token or GitHub Pages site is required for this same-repository setup.

Scheduled run: daily at 00:17 UTC (05:47 India time), subject to GitHub scheduling delays. You can also run it manually. Scheduled workflows must be on the default branch; GitHub may disable schedules in inactive public repositories.

The PDF uses a separate github-snake repository. This package keeps the workflow inside night-owldev/night-owldev instead, with matching README URLs. `output` is a branch, not a folder on main. Use this output branch for generated snake assets only.

The workflow has been prepared and checked locally, but has not been uploaded or run on your GitHub account.

References:
- https://github.com/Platane/snk
- https://github.com/crazy-max/ghaction-github-pages
