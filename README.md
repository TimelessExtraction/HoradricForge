Horadric Forge

A modern recreation of the classic Diablo II Hero Editor.

Horadric Forge is a portable Windows application and browser-based save editor for Diablo II Classic and Lord of Destruction, supporting game versions 1.00 through 1.14d.

It reads and edits character saves using the file formats, game tables, and gameplay rules of the original patch. From character progression and quests to equipment, runewords, mercenaries, and low-level item generation, Horadric Forge aims to preserve the behavior of each supported version rather than applying modern rules to older saves.

No installation required. Open a save, make your changes, validate the result, and return to the game.

Features
Character Editor

Manage character statistics, progression, and controls from a single interface.

Edit character name, level, and experience.
Set attributes, life, mana, and stamina.
Adjust carried gold and stash gold.
Change difficulty, act, and saved progression.
Validate character values and reject combinations the game cannot load.
Edit skill assignments individually or all at once.
Configure waypoints, skill hotkeys, and mouse skills.
Inspect the underlying save data with the built-in hexadecimal viewer.
Quest and Progression Editor

Edit quest states while respecting the rules and rewards of the selected game version.

Complete or reset quests.
Apply legitimate quest rewards, including skill points and attribute bonuses.
Handle rewards from Lam Esen's Tome and the Golden Bird quest.
Unlock subsequent acts when the final quest of an act is completed.
Update character titles as progression advances.
Validate quest and progression combinations against the selected patch.
Item Editor

Manage equipment and inventory through an interface modeled after the game.

Supported storage and equipment locations include:

Inventory
Personal stash
Horadric Cube
Belt
Equipped gear
Mercenary equipment

Item editing capabilities include:

Create, move, copy, import, and export items.
Change item quality.
Add or modify sockets.
Edit item properties and supported modifiers.
Work with magic, rare, set, unique, and runeword items.
Apply class skill bonuses and patch-specific item properties.
Search for items by name or property using the Find box.

Item properties are resolved using the game tables associated with the save's original patch, helping preserve version-specific behavior.

Legacy Item Generation

Horadric Forge supports the seed-based item generation used by early Diablo II versions.

In versions 1.00–1.06, item saves store a seed rather than every generated property. Horadric Forge reproduces the corresponding item-generation logic so that properties can be regenerated according to the original version's rules.

Generate items for supported early patches.
Reconstruct item properties from saved seeds.
Re-roll eligible items to generate new properties.
Preserve patch-specific item generation behavior.

This functionality is based on analysis of the original game files and item-generation logic for patches 1.00 and 1.06.

Mercenary Editor

Manage hirelings using the mechanics of the character's game version.

Hire and dismiss mercenaries.
Adjust mercenary levels and experience.
Revive fallen mercenaries.
Calculate resurrection costs according to the relevant patch.
Apply patch-specific mercenary experience formulas.
Character Summary

Review calculated character statistics in one place.

The Summary tab calculates and displays:

Defense
Resistances
Damage
Attack rating
Relevant breakpoints

Use it to inspect a character's build and understand how edited equipment and statistics affect the resulting character.

Save Validation

The Check tab compares a character against the rules and constraints of its corresponding game version.

Detect invalid or inconsistent character values.
Identify data that does not match the selected patch's rules.
Offer one-click fixes for supported validation issues.
Help prevent edits that would produce a character the game cannot load.

Validation is designed to be patch-aware rather than relying on a single set of modern rules for every save.

Backup and Reload

Protect your original character files while editing.

Create a backup for each save before modifications.
Reload a save from disk after playing the game.
Re-read the file to pick up changes made outside the editor.

Recommended practice: Keep independent backups of important characters before making extensive changes.

Supported Versions

Horadric Forge is designed to support Diablo II save files across the following version range:

Game	Supported versions
Diablo II Classic	1.00–1.14d
Diablo II: Lord of Destruction	1.00–1.14d

Each supported patch uses its own file-format handling and game data where required.

Version-sensitive behavior includes item properties, item generation, character progression, mercenary experience, and revival costs.

Exact feature coverage may vary by patch. Consult the project's compatibility documentation and test results for detailed per-version support.

Getting Started
Windows
Download the appropriate Horadric Forge release.
Extract the application if it is distributed in an archive.
Launch the executable.
Open your Diablo II character save.
Select the tab for the data you want to edit.
Review validation results before saving your changes.
Launch the matching Diablo II version and verify the character in-game.

Horadric Forge is designed to run as a portable application without a conventional installation.

Open the hosted Horadric Forge web application.
Load a supported character save.
Make the desired edits.
Validate and save the resulting character file.
Place the edited save in the appropriate game save directory.

Browser file access and download behavior depend on the browser and hosting environment.

Important: Always use a game version compatible with the save you are editing. Keep backups of your original saves, especially when working with legacy patches.
How It Works

Horadric Forge combines patch-aware save parsing, game data, item-generation logic, and character validation.

At a high level, the workflow is:

Identify the save version and select the appropriate parsing rules.
Read character and item data from the original save format.
Load the corresponding game tables for version-sensitive properties.
Apply edits through the character, quest, item, or mercenary interface.
Validate the result against the selected patch's constraints.
Back up and write the save, preserving a recovery path for the original character.

For early versions that use seed-based item storage, item properties are reconstructed using the corresponding generation rules rather than treating the save as if it contained all modern item attributes.

The Hex view provides access to the underlying file data for low-level inspection and troubleshooting.

Design Principles

Horadric Forge is built around a few core principles:

Historical accuracy: Use the rules and data of the character's original patch.
Patch awareness: Avoid applying one version's assumptions to every save.
Practical editing: Provide an accessible interface for both character and item management.
Validation first: Catch unsupported or impossible combinations before they cause problems in-game.
Recoverability: Maintain backups and support reloading files after gameplay.
Portability: Make save editing available without requiring a traditional installation.
Project Status

Horadric Forge is intended to cover character editing, item manipulation, mercenary management, character calculations, and save validation across the supported Diablo II version range.

For each release, the project's compatibility notes should document:

Tested game versions
Supported save formats
Item-generation coverage
Known limitations
Validation behavior
Outstanding compatibility issues
Contributing

Contributions that improve compatibility, correctness, usability, and testing are welcome.

Useful areas for contributions include:

Save-format research and documentation
Patch-specific game table verification
Item-generation tests
Character and mercenary calculations
Validation rules and regression tests
User interface improvements
Bug reports with reproducible save-file examples

When reporting a compatibility issue, include the game version, whether the save is Classic or Lord of Destruction, the affected feature, and the steps required to reproduce the problem. Do not publish personal or otherwise sensitive files.

Disclaimer

Horadric Forge is an independent community project and is not affiliated with, endorsed by, or supported by Blizzard Entertainment.

Diablo II and Diablo II: Lord of Destruction are trademarks of their respective owners. Use the editor with legally obtained game files and keep backups of your character saves.

License

The project's license has not been specified here. Add the applicable license and any required notices before distributing the source code or binaries.
