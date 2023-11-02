# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [6.18.0] - 2023-11-02
### Fixed
- Significant performance improvements in the validation tool for large and complex documents

### Changed
- More clearly de-emphasise other non-child annotations when focussing on a group or table

## [6.17.0] - 2023-10-31
### Fixed
- Fixed issue where incorrect currency values could be introduced for some currency codes

## [6.16.0] - 2023-10-23
### Changed
- Document.identifier has been made globally unique, and replaced with customIdentifier where users would like topass through their own identifiers for a document.

## [6.15.0] - 2023-10-09
### Added
- Added hideSidePanel option for resume and job search tools

## [6.14.0] - 2023-10-05
### Changed
- New invoice collection will now use the new "magic tables" interface by default.
- Documentation can be found [here](https://docs.affinda.com/docs/magic-tables).

## [6.13.0] - 2023-09-28
### Changed
- Enable annotations to be drawn across multiple pages

## [6.12.0] - 2023-09-28
### Changed
- Migrated several confirmation dialogs to be in-app instead of using browser dialogs

## [6.11.0] - 2023-09-27
### Added
- Improved usability of field configuration dialog
- Added ability to configure dropdown field options and text field automatic matching

## [6.10.0] - 2023-09-18
### Changed
- Improved queuing algorithm for a smoother bulk parsing experience

### Fixed
- Implemented stricter limits on email uploads

## [6.9.0] - 2023-09-14
### Changed
- Made it easier to discover the change collection menu

## [6.8.0] - 2023-09-12
### Changed
- Rebrand for consistency with new frontend website
- Added new validation tool config to disable currency formatting of decimal values
- Added requirement for valid currencyCode field+value for Invoices, Receipts and Credit Notes

## [6.7.0] - 2023-09-08
### Changed
- Significant overhaul of the new (Beta) tables interface to improve stability and user experience

## [6.6.0] - 2023-09-05
### Added
- Added setting to workspace settings allowing users to control the sensitivity of the document splitting model

### Changed
- Enable users to zoom in on documents in the splitting interface by clicking on the thumbnail

## [6.5.0] - 2023-09-04
### Added
- Allow users to see when non-base extractors were last trained
- Allow users to control if a collection trains its (non-base) extractor
- Add field and datapoint to the annotation deleted front-end event.

### Fixed
- Fixed issue with new table fields not displaying correctly in the field config editor

## [6.4.0] - 2023-08-23
### Added
- Stabilization for search scores.

## [6.3.21] - 2023-08-21
### Fixed
- Fixed custom receipt table parsing

## [6.3.20] - 2023-08-21
### Fixed
- Improve document upload experience in free tool
- Allow users with customised models to parse at a higher rate

## [6.3.19] - 2023-08-19
### Fixed
- Significant speed improvements for parsing with OpenAI

## [6.3.18] - 2023-08-17
### Fixed
- Fixes to bullhorn integration authentication flow

## [6.3.17] - 2023-08-16
### Fixed
- Minor bug fixes

## [6.3.16] - 2023-08-16
### Fixed
- Minor bug fixes

## [6.3.15] - 2023-08-16
### Fixed
- Minor bug fixes

## [6.3.14] - 2023-08-16
### Fixed
- Small fixes to frontend tool UI
- Fix for bullhorn authentication flow

## [6.3.13] - 2023-08-16
### Added
- When a model is fine-tuned, we now reparse up to 100 unvalidated documents to take advantage of the improved model

### Changed
- Fine tuned improved document classifier

### Fixed
- Improved stability of magic tables interface for non-invoice document types

## [6.3.12] - 2023-08-15
### Fixed
- Better error handling
- Improved table detection

### Added
- Free tool improvements

## [6.3.11] - 2023-08-14
### Fixed
- Backend bug fixes relating to annotation display for rotated documents

## [6.3.10] - 2023-08-11
### Fixed
- Improved GPT error handling

## [6.3.9] - 2023-08-10
### Fixed
- Minor backend fixes

## [6.3.8] - 2023-08-10
### Fixed
- Fixed issue where identical annotations on different pages were not being rendered

### Added
- Automatically close field editor when drawing new annotations
- Improved performance for detecting large text spans with openAI

## [6.3.7] - 2023-08-10
### Added
- Allow magic table fill to be turned off at a workspace level by administrators

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
