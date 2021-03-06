# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [0.10.1] - 2020-03-29

### Added

- generated ebuild file
- pkgs/ to .gitignore
- support for Gentoo Portage ebuild packages

### Fixed

- custom extensions
- RPM spec add swipl dependency
- recognise RPM spec files

### Removed

- obsolete custom heuristics

## [0.10.0] - 2020-06-27

### Added

- AGPL header to source files
- `pkgs/` to `.gitignore`
- support for qubes-builder
- target `test` to `Makefile`
- tests for parsing filename extensions
- unittest for linguist samples

### Changed

- `file:list_files_recursive` to use relative paths
- project structure to recommended by SWI Prolog
- read buffer to 10 * 1024
- `t/linguist` to be deterministic
- speed up by ~16%
- move read_file to file module

### Fixed

- exception `max_files`
- handling files starting with a dot
- more failing tests
- `parse_extension`
- Singleton warning in `main([])` goal
- swi prolog warning
- typo in pydoc
- `parse_extension/2` handle files starting with dot and no extension

### Refactored

- file extension parsing to `module(file)`
- file guessing functions to `module(file_expert)`

## [0.9.0] - 2019-01-27

### Added

- First release
