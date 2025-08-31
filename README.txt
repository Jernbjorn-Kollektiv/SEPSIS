SEPSIS V1 1.4.8.31.25.1 (1.4) - ABS 3.0 Update
Update Pushed on 31 August, 2025 
Bjørn - Jernbjørn Kollektiv - Team Titanium

--------------------------------------------
KEY FEATURES
--------------------------------------------
- Precise-Aim System
- New Bullet Ballistics
- Enhanced Weapon Visuals
- New Player Bullet-Damage System
- New Armor Penetration System
- New Enemy Damage System
- Enemy Combat Personality System (Part 1)
- Rail, Optic, & Mounting System
- Gun Attachment Inspection
- Gas Mask Filter System
- Enhanced Weapon Maintenance, Cleaning, & Repair
- Noise Detection & Suppressor Sound System
- Major Bug Fixes & Quality of Life Improvements

--------------------------------------------
COMPLETE CHRONOLOGICAL CHANGELOG
--------------------------------------------
- Added UI for when aiming at any enemy
- Added line-of-sight system for line-to-wall collisions
- Added UI for 'Precise-Aim,' activated by aiming while hovering on the enemy you want to shoot
- Added bullet height which determines how high the player is aiming
- Enemies now have their own heights and precise-aim sprites that display in the Precise-Aim UI
- Fixed bug which allowed player to equip a sight without removing the already attached one
- Enemies have been recolored for more apparent distinction
- The zenith holosight overlay now displays twice as large
- Optic modifiers now reset when removed to avoid bugs
- Added adrenaline tolerance (over time the player will become used to adrenaline and stimulants will produce less)
- Base Precise-Aim system implemented

- Added bullet drop-off
- Added bullet velocity drop-off
- Rebalanced weapon velocities
- Added trail effect to bullets
- Added damage markers for when enemies are hit by projectiles, showing the elevation at which it hit

- Rebalanced system for bullet drop
- Added sprites for the player holding each type of firearm
- Added new muzzle positioning for more accurate discharge from the end of the barrel
- Added small muzzle explosion and flash

- Screenshake bug fixed when firing firearms
- Added bolt-action open and close animation
- Added pistol chamber animation
- Added rifle chamber animation
- Extended rifle chamber sound to accompany new visuals

- Added shotgun animation open and close animation
- Realigned shotgun open audio to accommodate for new animation

- Added animation for SMG's and Rifles when switching fire modes
- Added visible recoil in hands (bump) when firing weapons

- Added rifle mag remove animation

- Added a new bullet-hit allocator for the player
- Hit-locations now display on the player's body when hit
- Added new impact calculator which determines which limb has been hit

- Changed hit marker image
- Added new damage calculation system for limbs, bones, and organs based on the exact location that was shot
- Changed depth management for organs when hovered over
- Added dynamic clothing damage for new limb damage calculation
- Bones now color blue when hovered on
- Added dynamic recoil that moves the aim height up for every shot

- Changed visuals for health screen slightly
- Changed hover-collisions for health screen organs and limbs
- Added precise-damage for limbs, bones, and organs

- The rate at which aim-height can be adjusted increases with distance to emulate smaller targets further away
- Redid calculation for if the brain is shot
- Damaging pixels now scale based on the stopping power of the bullet
- Damaging pixels now display as light hues around the hit location
- The precise-aim screen now displays for the player-dummy for accurate shot-placement testing
- Reimplemented new penetration system for armors
- Bones now fracture when bullets do not penetrate (from kinetic dump)
- Hit-markers are red when the bullet passes armor and blue if it only hits the player but does not pass
- All limbs and organs now have dynamic bleed calculations (certain areas have higher vascular density now)

- All contact bones from a damaging pixel are now damaged
- Fixed bug where contacted bones would not be damaged any further from rapid-fire after previously taking damage
- Added wound-coverage values to all bullets which affects the size of the damaging pixel when spawned
- Resized the damaging pixel to look smoother at larger sizes
- Grenades now affect the body and are fixed
- Slightly changed death screen
- Fragments of fragmentation grenades have temporarily been disabled

- Fixed bug where brain could not be damaged
- Fixed some small bone-collision bugs

- Fixed the initial coverage of an incendiary blast
- Grenade now fully functional again
- Fixed minimum condition for bones
- Fixed damaging pixel system

- Fixed conditions going into negatives
- Bones can no longer exceed level 5 breaks when shot
- Fixed numerous grenade bugs
- Fixed numerous damaging pixel bugs
- Added back fragments with fragmentation grenade
- Added random fragment height
- Grenades now no longer contaminate wounds with bullets
- Explosive rounds and grenades now burn affected areas
- Added inhibiter so stats can not exceed maximum level bleeding, open wound amount, burning, etc.
- Fixed grenade lag
- Limbs now display colors to show condition
- Limbs no longer heal at 0%
- Limbs black at 0% as early application of dismemberment/crippling
- Fixed radiation sign sizing in-health on-hover for irradiated body parts
- Added secret change to player model in armor-view
- Used lower sized texture models for precise-aim for more adaptability for enemy sprites in the future
- Added new base enemy model
- All current enemies are part of the new Rafnheim Faction
- Added font support for special characters
- Added character name and faction
- Added random name generator for enemies
- Improved visuals for precise-aim UI

- Shifted displaced hit locations over in precise aim UI
- Reevaluated bullet drop factor and distance before drop occurs
- Revised visuals for 2x scope for higher peripheral visibility
- Added peripherals to all sights to distinguish their coverage
- Fixed bug where damaging pixel did not damage multiple organs

- Reintegrated dynamic movement for all the inventory and health UI systems
- Player no longer shifts to 0, 0 when opening any menus
- Player can now be damaged when any UIs are open

- Support for the new UI movement system integrates Journal, Map, and Statistics UIs
- Changed item spawning command in debug to "$spawn.item #" (ex.- $spawn.item 52)
- Added 4 unique AI sections that define their personality and behavior in combat
- Random actions corresponding to certain keystrokes no longer occur when the debug menu is open
- Added faction banners that display next to enemy names
- Added difficult settings configuration file that allows players themselves to alter the gameplay
- Ammo displaying in-hand now disabled by default
- Fixed small loading dialogue bug
- There's now a 1% chance getting shot in the brain will not kill you, in which case a memory will be created of the survival
- In-hand items now no longer display over the journal UI
- Moved room slightly
- Ammo no longer default displays on hover
- Can now do ammo checks on mags and boxes
- Boxes display the exact amount of remaining ammo in an ammo check

- Hand animations now play at a speed based on the game's fps to match with sound
- Precise aim value visibility is now a difficulty option disabled by default
- Added small descriptions to settings in the difficulty settings file for ease of use
- Added ASCII font support for journal font
- Bullets that do not pass through armor now have lower stopping power effects
- Readded new damage calculation to enemies
- New stopping power system in place for enemies
- New armor penetration system integrated for enemies
- Reimplemented blood explosions when the player and enemy are hit
- Improved settings menu
- Default in-game settings menu disabled
- Removed the config file and moved the load buffer setting to the new settings menu

- All guns have either a dovetail, picatinny, or footprint sight rail/mount
- All optics have unique mount preferences
- Optics not matching the guns rail style cannot be placed
- Added the side-mounted rail which allows dovetail weapons to have picatinny sights
- Added ability to attach and remove rails
- The mount style now displays on-hover on guns
- Simplified names for optics
- The 2x scope now only natively works on the VZ54 and VZ58
- Optics, underbarrel, suppressor, and rails now display in-inventory on-hover
- Optics, underbarrel, suppressor, and rails no longer display on-hover in-hand if not applicable
- Sights and scopes can now be placed on ALL weapons as long as the corresponding rail is in place

- Added the crag red-dot optic with a footprint attachment style
- Resized all the optics
- Changed inventory screen slightly so objects no longer blend with background
- Optics and rails can now be detached from all weapons
- Sound now plays when equipping and removing rails
- Added a Base-Footprint rail
- Removed scope on VZ54 base sprite
- Slightly changed side-mount sprite
- Changed 2x scope sprite to show dovetail mount
- Fixed a bug where optics not matching the gun's mount style could still be attached
- Fixed VZ54 being base mounted not dovetail mounted
- Fixed some bugs that would crash the game when getting shot and holding certain items
- Added 'gun-inspection' screen openable with 'G' that shows the gun and its attachments in detail
- Resprited laser
- Resized laser
- Resprited all suppressors
- Recolored spriting on the side mount
- Firing mode can also be changed when the mouse side button is pressed
- Underbarrel toggle mouse keybind swapped to other side button
- Sound now plays when equipping lasers

- Changed death screen slightly
- Added conditions to attachments in gun inspection
- Shake and shake magnitude now defined in settings
- Firearm condition is now the average of all the part conditions and the overall cleanliness
- Fixed some hover-item modifier bugs
- Retitled some modifiers on-hover
- Guns now have cleanliness that will degrade naturally
- Guns will dirty faster if wet due to rusting

- Added passive rusting and dirtying in-hand

- Lowered natural dirtying rate
- Lowered natural rusting rate per level of dampness
- Added passive dirtying and rusting while items lay on the ground
- Guns no longer rust and dirty past 50% condition
- Guns now dirty and rust while being transferred between clothing items and held in the mouse
- Resized the water bottle sprite
- Added G-D 40 Lubricant
- Added toothbrush
- Player can now apply G-D 40  to all attachments. components, and firearms
- Player can brush attachments, components, and firearms
- Brushing firearms will increase their cleanliness
- Brushing components and attachments will increase their condition by a quarter the rate they clean firearms
- Fixed some spriting issues with gun components
- Resprited barrel components
- Fixed component collisions
- Recolored triggers
- Added 'Tool' tab in inventory filter
- Resized misc. items
- Revised collisions on misc. items
- Added multitool
- Multitool can repair components

- Fixed bug where quick-dropped mags could not be reloaded causing crash
- Added ability to slowly unload ammo-boxes with right-click
- Aim height now displays on top of quick stats
- Can no longer attach rails when an optic is already on the firearm
- Resized firearm on-hover box to fit new condition system
- Prepped for tutorial system

- Fixed armor stats not showing on-hover
- Resized aim-height UI
- Armor starts to lose its protection-power as its condition lowers
- Changed the hypothermia condition image

- Gas-Mask now has a filter slot, filter condition, and filter type
- Added the CB54 Filter that can be mounted to the gas-mask
- Renamed gas-mask to CB1.6 Gas Mask (Numbers represent first number times 10 (10) all the way to the second number times 10 (60) compatibility (CB10-CB60 filters)
- Can screw and unscrew filters into gas mask
- Redid some UI elements on-hover for new filter system
- Grid size now displays on-inspection in-inventory instead of CC occupancy for legacy system (outdated)
- Gas Mask Filter condition lowers with use
- Changed sprite for gas mask overlay
- Gas mask overlay now displays filter integrity

- Face clothing items can now be damaged when hit (headshots damage gas mask)
- Added fragility to all armor items so certain ones damage faster

- Main body parts now damage from hits, not just damage over time
- A torso at 0% causes death
- Dismemberment can now only occur from overkill hits
- Added 12 new unique songs
- Player consciousness now no longer dependent on LOWEST condition but now TORSO condition
- 0% condition limbs now remain red and dismembered limbs are black
- Dismembered limbs can no longer be damaged
- Can no longer apply items on dismembered limbs
- Selected limbs and organ names and descriptions display again
- All limbs and bones now have unique descriptions
- Extended attachments corner in room to include new cleaning items
- Added new testing room
- Added gun racks (WIP)

- Guns can now be dropped onto gunracks and automatically placed on
- Field stripping now automatically calculates real condition with new cleanliness system
- Only certain guns can go on racks now
- Fixed Zbrojovka not having cleanliness (0% always)
- Zbrojovka can now be put on racks

- Added a shelf for holding smaller guns
- Shelves can hold pistols and ammo boxes
- Changed gun racks

- Grenades can no be placed on shelves
- Resized in-world toothbrush and GD40
- Added ramrod
- Can clean barrel both in and out of gun with ramrod

- Fixed scope sizing in-inventory on-grid
- Fixed sizing of ramrod in-hand
- Minor change to Z-Rapid Suppressor Sprite
- Baseball bat can now be put on a rack
- Fixed multiple weapon collision masks for higher precision
- Hands default off when no weapon is being held

- Holding C when firing now controls recoil to keep it in the general vicinity of where you shot
- Revalued recoil values for each firearm
- Added a bar which dynamically increases and decreases depending on current sounds
- Player walking, idle, and sprinting have unique sound levels
- Firing, chambering, etc. guns now produces unique sound levels
- Player now shakes with mouse when it moves from shake factors
- Suppressors now lower the net sound value of firearms so they are less detectable
- Fixed depth issues for applied health items