<img src="https://my-badges.github.io/my-badges/fix-3.png" alt="I did 3 sequential fixes." title="I did 3 sequential fixes." width="128">
<strong>I did 3 sequential fixes.</strong>
<br><br>

Commits:

- <a href="https://github.com/AndrewWeinmann/andrewweinmann.dev/commit/9fd92af6d92af8f981203192b6d18593774751b6">9fd92af</a>: fix(ci): hard-fail on missing Playwright image and block e2e on version sync (#24)
- <a href="https://github.com/AndrewWeinmann/andrewweinmann.dev/commit/b80cc69b9c84348d4aeaf4d7b9d4347841e68337">b80cc69</a>: fix(ci): hard-fail on missing Playwright image and block e2e on version sync

- Exit 1 (not 0) when no Playwright Docker image is found in ci.yml
- Add playwright-version-sync to e2e job's needs so a version mismatch
  actually prevents E2E from running

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>
- <a href="https://github.com/AndrewWeinmann/andrewweinmann.dev/commit/42b93b6c37cccc0db7699b0e65bdc9bab38ca4aa">42b93b6</a>: fix(dependabot): group react packages and exclude types from dev-dependencies

react and react-dom are prod deps so they fell outside the dev-dependencies
group — Dependabot was bumping them separately, causing render failures when
versions diverged (as seen in PR #13).

Also adds exclude-patterns on dev-dependencies for @types/react and
@types/react-dom so group membership is explicit rather than relying on
ordering.

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>