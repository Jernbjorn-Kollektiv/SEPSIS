 January Monthly Build

 - Lower consciousness now blurs the screen
 - Lower consciousness now hazes the screen
 - If consciousness is below 10%, it will increase by 0.025% per second
 - Consciousness increases by (1/consciousness)% per second if lower than 50% and greater than 10%
 - If consciousness is 0%, a dark haze will fade from the screen and a large ring will fade out
 - Player drops items in hands upon being between 0-10% consciousness and cannot pick them back up until they return to over 10% consciousness
 - Attempting to grab items while still incapacitated will result in them being thrown around you within a 100 pixel radius randomly (unable to pick up items while near unconscious)
 - The pickup threshold distance is now the same as the drop distance (defaults 100 pixels)
 - The mouse goes gray when your mouse is too far away to drop or pickup items
 - If consciousness exceeds 0.04 * (blood_levels - 2500) then it is set to that
    - This results in 100% consciousness at full blood levels and 0% consciousness at 2500 mL or less
 - Player dies outright after blood levels are 2000 mL or lower
 - Headshots will always result in incapacitation
 - Headshots that damage the brain (50% chance) will always result in death
 - Death screen no longer transparent

 - Headshots have a 50% chance of fatality
 - Incapacitations produce a recovery time of (bullet SP+weapon SP) minutes
 - Overkills produce a recovery time of (bullet SP+weapon SP)*2 minutes
 - Player now takes a 'recovery time' after being shot to return back to above 10% consciousness where they can then proceed normally
 - The bleed-out time estimate on the quick-stats bar now registers in minutes and seconds instead of just seconds
 - Added consciousness bar to quick-stats

 - Fixed a bug where bullets that did not cause immediate incapacitation but lowered consciousness to 0 resulted in the ringing sound playing infinitely
 - Bullets that injure the player but cause unconsciousness now also have recovery time
 - Recovery time for injuries causing incapacitation now half that of immediate incapacitation
 - Item labels are not visible during recovery state
 - Lowered intensity of consciousness visual artifacts
 - Added ripple effect during lowered consciousness 
 - Recovery countdown is now precise per frame
 - Your consciousness cannot exceed 100-tiredness

 - Added venous fluid variable (max 2 Liters [2000 mL]) starting at 0
 - Oxygen can not exceed your remaining blood volume %
 - Organ and limb max conditions cannot exceed your remaining blood volume + additional venous fluid volume %
 - Venous fluids now display on quick-stats bar
 - Venous fluids now display textually on quick-stats blood inspection
 - Venous fluids are displayed alongside blood in main-stats screen
 - Venous fluid visuals now fit next to blood-level main stats and quick-stats
 - Venous fluids dynamically dissipate if blood levels + venous fluids exceed 5000 mL (5 L)
 - Venous fluids naturally diffuse to other layers by around 0.28 mL per second
 - As venous fluids diffuse, thirst increases by about 0.14 mL per second
 - Fixed a bug where healed bleeds closed the wound
 - Wounds cannot be infected for 6-wound_intensity minutes after opening
 - Foods now add to a 'digestion array' after being consumed
 - Foods now dynamically dispense nutrients into the body after consumption
 - Foods have a 1 minute delay before dispensing nutrients
 - The apple and orange take 1 minute to fully absorb all of their nutrients after consumption

 - Swapped 'Bruising' and 'Irradiated' limb damage locations
 - Fixed damage-testing interface keybinds
 - Added algorithm to keep the limb-damage and bone-damage interface on-screen no matter mouse position
 - Extended blood-damage and extended infection damage screens now always visible next to main damage panels
 - Removed damage-selection panel
 - 'Irradiated' damage now has 3 levels (Alpha, Beta, and Gamma)
    - All radiation levels now also have additional dialogues
    - Radiation damage now has an extended damage-inspection box
 - Added 3 burn types (1st, 2nd, 3rd)
    - All burns have additional dialogues
    - Burn damages have an extended damage-inspection box
 - DU ammunition now does Alpha Radiation Damage to hit area
 - Radiation and Burns now dynamically do limb/organ damage over time

 A complete redo of the inventory system, converting it into a grid-based system 

 - Moved objects in room to original positions
 - Reset blood levels to max and supporting fluid levels to 0
 - Resprited the trigger
 - Repositioned the origin of the gun component sprites
 - Fixed gun component sprite collisions
 - Resized optics on grid
 - Resized gun components on grid
 - Resized all gun component close-ups on inspection
 - Fixed bug where if there was multiple of the same item in a grid set then it would move other items when picked up
 - Fixed suppressor durability not showing on hover in-hand
 - Fixed right-hand field strip not showing disabilities next to component
 - Fixed right and left hand field stripping bugs/crashes
 - Fixed right and left hand component swapping bugs/crashes

 - Improved contaminant every-second damage functions
 - Added bullet, shrapnel, glass, birdshot pellet, buckshot pellet, alpha hot particles, beta hot particles, and gravel contaminants
 - Moved radiation contaminant extended dialogue next to bleed extended dialogue
 - Added extended dialogue for contaminants
 - Added 'size' attribute to all contaminants
 - Added minor addition to contaminant description in main health dialogue
 - Hot particles (A & B) dynamically cause radiation damage persistently until removed
 - Bullets that do not pass through the body produce bullet contaminants
 - All the parts of a contaminant must be removed before it is fully remedied 
 - Additional testing controls

 - Added 'whole-body' tab to health-screen
 - Changed 3 dot counter in inventory to 2 dot counter
 - Changed 3 dot counter in health to 4 dot counter to add new 'whole-body' tab
 - Added lead poisoning, fever, sepsis, heatstroke, delusional, acute radiation sickness (alpha, beta, and gamma), anaphylactic shock, dyspnea, shock, food poisoning, and hypothermia conditions
 - Added A+, A-, B+, B-, AB+, AB-, O+, and O- blood type, & body temp & heart rate persistent conditions
 - Fixed bug where 2 health manager objects existed at once
 - Conditions (persistent and non-persistent) are drawn on the 'whole-body' health screen tab
 - Tab-navigation for inventory only works when in-inventory
 - Tab-navigation for health only works when in-health
 - Changed speedloader origin and size on grid (1x2)
 - Bone, organ, and limb tangible extended-health menus now have opaque blue background

 - Fixed armor-label for shouldered weapons back to gun sprite
 - Resized backpack to 13x13
 - Added bar selection when inventory is open to select what type of items to see
 - Bar selection can be clicked to display items of a certain type
    - All
    - Firearms, melee weapons, grenades, scopes, sights, suppressors, and underbarrel items
    - Ammunition, boxes, magazines, and speedloaders
    - Food & Beverages
    - Medical items
    - Documents
    - Clothing/armor
    - Weapon components
    - Resources
    - Misc.
 - Non-selected item types are greyed out
 - Resized gun component sprites on grid
 - Moved gas mask sprite origin
 - Fixed gas mask on-player rendering (stretching)
 - Gas mask now a 2x2

 - Extended shifted inventory boundary down by 32 pixels to accommodate for new bar
 - Removed shading for items not of the selected type