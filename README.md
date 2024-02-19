# Deadair Scripts
## Dynamic Universe
Reworked all md based mods and some xml diff based into combined script package. Contains improved versions of Dynamic War, Dynamic News, Evolution, Fill, Jobs Expeditions, Jobs Smart Sector Tags, and Gate. Readme may be out of date on features or numbers at times so feel free to contact me on the Egosoft Discord.
## Dynamic War
- Scripted events at set intervals that change relations between two AI factions. The stronger a faction is, the more enemies it will likely have. The weaker a faction is, the more friends it will likely have.
- Uses the following factors to determine factions selected for event: Accrued chance from times not selected, Military strength, Sectors owned, Primary Race, Current Relations, and Shared Allies/Enemies Count.
- Adjustable interval, event weight, misc factors, and ignored factions.
- Relation change script can be disabled.
- Contains several information menus including military ship count, economic ship/station count, ware stored/wanted information, station resource fullness information.
- Allows locking / unlocking relations for factions.
- Adds menus for improving or decreasing relations between factions.
- Can earn "favors" from factions that player has 20+ relation with for free relation changes.
- Has optional script that limits positive relation level between two factions to avoid them meeting the "self" requirement for job locations.
- Events for Dynamic War include: Best Friends (Instant max relations), Big Boost (+15 relation), Small Boost (+5 relation), Small Blow (-5 relation), Big Blow (-15 relation), and Nemesis (Instant max negative relations).
- Most menu entries will display text that may help understand the option or reason when hovered over.
## Dynamic News
- Collects information from included scripts and events from around the galaxy to provide player with additional information.
- Supported events include: Major station destroyed, Economic station expanded, Economic station started, and Sector changed ownership.
- Outputs news events at adjustable interval and combines multiple reports per faction to avoid spam.
- Can enable/disable the script, notifications, logbook entries, and the recent news database.
## Evolution
- Newly built Xenon ships will have added equipment mods after adjustable intervals determining Xenon evolution level of 1-5.
- At evolution levels 1,3,5 the Xenon will expand their shipyards with additional storage, shipbuilding, and defence modules.
- Adds option for adjustable Xenon Evolution fleets that allow user to choose between small, medium, and large templates.
- Fleets built will patrol a Xenon owned sector bordering an enemy and are available to faction logic for invasions.
- Adjustable option for Xenon to request a single fleet per interval, or one fleet per shipyard (for faster build up).
### Evolution Xenon Ship Mod Stats
- Weapon damage: Min: +5% -- Max: +25%
- Weapon rotationspeed: Min +5% -- Max: +25%
- Engine forward thrust: Min +5% -- Max: +25%
- Engine rotationthrust: Min +5% -- Max: +25%
- Ship mass: Min -5% -- Max: -25%
- Ship drag: Min -5% -- Max: -25%
- Shield capacity: Min +5% -- Max: +25%
- Mining multiplier (eco): Min +10% -- Max: +50%
- Radar range (eco): Min +5% -- Max: +25%
- Radar signature (eco): Min -10% -- Max: -50%
## Fill
- Adds or removes cargo from Trade Stations, Shipyards, and Wharves at adjustable intervals.
- Can disabled / adjust the adding or removing of wares.
- When wares are removed from Trade Station the faction gains ship mods for a XL/L combat and XL/L economy ship.
## Jobs Expeditions
- Adds fleets and logic for factions to perform similar long range attacks to Terran Interventions.
- Fleets will build patrol a critical sector while building up their fleet.
- Fleets will attack the closest sector of one of their enemies that need not border the factions space.
## Jobs Smart Sector Tags
- Adds new logic for determining strategic value of sectors grouped into four categories.
- Critical Sectors contain a ship building station and is owned by the faction.
- Core Sectors contains economic stations, owned by the faction, and does not border enemy sectors.
- Border Sectors contains economic stations, owned by the faction, and borders enemy sectors.
- Contested Sectors contains economic stations of both the faction and an enemy faction.
- Adds adjustable job amounts, job size templates of small/medium/large for each supported faction.
- The ships will patrol a sector that meets the conditions of one of the categories above (Critical, Core, Border, or Contested) and are available to faction logic for invasions.
## Gate
- Adds several new gates to the universe which can be enabled or disabled.
## Files Adjusted and Possible Conflicts
- All diffs are written to be as compatible as possible but can be broken by terribly written mods that replace more than they should (eg replacing root node). They may cause issues with poorly written mods that do not use specific xpaths.
- libraries\equipmentmods.xml - Only adds to file.
- libraries\jobs.xml - Only adds to file.
- libraries\mapdefaults.xml - Only adds to file. May cause issues with other mods that use sector tags for xenon sectors.
- libraries\wares.xml - Only adds to file.
- maps\galaxy.xml maps\sectors.xml maps\zones.xml (split dlc and terran dlc files as well) - Only adds to file. May cause issues with other mods that adjust where zones are placed in sectors.
- md\factionlogic_economy.xml - Only adds to file.
- t\0001.xml - Uses page id 33232474 for entries. Should only conflict with someone who is a little too inspired by DeadAir4.
## Dependencies
- Sir Nukes Mod Support API
- DeadAir Eco (optional and unreleased)
## Installation Info
- This mod is not compatible and must not be used with the older versions of Dynamic War, Evolution, Fill, Jobs, and Gate.
## Requesting Help
- It is very helpful to have a debug log with the debug options enabled.
- Include your mod list in any bug reports. There are a lot of poorly written mods out there.
- Best place to contact me is via @ on Egosoft Discord
