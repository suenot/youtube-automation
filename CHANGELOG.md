# Changelog

All notable changes to this repository are documented here. The format follows Keep a Changelog, and versions follow Semantic Versioning.

## [Unreleased]

## [0.2.1] - 2026-10-08

### Fixed

- Pin publisher 0.2.1: expired Google sessions are detected from authenticated
  Studio UI, and Firefox session refresh preserves the channel binding and
  publication journal with cookie rollback on failed verification.

## [0.2.0] - 2026-10-07

### Changed

- Pin `youtube-automation-prepare` 0.2.0 with scoped Firefox login transfer into Camoufox, exact channel and Public preflight, saved-video verification, and a durable request journal preventing repeat uploads after uncertain results.

### Added

- Record the verified Caribbean Awesome channel ID and the no-upload preflight for its first public Short.

## [0.1.0] - 2026-10-06

### Added

- Group YouTube metadata preparation and publishing as pinned Git submodules.
