# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.4.0] - 2020-12-06

### Added

- Allow to set custom delimiters on tables, columns and cells.

### Changed

- Expose all important traits. I.e. `ToRow`, `ToCell` and `ToCells`.

## [1.3.0] - 2020-11-20

### Added

- New ColumConstraint for hiding columns

## [1.2.0] - 2020-10-27

### Added

- Add the option to set a max-height on rows. Long content will be truncated.

## [1.1.1] - 2020-08-23

### Changed

- A simple update of all dependencies.

## [1.1.0] - 2020-08-23

### Changed

- Move `is_tty` logic from `atty` to `crossterm`.
- Remove `skeptic`, since it fails in CI and bloats compile time. Compile time is reduced by ca. 40%.

## [1.0.0] - 2020-07-07

### Changed

- The project has been in use for quite some time and seems to be quite stable!
- Use cargo's `example` functionality for examples.

## [0.1.1] - 2020-05-24

### Added

- `Column::get_max_width()`, which returns the character count of the widest line in this column including padding.
- `current_style_as_preset` method for convenient conversion of a style into a preset
- New Markdown like table style prefix. Thanks to [joeydumont](https://github.com/joeydumont).

## [0.1.0] - 2020-03-21

### Added

- Better test coverage

### Fixed

- Fixed a bug with broken percentage constraints for super wide tables.

## [0.0.7] - 2020-02-09

### Added

- Introduce proptest

### Fixed

- Fix wrong calculation due to bytes count instead of char count
- Fix panics caused by wrong string splits

## [0.0.6] - 2020-01-31

### Changed

- Crossterm 0.15 update
- Simplify the project's module structure

## [0.0.5] - 2020-01-29

### Added

- Add `Column::remove_constraint()`
- Preset `UTF8_NO_BORDERS`
- Preset `UTF8_HORIZONTAL_BORDERS_ONLY`

## [0.0.4] - 2020-01-27

### Added

- Add skeptic tests
- Add code coverage
- A lot more tests

### Changed

- Removed `Hidden` Constraint
