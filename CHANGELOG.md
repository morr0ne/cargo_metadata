# Changelog

## Unreleased

### Added

- Re-exported `semver` crate directly.

### Changed

- Made `parse_stream` more versatile by accepting anything that implements `Read`.

### Removed

- Removed re-exports for `BuildMetadata` and `Prerelease` from `semver` crate.

### Fixed

- Parsing no longer fails for future rust editions.

### Internal Changes

- Make use `thiserror` crate for the Error implementation.

## [0.15.0] - 2022-06-22
### Added

- Re-exported `BuildMetadata` and `Prerelease` from `semver` crate.
- Added `workspace_packages` function.
- Added `Edition` enum to better parse edition field.
- Added `rust-version` field to Cargo manifest.

### Changed

- Bumped msrv from `1.40.0` to `1.42.0`.

### Internal Changes

- Updated `derive_builder` to the latest version.
- Made use of `matches!` macros where possible.
- Fixed some tests

## [0.14.2] - 2022-02-16

### Added

- Derive `PartialEq` and `Eq` where possible

### Internal Changes

- Fixed some tests
