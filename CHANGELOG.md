# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0] - 2026-05-04

### Changed
- Bump `wp-connector-api` from `0.9` to `0.10`.
- Bump `orion-error` from `0.7` to `0.8`.
- Bump `derive_more` from `2` to `2.1`.
- Migrate runtime error conversion helpers from the removed `orion_error::conversion_ext` path to `orion_error::conversion`.
- Use `conv_err()` for structured `Result` reason conversions under `orion-error` `0.8`.

[Unreleased]: https://github.com/wp-labs/wp-connector-test-utils/compare/v0.2.0...HEAD
[0.2.0]: https://github.com/wp-labs/wp-connector-test-utils/releases/tag/v0.2.0
