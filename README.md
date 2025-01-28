# Project Underground custom card databases for EDOPro

These databases are automatically synchronized with servers. Please keep all bug reports and questions on Discord; do NOT open an issue or pull request. External contributions are not allowed here.

## Guidelines for SQLite3 CDB files

* For new custom cards:
	* All new custom cards should be added to `unstable-custom.cdb`. Cards in this file are considered experimental and may still contain errors.
		* When a card is verified and deemed stable, it can be moved to the stable database for custom cards.

* For fixes to existing custom cards:
	* Changes made to the files in this repository are automatically imported to [the repository the users get updates from](https://github.com/YGOProjectUnderground/Nexus).

### GitHub Actions

Responsible for pushing database updates to the repository the users get updates from.

- When new cards are added or existing cards are updated, the full database is committed and pushed to the repository.
- If a pushed HEAD commit title contains `[ci skip]`, `[skip ci]`, `[actions skip]`, or `[skip actions]`, the update process is skipped.

## Guidelines for passcodes

Custom cards follow a simple passcode format: `2YYYYSSSSS`, where:
- `YYYY` is the current year.
- `SSSSS` is a sequential number assigned to the card within that year, starting from `00001`.

Cards with passcodes aliased to another within the same year are treated as alternate artworks.
