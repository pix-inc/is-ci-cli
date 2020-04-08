# is-ci-cli

Run different npm scripts in a CI environment

Workaround instead of [is-ci-cli](https://github.com/YellowKirby/is-ci-cli) to be used with GitHub Actions.

Under the hood it uses [ci-info](https://github.com/watson/ci-info) which hasn't released an update with GitHub Actions support for a long time.

## Usage

In your `package.json`:

```json
"scripts": {
    "test": "is-ci test:ci test:local"
}
```

When in a CI environment, this runs the first argument as a yarn or npm script.
Otherwise, run the 2nd argument (if provided)
