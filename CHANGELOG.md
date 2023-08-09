# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [6.3.6] - 2023-08-09
### Added
- Emphasise new field button when collection has no fields

### Fixed
- Minor backend bug fixes

## [6.3.5] - 2023-08-09
### Changed
- Fields that can be selected multiple times are no longer greyed out after a single selection

### Fixed
- Fixed an issue preventing reordering fields
- Make it easier to discover the configure fields button
- Fixes to usage tracking
- Improvements to magic tables
- Improvements to custom field predictions

## [6.3.4] - 2023-08-08
### Changed
- Improved logging

### Fixed
- Improved performance in annotation handling (stage 1)
- Various backend bug fixes

## [6.3.3] - 2023-08-08
### Added
- Allow users to add data points that don't have bounding boxes on the page

### Fixed
- Improved document sorting algorithm
- Improved construction of nested annotations
- More graceful handling of errors around currencies
- Other backend bug fixes
- Fix bug in scenario where document does not have a workspace specified

## [6.3.2] - 2023-08-05
### Fixed
- Minor backend bug fixes

## [6.3.1] - 2023-08-05
### Fixed
- Better handling of huge images during OCR
- Improved parsing of dates from text

## [6.3.0] - 2023-08-04
### Removed
- Removed deprecated db tables

## [6.2.9] - 2023-08-04
### Changed
- Only use documents within selected collection when parsing with GPT-4
- Improved grouping of annotations when using group annotation types.
- When words contain a forward slash, split them into two words

### Fixed
- Backend bug fixes
- Handle error with unidentified images
- Fix null handling in resume sections
- Improve handling for scenario when two tables are shown side by side
- Parse quantities annotated as "free" as 0

## [6.2.8] - 2023-08-03
### Removed
- Removed legacy Azure OCR service

### Fixed
- Backend bug fixes

## [6.2.7] - 2023-08-03
### Fixed
- Fixed issue where renaming table fields could remove nested fields

### Added
- Show in the validation tool if a document has been split
- Show in the document list if a document has been split

## [6.2.6] - 2023-08-03
### Fixed
- Magic tables bug fix that was causing row items not to be visible

## [6.2.5] - 2023-08-03
### Added
- Better filename handling

### Fixed
- Various bug fixes

## [6.2.4] - 2023-08-02
### Changed
- Improved logging

## [6.2.3] - 2023-08-02
### Added
- Additional setup for automatic document sorting

### Fixed
- Bullhorn bug fixes

## [6.2.2] - 2023-08-02
### Changed
- Improved rate limiting for custom extractors

## [6.2.1] - 2023-08-01
### Fixed
- Various backend bug fixes

## [6.2.0] - 2023-08-01
### Added
- Support for nested field configurations
- GPT parsing for picklists, nested fields, multiple fields, and rectless fields.

### Changed
- Improved handling for ingestion of documents via email

## [6.1.4] - 2023-07-31
### Fixed
- Improved email sender handling
- Fix tooltip persisting after hovering field in sidebar
- Improve parsing of floats

## [6.1.3] - 2023-07-31
### Fixed
- Various backend bug fixes

## [6.1.2] - 2023-07-28
### Changed
- Better signup flow for bullhorn integration

## [6.1.1] - 2023-07-27
### Changed
- Improving release process

## [6.1.0] - 2023-07-23
### Added
- Initial public release
