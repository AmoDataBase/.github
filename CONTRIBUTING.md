# Contributing to amodb

Thanks for helping. Keep changes small and focused.

This file applies to every repository in the amodb-dev organization that does not ship its own CONTRIBUTING.md. Repository files take priority and list the exact checks for their stack.

## Before you start

1. Read the [code of conduct](CODE_OF_CONDUCT.md).
2. Search the open and closed issues for the same topic.
3. Open an issue first for anything larger than a bug fix or a doc fix, so we can agree on the approach.

## Make a change

1. Fork the repository and create a branch from `main`.
2. Make the change and add or update tests for the behavior you change.
3. Run the checks listed in the repository README or CONTRIBUTING.md.
4. Open a pull request and fill in the template.

## Commits

- Imperative mood, one short line, no trailing period. For example: `Add retry on 429`.
- One logical change per commit.
- No generated trailers or tool attribution lines.

## Text in docs and comments

- Short, concrete sentences with numbers where you have them.
- Sentence case headings.
- No long dashes and no `--` in prose.
- No filler words.

## Secrets

Never commit API keys, tokens or `.env` files. Use environment variables. If a key lands in a commit by mistake, revoke it first, then tell security@amodb.dev.

## License

By contributing you agree that your work is released under the MIT license of the repository you contribute to.
