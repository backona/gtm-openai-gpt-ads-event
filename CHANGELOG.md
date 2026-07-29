# Changelog

All the project changes should be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Do not edit the NEW_VERSION and VERSION_DATE fields, they will be updated automatically by the Github Action script.

## [<NEW_VERSION>] - <VERSION_DATE>
### Added
### Changed
### Fixed

## [1.1.4] - 2026-07-29 (by @slazak)
### Fixed
- Log a clear console error when `window.oaiq` exists but is not a function (includes `oaiqType`) instead of a silent GTM exception

## [1.1.3] - 2026-07-16 (by @slazak)
### Changed
- Install docs prioritize `template.tpl` import; note Community Template Gallery submission is pending Google approval

## [1.1.2] - 2026-07-08 (by @slazak)
### Added
- Debug mode checkbox to enable measure payload logging in GTM preview and browser console

## [1.1.1] - 2026-07-08 (by @slazak)
### Changed
- Optional section labels simplified: redundant “(Optional)” removed from fields inside optional groups; Advanced options renamed to Advanced options (Optional)

## [1.1.0] - 2026-07-07 (by @slazak)
### Changed
- Clearer tag layout: event guidance directly under Event selector (expanded by default), dedicated sections for custom event name and Plan ID, recommended setup below Advanced options
- Optional amount × 100 conversion for mapping GA4-style major currency values to OpenAI minor units
- GTM preview logs the resolved measure payload to the console when the tag fires successfully

## [1.0.1] - 2026-07-03 (by @slazak)
### Changed
- Recommended setup guidance aligned with Configuration template: Initialization — All Pages trigger recommended

## [1.0.0] - 2026-07-03 (by @slazak)
### Changed
- Plan ID, Event value, and Event contents are shown inline under the Event selector when the selected event supports them

## [0.0.1] - 2026-07-02 (by @slazak)
### Added
- OpenAI ChatGPT Ads Event GTM template to send `oaiq('measure', …)` for all JavaScript Pixel standard events, custom events, and optional contents array

