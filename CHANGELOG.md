<!-- Source: Keep a Changelog 1.1.0 (MIT) — https://keepachangelog.com/en/1.1.0/ -->
# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.3] - 2026-09-23

### Fixed

- Create mode no longer falls back to a local repository on its own when the user asked for GitHub and the GitHub CLI is not signed in; it asks the user to sign in or to approve a local repository instead.
- Create mode now asks for a keep-or-remove decision on every recommended module as well as every optional one, as the template's setup step S07 requires.
- CONTRIBUTING pointed at a README section that does not exist; it now points at Install and the Agent Skills validator.

## [1.0.2] - 2026-09-23

### Changed

- The skill repository moved to the chefs-pick-oss-starter organization, beside the template: https://github.com/chefs-pick-oss-starter/chefs-pick-oss-starter-skill. Install and link addresses are updated; the old address redirects. Matches template 1.2.1.

## [1.0.1] - 2026-09-23

### Fixed

- Point at the template's current home, chefs-pick-oss-starter/chefs-pick-oss-starter, instead of relying on GitHub's redirect from the old address.

## [1.0.0] - 2026-09-23

### Added

- The chefs-pick-oss-starter skill: create a repository from the Chef's Pick OSS Starter template, or align an existing repository with it. Works with template 1.1.0 and later.

[Unreleased]: https://github.com/chefs-pick-oss-starter/chefs-pick-oss-starter-skill/compare/v1.0.3...HEAD
[1.0.3]: https://github.com/chefs-pick-oss-starter/chefs-pick-oss-starter-skill/compare/v1.0.2...v1.0.3
[1.0.2]: https://github.com/chefs-pick-oss-starter/chefs-pick-oss-starter-skill/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/chefs-pick-oss-starter/chefs-pick-oss-starter-skill/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/chefs-pick-oss-starter/chefs-pick-oss-starter-skill/releases/tag/v1.0.0
