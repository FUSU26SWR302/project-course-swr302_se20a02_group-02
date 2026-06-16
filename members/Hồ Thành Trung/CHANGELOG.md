# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Added
- Completed implementation for `feature-de190928/eKYC-scan-CCCD-CMT`.
- Added database schema updates in `data-sqlserver.sql` for eKYC scanning.
- Created `AI_AUDIT_LOG.md`, `PROMPTS.md`, `REFLECTION.md`, and `CHANGELOG.md` in the `members/Hồ Thành Trung` directory to track AI tool usage.

### Changed
- Updated `.gitignore` to prevent large binary folders (`src/Back_end/jdk21/` and `src/Back_end/maven-bin/`) from being pushed to the remote repository.

### Fixed
- Fixed Git push rejection errors caused by exceeding GitHub's file size limit.

### Removed
- Removed untracked environment and JDK binary files from Git staging area.
