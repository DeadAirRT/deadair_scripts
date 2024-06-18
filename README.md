# Deadair Scripts
## Dynamic Universe
Collection of my custom scripts that aims to reduce the static nature of X4 Foundations and expand the sandbox experience. Readme is often out of date on features or numbers so feel free to contact me on the Egosoft Discord or check patch notes on pushes.
## Menu Option Information
- Most menu entries will display text that may help understand the option or reason when hovered over.
## Dynamic War
- Scripted events at set intervals that change relations between two AI factions. The stronger a faction is, the more enemies it will likely have. The weaker a faction is, the more friends it will likely have.
- Uses the following factors to determine factions selected for event: Accrued chance from times not selected, Military strength, Sectors owned, Primary Race, Current Relations, and Shared Allies/Enemies Count.
- Adjustable interval, event weight, misc factors, and ignored factions.
- Relation change script can be disabled.
- Allows locking / unlocking relations for factions.
- Adds menus for improving or decreasing relations between factions.
- Can earn "favors" from factions that player has 20+ relation with for free relation changes.
- Has optional script that limits positive relation level between two factions to avoid them meeting the "self" requirement for job locations.
- Events for Dynamic War include: Best Friends (Instant max relations), Big Boost (+15 relation), Small Boost (+5 relation), Small Blow (-5 relation), Big Blow (-15 relation), and Nemesis (Instant max negative relations).
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
- Mods now have a chance at increasing travel speed, travel charge time, or max hull.
## Fill
- Adds or removes cargo from Trade Stations, Shipyards, and Wharves at adjustable intervals.
- Can disabled / adjust the adding or removing of wares.
- When wares are removed from Trade Station the faction gains ship mods for a XL/L combat and XL/L economy ship.
## Jobs Expeditions
- Adds fleets and logic for factions to perform similar long range attacks to Terran Interventions.
- Fleets will patrol a critical sector while building up their fleet.
- Fleets will attack the closest sector of one of their enemies that need not border the factions space.
## Jobs Smart Sector Tags
- Adds new logic for determining strategic value of sectors grouped into four categories.
- Critical Sectors contain a ship building station and is owned by the faction.
- Core Sectors contains economic stations, owned by the faction, and does not border enemy sectors.
- Border Sectors contains economic stations, owned by the faction, and borders enemy sectors.
- Contested Sectors contains economic stations of both the faction and an enemy faction.
- Adds adjustable job amounts, job size templates of small/medium/large for each supported faction.
- The ships will patrol a sector that meets the conditions of one of the categories above (Critical, Core, Border, or Contested) and are available to faction logic for invasions.
- Supports increased trade ship and mining ship jobs.
## Gate
- Adds several new gates to the universe. These gates are disabled by default.
- Allows enabling or disabling any gate in the universe.
## God
- Shares the name of previous god.xml mod but entirely separate.
- Adds custom logic for expanding faction economy by setting desired number of production modules to add (and attempt to maintain).
- Does not consider, track, or care about initial module count.
- Default settings are calculated for a stable self-sufficient economy. Data collected over several hundred hours of testing with deadair_eco.
- Option to allow expanding into allied space if no suitable locations are found inside faction owned space.
- Stations are generated using size numbers from deadair_eco. Setting for station max size to be added in future.
- Allows factions to upgrade their shipyard or wharf with additional storage or L production modules.
## Blueprint Analysis
- Inspired by Jack the Strippers mod of the same name. Permission to rework and continue mod granted by author.
- Allows scanning of station modules and ships to gain blueprints.
- User adjustable settings for number of scans required for blueprint unlock.
- Player owned ships performing police behaviour grant credit for scans as well.
- Scan progress is affected by level of scanner on ship. Generic scanner grants one, police scanner grants two, etc.
## Info Menus
- Contains several information menus including military ship count, economic ship/station count, ware stored/wanted information, station resource fullness information.
- Contains menu that tracks and displays ship and station performance.
## Files Adjusted and Possible Conflicts
- All diffs are written to be as compatible as possible but can be broken by terribly written mods that replace more than they should (eg replacing root node). They may cause issues with poorly written mods that do not use specific xpaths.
- aiscripts\order.build.recycle.xml - Removes cover usage for ships enroute to recycle.
- aiscripts\order.move.recon.xml - Adds signalling for when player owned police ships scan.
- libraries\baskets.xml - Only adds to file.
- libraries\equipmentmods.xml - Only adds to file.
- libraries\jobs.xml - Only adds to file.
- libraries\mapdefaults.xml - Only adds to file. May cause issues with other mods that use sector tags for xenon sectors.
- libraries\modules.xml - Removes teladi from refined metals module definition.
- libraries\wares.xml - Only adds to file.
- maps\galaxy.xml maps\sectors.xml maps\zones.xml (split dlc and terran dlc files as well) - Only adds to file. May cause issues with other mods that adjust where zones are placed in sectors.
- md\factionlogic_economy.xml - Only adds to file.
- t\0001.xml - Uses page id 33232474 for entries. Should only conflict with someone who is a little too inspired by DeadAir4.
## Dependencies
- Sir Nukes Mod Support API
- DeadAir Eco (optional but highly recommended)
## Installation Info
- This mod is not compatible and must not be used with the older versions of Dynamic War, Evolution, Fill, Jobs, and Gate.
- Folder should be named "deadair_scripts" in case of added assets in future.
## Requesting Help
- It is very helpful to have a debug log with the debug options enabled.
- Include your mod list in any bug reports. There are a lot of poorly written mods out there.
- Best place to contact me is via @ on Egosoft Discord modding channel.
## Random Notes
- Can't believe I have to add this. No, you are not allowed to just copy my stuff and put it into your own mod or modpack WITHOUT permission.
