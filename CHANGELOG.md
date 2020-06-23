# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](keep-a-changelog.md),
and this project adheres to [Semantic Versioning](semver.md).

## [Unreleased]

### Added
### Changed
### Deprecated
### Removed
### Fixed
### Security

## [1.4.0] - 2020-06-23

### Changed
* AM is now able to use multiple args, it will consume all args up to a `--`. Args after ar passed to Make or Ninja

## [1.3.0] - 2020-06-23

### Added
* Check that Make, CMake and Ninja are installed

## [1.2.0] - 2020-06-23

### Added
* Flag `-l` to cat the `build/am-build.log`

### Changed
* Modulerize the code into functions

### Fixed
* Fix name of the ninja build file

## [1.1.0] - 2020-06-23

### Added
* Check for Ninja and Makefile before CMakeLists

## [1.0.0] - 2020-06-23

### Added
* First Implementation
