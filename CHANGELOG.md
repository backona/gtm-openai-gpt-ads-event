# Changelog

All the project changes should be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Do not edit the NEW_VERSION and VERSION_DATE fields, they will be updated automatically by the Github Action script.

## [<NEW_VERSION>] - <VERSION_DATE>
### Added
- OpenAI ChatGPT Ads Event GTM template to send `oaiq('measure', …)` for all JavaScript Pixel standard events, custom events, and optional contents array
- Unit tests that optional value, plan, and contents fields are omitted from the measure payload when not applicable to the selected event, even if set in tag data
### Changed
- Renamed template display name from OpenAI GPT Ads Event to OpenAI ChatGPT Ads Event; aligned Configuration companion template references to OpenAI ChatGPT Ads Configuration; README and install steps reference [gtm-openai-gpt-ads-event](https://github.com/backona/gtm-openai-gpt-ads-event) and root `template.tpl`
- Simplified Recommended setup help to Configuration tag prerequisite only; removed App install / open events field section; moved Recommended setup below Event guidance and added Consent Mode v2 guidance matching the Configuration template; aligned Event guidance copy with current field labels and lowercase contents references, including Page viewed confirmation-page contents guidance; moved Custom event name directly below Event when Custom is selected; tag summary shows Event and Recommended setup only; Event guidance uses ZIPPY_OPEN_ON_PARAM so it stays collapsed when opening tag edit until expanded manually
- Event contents: optional contents array (variable or JSON) with structure hints and spaced JSON example in field help and placeholder instead of row-by-row table; section guidance blended into Amount, Plan ID, and Contents source field help; optional GA4 items auto-mapping into OpenAI contents
### Fixed
- GTM Code tab and test runtime errors: sandbox-safe integer parsing (no regex, parseInt, charCodeAt, isNaN, or try/catch)
- Blank Template Preview on the Fields tab: consolidated event hints into a group, added default Event selection, removed REGEX field validators, and normalized em dashes to ASCII hyphens in field labels
- Template import error: replaced invalid groupStyle enum ZIPPY_OPEN_ON_NONDEFAULT with ZIPPY_CLOSED
- Empty Event dropdown in template preview: removed unsupported help property from Event selectItems
- oaiq missing console message: two-line guidance naming the Backona ChatGPT Ads Configuration tag explicitly
- Sandbox ignores optional value, plan_id, and contents not applicable to the selected event (matches Fields tab visibility), including invalid contents on inapplicable events
