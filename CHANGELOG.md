# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

### Added
* Added level based log filtering

### Removed
* Stopped creating bevy events for incomming logs

### Fixed
* Logviewer will no longer panic if a log event arrives after the receiver was dropped

## [0.2.1] - 2024-11-01

### Fixed
* Fixed wasm build

## [0.2.0] - 2024-11-01

### Added
* Logviewer now has buttoms for clearing logs and going fullscreen
* Loglines now show timestamps
* Logviewer can now be configured to open automtically when an event of a certain level is received.

### Changed
* Replaced the plugin initialization function `bevy_debug_log::plugin()` with `bevy_debug_log::LogViewerPlugin::default()` 

## [0.1.1] - 2024-10-10

### Added
* Added screenshot to `README.md`

### Changed
* Updated `Cargo.toml` to exclude `assets` directory

## [0.1.0] - 2024-09-01

### Added
* Initial implementation of `bevy_debug_log` with basic logging functionality