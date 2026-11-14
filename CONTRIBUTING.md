# Contributing to theyvoteforyou

They Vote For You presents parliamentary voting information through a Rails application. Contributions can improve accurate data handling, application behaviour, accessibility, documentation and country-specific support.

## Before you start

Read [README.md](README.md), especially Development and the relevant country-specific notes. Check open issues and pull requests before starting a substantial change. Preserve the project's upstream attribution and country-specific behaviour. This guide concerns changes in this repository; an upstream contribution should follow the upstream project's process.

For bugs, provide the affected version or commit, environment, minimal reproduction, expected result and observed result. For a substantial proposal, describe the use case and compatibility impact before expanding implementation scope. Use existing issue templates when offered.

## Development and validation

Use the Ruby version in [.ruby-version](.ruby-version) and the dependency versions in [Gemfile.lock](Gemfile.lock). The README documents MySQL, HTMLTidy and the local configuration steps. Work with a disposable development database and sanitized fixtures. After completing that setup, its established commands include:

```sh
bundle install
bundle exec rake
```

The second command runs the test suite. Follow the README for development configuration and database setup instead of using production settings. Do not copy real credentials, accounts or a production database into fixtures.

Add a focused regression test for changed calculations, imports, routing or user-visible behaviour. For database changes, describe migrations and compatibility. For interface work, inspect affected pages and accessibility as well as automated results. Record which country-specific paths were exercised and which remain unverified.

## Pull requests

Create a focused branch from the current `main` branch and submit a pull request to this repository. Link the relevant issue or existing project task, explain the resulting behaviour, and update affected examples and documentation. Keep unrelated changes in separate pull requests.

Report executed commands, outcomes and the commit they validate. Identify unavailable checks and remaining limitations explicitly. Follow the repository's existing review and automated-check requirements; retain required gates and current ownership. Address findings and verify the final head before integration. Repository changes do not themselves authorise a release or external operational action.

## Security, rights and conduct

Follow the [security policy](https://github.com/edithatogo/.github/blob/main/SECURITY.md). Use private vulnerability reporting if available; otherwise request a private contact without publishing vulnerability details. Keep credentials, personal information and restricted source material out of issues, fixtures, logs and artifacts.

Read the [existing licence](LICENSE) and preserve attribution and third-party terms. Follow the [code of conduct](https://github.com/edithatogo/.github/blob/main/CODE_OF_CONDUCT.md) and keep technical discussions respectful.

## Basis for this guide

This guide follows [GitHub's contribution-guideline guidance](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors) and the contribution-process and testing principles in [OpenSSF Best Practices](https://www.bestpractices.dev/en/criteria). It does not assert certification.
