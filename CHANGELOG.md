# Changelog

All the project changes should be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Do not edit the NEW_VERSION and VERSION_DATE fields, they will be updated automatically by the Github Action script.

## [<NEW_VERSION>] - <VERSION_DATE>
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

