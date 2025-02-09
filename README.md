# Project Underground Custom Card Databases for EDOPro

These databases are automatically synchronized with servers. Please direct all bug reports and questions to [Discord](https://discord.gg/NwPa6mwyYx). Do **NOT** open issues or pull requests on this repository. External contributions are only allowed through the [Discord](https://discord.gg/NwPa6mwyYx) process outlined below.

## Guidelines for SQLite3 CDB Files

* For new custom cards:
	* All new custom cards must be added to `unstable-custom.cdb`. Cards in this file are considered experimental and may contain errors.
		* Once a card is verified and deemed stable, it can be moved to the stable custom card database.

* For fixes to existing custom cards:
	* Any changes made to the files in this repository will be automatically imported to [the repository users receive updates from](https://github.com/YGOProjectUnderground/Nexus).

### GitHub Actions

GitHub Actions handle pushing database updates to the repository where users receive updates.

- When new cards are added or existing cards are updated, the full database is committed and pushed.
- If the HEAD commit title includes `[ci skip]`, `[skip ci]`, `[actions skip]`, or `[skip actions]`, the update process is skipped.

## Becoming a Contributor

If you would like to become a contributor, please join the [Discord server](https://discord.gg/NwPa6mwyYx) and request access in the `#be-a-contributor` channel. Once approved, you'll be assigned a unique contributor number.

You can also connect with other scripters and contributors in the `#card-scripting` and `#database-updates` channels for support and collaboration.

## Guidelines for Passcodes

Custom cards now follow this passcode format: `2UUUSSSSSS`, where:
- `UUU` is the unique contributor number assigned by staff after your request to become a contributor is accepted.
- `SSSSSS` is any sequence number that the contributor desires to use.