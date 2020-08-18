# Workflow for Semantic Release

This is a GitHub Actions workflow for [Semantic Release][@GH/semantic-release].

## What it implements
1. It executes `build` and `test` scripts with node `10.x`, `12.x` and `14.x` if the scripts are present.
2. It executes `semantic-release` script.

## How to use
1. Follow [this instruction][@NPM/doc/token] to fetch a npm token.
2. Add npm token as `NPM_TOKEN` in GitHub Actions secrets.
3. Copy `.github/workflows/semantic-release.yml` in this repo to your repo.
4. Configure Semantic Release in you repo, add `semantic-release` package and `semantic-release` script in `package.json`, i.e
```json
"scripts": {
    "semantic-release": "semantic-release"
}
```
5. Commit and push your project.

[@GH/semantic-release]: https://github.com/semantic-release/semantic-release
[@NPM/doc/token]: https://docs.npmjs.com/creating-and-viewing-authentication-tokens
