# Typescript NPM Package Template

Create and publish TS/JS NPM packages seamlessly.

**Interested in supporting this free template?**

<a href="https://www.buymeacoffee.com/josegoval" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Steps

1. Clone, download or fork this project.
2. Replace in the [package.json](package.json) the next values with your own ones:
    - name
    - description
    - keywords
    - repository
    - author
3. Create a NPM secret and add it to the project secrets:
    - Generate Token in `https://www.npmjs.com/settings/<your-profile>/tokens`
    - Create a `New repository secret` named `NPM_TOKEN` and copy its value (`https://github.com/<username>/<project-name>/settings/secrets/actions`)

## How to skip the `npm publish` step

As you can check in [.releaserc](.releaserc) and [release.yml workflow](.github/workflows/release.yml), and read in depth in the [semantic-release documentation](https://semantic-release.gitbook.io/semantic-release/usage/configuration), the project is configured to trigger a new versioned commit and publish to NPM under `master`, `next`, `next-major`, `beta` and `alpha`.

To skip a CI include `[skip ci]` in the commit title or cancel the Github action.



