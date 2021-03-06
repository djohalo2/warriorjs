# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to
[Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.5.1] - 2018-06-01

### Fixed

- External towers discovery ([@olistic][] in [#188][])

## [0.5.0] - 2018-06-01

### Added

- Load towers dynamically (support for external towers) ([@olistic][] in
  [#169][])
- Add tower description to README if available ([@olistic][] in [#185][])

### Changed

- Prevent seeing through walls with "look" ability ([@pigalot][] in [#162][])
- Optimize profile file ([@olistic][] in [#170][] and [#180][])
- No longer ask for confirmation before creating game directory ([@olistic][] in
  [#177][])

## [0.4.2] - 2018-05-23

### Added

- Warrior name suggestions ([@olistic][] in [#152][])

## [0.4.1] - 2018-05-22

### Added

- `--silent` flag to CLI ([@xaviserrag][] in [#82][])

### Changed

- Print level independently of play log ([@olistic][] in [#145][])
- UI tweaks ([@olistic][] in [#147][])
- Improve think ability description ([@olistic][] in [#149][])
- Improve level tips ([@olistic][] in [#150][])

## [0.4.0] - 2018-05-19

### Added

- Make warrior upset when losing points ([@skywalker212][] in [#107][])
- `getRelativeOffset` function (`@warriorjs/geography`) ([@olistic][] in
  [#138][])
- `unit.release()` method ([@olistic][] in [#140][])

### Changed

- Rename `unit.say()` to `unit.log()` ([@olistic][] in [#131][])
- Improve profile directory detection ([@glneto][] in [#133][])
- Rename `unit.isHostile()` to `unit.isEnemy()` ([@olistic][] in [#129][])
- `space.getLocation()` returns the relative location of the space ([@olistic][]
  in [#129][])
- `unit.isEnemy()` returns whether the unit is considered an enemy by the unit
  that sensed it ([@olistic][] in [#129][])

### Removed

- `unit.isFriendly()` ([@olistic][] in [#129][])
- `unit.isWarrior()` and `unit.isPlayer()` ([@olistic][] in [#129][])

### Fixed

- Line breaks on CLI output on Windows ([@olistic][] in [#120][])
- Diamond symbol on Windows ([@glneto][] in [#121][])

## [0.3.0] - 2018-05-16

### Added

- Subtract reward points when killing a friendly unit ([@Terseus][] in [#87][])
- Think ability (`console.log` replacement) ([@olistic][] in [#102][])

### Changed

- Distinguish between hostile and friendly units ([@xFloki][] in [#101][])
- Move unit methods out of the Space API and to the Unit API ([@olistic][] in
  [#113][])

### Fixed

- Enforce [Player API](https://warrior.js.org/docs/space-api) ([@olistic][] in
  [#114][])

## [0.2.0] - 2018-05-14

### Added

- Reward property to Unit class ([@RascalTwo][] in [#67][])
- Warrior score next to health in play log ([@RascalTwo][] in [#70][])
- Support for Node 9 and 10 ([@olistic][] in [#81][])
- `--yes` flag to CLI ([@olistic][] in [#93][] and [#98][])

### Changed

- Exclude abilities from play log except warrior's ([@olistic][] in [#83][])
- Rescue ability awards Unit's reward ([@RascalTwo][] in [#86][], [@olistic][]
  in [#90][])
- CLI default answers ([@olistic][] in [#97][])

### Removed

- `--skip` flag from CLI ([@olistic][] in [#93][])

### Fixed

- Path normalization in tests ([@jakehamilton][] in [#77][])

## [0.1.1] - 2018-05-03

### Fixed

- Missing `bin` directory in `@warriorjs/cli` package files

## 0.1.0 - 2018-05-03 [YANKED]

Initial version.

[unreleased]: https://github.com/olistic/warriorjs/compare/v0.5.1...HEAD
[0.5.1]: https://github.com/olistic/warriorjs/compare/v0.5.0...v0.5.1
[0.5.0]: https://github.com/olistic/warriorjs/compare/v0.4.2...v0.5.0
[0.4.2]: https://github.com/olistic/warriorjs/compare/v0.4.1...v0.4.2
[0.4.1]: https://github.com/olistic/warriorjs/compare/v0.4.0...v0.4.1
[0.4.0]: https://github.com/olistic/warriorjs/compare/v0.3.0...v0.4.0
[0.3.0]: https://github.com/olistic/warriorjs/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/olistic/warriorjs/compare/v0.1.1...v0.2.0
[0.1.1]: https://github.com/olistic/warriorjs/compare/v0.1.0...v0.1.1
[@olistic]: https://github.com/olistic
[@rascaltwo]: https://github.com/RascalTwo
[@jakehamilton]: https://github.com/jakehamilton
[@terseus]: https://github.com/Terseus
[@xfloki]: https://github.com/xFloki
[@skywalker212]: https://github.com/skywalker212
[@glneto]: https://github.com/glneto
[@xaviserrag]: https://github.com/xaviserrag
[@pigalot]: https://github.com/pigalot
[#67]: https://github.com/olistic/warriorjs/pull/67
[#70]: https://github.com/olistic/warriorjs/pull/70
[#77]: https://github.com/olistic/warriorjs/pull/77
[#81]: https://github.com/olistic/warriorjs/pull/81
[#82]: https://github.com/olistic/warriorjs/pull/82
[#83]: https://github.com/olistic/warriorjs/pull/83
[#86]: https://github.com/olistic/warriorjs/pull/86
[#87]: https://github.com/olistic/warriorjs/pull/87
[#90]: https://github.com/olistic/warriorjs/pull/90
[#93]: https://github.com/olistic/warriorjs/pull/93
[#97]: https://github.com/olistic/warriorjs/pull/97
[#98]: https://github.com/olistic/warriorjs/pull/98
[#101]: https://github.com/olistic/warriorjs/pull/101
[#102]: https://github.com/olistic/warriorjs/pull/102
[#107]: https://github.com/olistic/warriorjs/pull/107
[#113]: https://github.com/olistic/warriorjs/pull/113
[#114]: https://github.com/olistic/warriorjs/pull/114
[#120]: https://github.com/olistic/warriorjs/pull/120
[#121]: https://github.com/olistic/warriorjs/pull/121
[#129]: https://github.com/olistic/warriorjs/pull/129
[#131]: https://github.com/olistic/warriorjs/pull/131
[#133]: https://github.com/olistic/warriorjs/pull/133
[#138]: https://github.com/olistic/warriorjs/pull/138
[#140]: https://github.com/olistic/warriorjs/pull/140
[#145]: https://github.com/olistic/warriorjs/pull/145
[#147]: https://github.com/olistic/warriorjs/pull/147
[#149]: https://github.com/olistic/warriorjs/pull/149
[#150]: https://github.com/olistic/warriorjs/pull/150
[#152]: https://github.com/olistic/warriorjs/pull/152
[#162]: https://github.com/olistic/warriorjs/pull/162
[#169]: https://github.com/olistic/warriorjs/pull/169
[#170]: https://github.com/olistic/warriorjs/pull/170
[#177]: https://github.com/olistic/warriorjs/pull/177
[#180]: https://github.com/olistic/warriorjs/pull/180
[#185]: https://github.com/olistic/warriorjs/pull/185
[#188]: https://github.com/olistic/warriorjs/pull/188
