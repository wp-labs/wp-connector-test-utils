# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.3.0] - 2026-09-19

### ⚠️ BREAKING CHANGES

- Bump `wp-connector-api` from `0.12` to `0.13` and `wp-model-core` from `0.9` to `0.10`. These two must be upgraded together: `wp-connector-api` `0.13` is the release aligned with `wp-model-core` `0.10`, which renamed the integer variants (`Value::Digit` → `Value::Int`, `DataType::Digit` → `DataType::Int`). Consumers such as `wp-connectors` must move in one go.

### Changed

- Follow the `wp-model-core` `0.10` integer rename: `DataField::from_digit` → `from_int`.

## [0.2.0] - 2026-05-04

### Changed
- Bump `wp-connector-api` from `0.9` to `0.10`.
- Bump `orion-error` from `0.7` to `0.8`.
- Bump `derive_more` from `2` to `2.1`.
- Migrate runtime error conversion helpers from the removed `orion_error::conversion_ext` path to `orion_error::conversion`.
- Use `conv_err()` for structured `Result` reason conversions under `orion-error` `0.8`.

[Unreleased]: https://github.com/wp-labs/wp-connector-test-utils/compare/v0.3.0...HEAD
[0.3.0]: https://github.com/wp-labs/wp-connector-test-utils/compare/v0.2.4...v0.3.0
[0.2.0]: https://github.com/wp-labs/wp-connector-test-utils/releases/tag/v0.2.0
