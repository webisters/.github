# Contributing to Webisters

Thanks for your interest in improving Webisters! This guide applies to every
repository in the [webisters](https://github.com/webisters) organization. It is a
default community health file, so individual repositories may add their own
`CONTRIBUTING.md` to override it.

- Documentation: https://docs.webisters.com
- Website: https://webisters.com

## Ways to contribute

- Report bugs and request features by opening an issue (please use the provided
  templates).
- Improve documentation, examples, and READMEs.
- Submit pull requests that fix bugs or add features.
- Help triage and review open issues and pull requests.

## Project layout

Webisters is a full-stack PHP framework organized as a monorepo of independently
versioned Composer packages. Each library, package, and project skeleton is its
own repository under the `webisters` organization and uses the `Framework\*` PHP
namespace. There is no root `composer.json`; every package manages its own
dependencies, tests, and coding standard.

## Requirements

- PHP `>=8.2`
- Composer 2.x
- The PHP extensions the package needs. See the
  [Requirements guide](https://docs.webisters.com/guides/webisters/#requirements)
  (commonly `intl`, `sodium`, `gd`, `mysqli`, `curl`, `fileinfo`, plus `openssl`
  and `zip` for Composer).

## Getting started

```bash
# 1. Fork and clone the repository you want to work on
git clone https://github.com/<your-user>/<repo>.git
cd <repo>

# 2. Install dependencies
composer install

# 3. Run the test suite
vendor/bin/phpunit

# 4. Check and fix coding style
vendor/bin/php-cs-fixer fix --dry-run --diff   # check
vendor/bin/php-cs-fixer fix                     # apply
```

Coding style is centralized in
[`webisters/coding-standard`](https://github.com/webisters/coding-standard); each
package's `.php-cs-fixer.dist.php` extends it. Please keep the standard file
header on new files (it is managed by php-cs-fixer).

## Pull request checklist

Before opening a pull request, please make sure:

- [ ] Tests pass (`vendor/bin/phpunit`).
- [ ] Coding style passes (`vendor/bin/php-cs-fixer fix --dry-run --diff`).
- [ ] New behavior is covered by tests where practical.
- [ ] Public APIs and notable changes are documented.
- [ ] The change is focused; unrelated changes are split into separate PRs.

## Commit and branch conventions

- Create a feature branch from the default branch; do not commit directly to it.
- Write clear, imperative commit messages (for example, "Add retry to HTTP client").
- Reference related issues in the PR description (for example, "Fixes #12").

## Reporting security issues

Please do not open public issues for security vulnerabilities. Email
**support@webisters.com** instead so we can address the problem responsibly.

## Code of Conduct

By participating in this project you agree to abide by our
[Code of Conduct](CODE_OF_CONDUCT.md).
