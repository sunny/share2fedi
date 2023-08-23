# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.4.5] - 2023-06-17

### Fixed

- blocked crawling of all pages other than index (#33)

## [2.4.4] - 2023-03-01

### Fixed

- fixed not working instance prefilling (#15)

## [2.4.3] - 2022-12-23

### Changed

- analytics script replaced with own implementation
  - now uses `navigator.sendBeacon()` for a more lightweight solution
  - now doesn't send anything other than path and screen size
- updated CanIUse databases, which may cause some browsers become unsupported

## [2.4.2] - 2022-12-21

### Changed

- analytics should send query parameters anymore

### Removed

- tracking pixel for JS-less analytics

## [2.4.1] - 2022-11-20

### Fixed

- "remember instance on this device" didn't work (#12, #13)

## [2.4.0] - 2022-11-14

### Added

- analytics from GoatCounter
  - the analytics are GDPR-friendly
  - the analytics script is lightweight
  - [the results are publicly accessible](https://share2fedi.goatcounter.com/)
- better instructions for self-hosting (cred Tealk: #4, #5)

## [2.3.1] - 2022-03-16

### Fixed

- wrong font-weight on the "Toot!" button

## [2.3.0] - 2022-03-16

### Changed

- self-hosted the Roboto font due to privacy concerns when using Google Fonts

## [2.2.2] - 2022-02-12

### Changed

- repository moved to Codeberg; updated all URLs

## [2.2.1] - 2021-02-02

### Changed

- changed GitHub username from `NickKaramoff` to `kytta`

## [2.2.0] - 2021-11-04

### Changed

- migrated to PNPM as primary package manager
- change URL from `toot.karamoff.dev` to `toot.kytta.dev`

## [2.1.0] - 2021-08-29

### Added

- LibreJS-compatible licence identifiers
- SPDX licence identifiers

## [2.0.0] - 2021-08-29

### Added

- hosting how-to (#17)
- description in the `<title>` (#13)
- sourcemaps for all files
- licence header to all files

### Changed

- toot doesn't require JS to post anymore (#12)
- make backend not Vercel-dependend
- update `robots.txt`
- use pure HTML instead of Pug
- simplify style and script pipeline

## [1.2.2] - 2021-08-14

### Security

- bumped dependencies (#16, #18)

## [1.2.1] - 2021-05-13

### Security

- bumped dependencies (#14, #15)

## [1.2.0] - 2021-03-17

### Changed

- design of the page so that it looks more like a Mastodon website (without impersonating anyone)

### Fixed

- page displacement if a child is added to `<body>` (#11)

## [1.1.2] - 2021-03-12

### Changed

- Node.js version is now 14, since it's now supported by Vercel

### Security

- migrated from `gulp-sass` to `@mr-hope/gulp-sass` to avoid loading and building `node-sass` and other old deps

## [1.1.1] - 2021-03-03

### Added

- `.node-version` file for nodenv
- Added `engines.node` field to `package.json`
  - this is required to ensure the correct environment for builds

### Security

- Bumped insecure Pug libraries
  - `pug-code-gen` (#9)
  - `pug` (#10)
- Bumped other dependencies

## [1.1.0] - 2021-01-30

### Added

- Add CHANGELOG as file

### Changed

- License changed from MIT to AGPL-3.0
- Add new, Mastodon-like logo (#6)
- Change "Mastodon" text to Mastodon's logo (#6)

## [1.0.0] - 2021-01-29

### Added

- Provide a list of Mastodon servers from joinmastodon.org (#1)
- Start marking version numbers

### Changed

- Reword the Remember checkbox (#2)
- Open Mastodon in the same tab (#3, #4)

## (no version number)

Initial release of the site

### Added

- Add main code for the site

[Unreleased]: https://codeberg.org/kytta/toot/compare/v2.4.5...HEAD
[2.4.5]: https://codeberg.org/kytta/toot/compare/v2.4.4...v2.4.5
[2.4.4]: https://codeberg.org/kytta/toot/compare/v2.4.3...v2.4.4
[2.4.3]: https://codeberg.org/kytta/toot/compare/v2.4.2...v2.4.3
[2.4.2]: https://codeberg.org/kytta/toot/compare/v2.4.1...v2.4.2
[2.4.1]: https://codeberg.org/kytta/toot/compare/v2.4.0...v2.4.1
[2.4.0]: https://codeberg.org/kytta/toot/compare/v2.3.1...v2.4.0
[2.3.1]: https://codeberg.org/kytta/toot/compare/v2.3.0...v2.3.1
[2.3.0]: https://codeberg.org/kytta/toot/compare/v2.2.2...v2.3.0
[2.2.2]: https://codeberg.org/kytta/toot/compare/v2.2.1...v2.2.2
[2.2.1]: https://codeberg.org/kytta/toot/compare/v2.2.0...v2.2.1
[2.2.0]: https://codeberg.org/kytta/toot/compare/v2.1.0...v2.2.0
[2.1.0]: https://codeberg.org/kytta/toot/compare/v2.0.0...v2.1.0
[2.0.0]: https://codeberg.org/kytta/toot/compare/v1.2.2...v2.0.0
[1.2.2]: https://codeberg.org/kytta/toot/compare/v1.2.1...v1.2.2
[1.2.1]: https://codeberg.org/kytta/toot/compare/v1.2.0...v1.2.1
[1.2.0]: https://codeberg.org/kytta/toot/compare/v1.1.2...v1.2.0
[1.1.2]: https://codeberg.org/kytta/toot/compare/v1.1.1...v1.1.2
[1.1.1]: https://codeberg.org/kytta/toot/compare/v1.1.0...v1.1.1
[1.1.0]: https://codeberg.org/kytta/toot/compare/v1.0.0...v1.1.0
[1.0.0]: https://codeberg.org/kytta/toot/compare/e85aa15400bcdbcccf655d331f72df8304744b85...v1.0.0
