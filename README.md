# I Ching: Shape of Momentum

Static SvelteKit landing page for the I Ching: Shape of Momentum app.

## Development

```sh
yarn install
yarn dev
```

## Checks

```sh
yarn run check
yarn build
```

## GitHub Pages

The project uses `@sveltejs/adapter-static` and deploys through
`.github/workflows/deploy.yml`. During GitHub Actions builds, SvelteKit uses the
repository name from `GITHUB_REPOSITORY` as `paths.base`, so assets resolve under
`/i-ching-site/`.
