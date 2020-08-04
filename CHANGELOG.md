# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](keep-a-changelog.md),
and this project adheres to [Semantic Versioning](semver.md).

## [Unreleased]

### Added
* `--update-self` to install the latest copy of AM
### Changed
### Deprecated
### Removed
### Fixed
### Security

## [1.6.0] - 2020-08-04

### Added
* `-c` To Clone a given git repository
* `-td` Path to clone into; Then move there and execute normal behaviour

### Changed
* Ninja is now default, `-n` was replace with `-m` which now enables GNU Make
* Git Submodules are now pulled by default `--no-git-modules` disables this

## [1.5.0] - 2020-08-03

### Added
* Help command
* `-g` Flag allows to init and update git submodules before a build

### Change
* Check for a non-zero error code after calling git, cmake, make and ninja

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
