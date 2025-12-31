SEPSIS V1 1.5.12.31.25.1 (1.5 Update)
Update Pushed on 31 December, 2025 
Bjørn - Jernbjørn Kollektiv - Team Titanium

--------------------------------------------
KEY FEATURES
--------------------------------------------

- Enhanced Enemy Thinking
- Enemy Detection, Scouting, Searching, & Cover AI
- Enemy Pathfinding AI
- Plate Carriers, Chest Rigs, Armor Plates, and Utility Pouches
- Cars and Chinook

--------------------------------------------
COMPLETE CHRONOLOGICAL CHANGELOG
--------------------------------------------

- Added new enemy trait "Inquisition" which determines what they do when detecting nearby noise
- Added unique enemy FOV, Visual Depth, Visual Acuity, Listening Range, & Listening Depth which affect player detection
- Doubled the height of the sound level bar
- Enemies look in the direction of any sound they detect
- Dropping and throwing items now produces a sound

- Improved muzzle flash lighting
- Added atmospheric default lighting to the gun room
- Added FOV detection to enemies
- Added line-of-sight obstruction for enemies so they cannot see through walls
- Enemies now point in the direction of the detected player
- Improved debug FOV visuals

- Enemies now delay being alarmed by visual detection based on visual acuity stat
- Enemy acuity delay quickens if the player is closer
- Added visual acuity representation for enemies in debug
- Added "team-play" trait to enemies which determines how well they work with their teammates
- Enemies no longer detect when incapacitated
- Added dynamic pathfinding to enemies
- Enemies automatically engage detected player
- Rebalanced sound and noise detection

- Rebalanced sprinting heartrate increase per second
- Added top speed and engage distance to enemies
- Added enemy scouting
- Added enemy searching

- Started setup for enemy cover system

- All walls have dedicated cover locations
- Added primitive cover seeking function for enemies

- Enemies now take cover when shot at
- Enemies move between cover if their spot is discovered
- Enemies pathfind to the most ideal cover location when necessary
- Allowed bullet passthrough across cover overlays (bug)

- Enemies no longer spin when incapacitated
- Enemies hit with grenades can no longer crash the game
- Enemy damage from grenades significantly reduced temporarily
- Fixed issue where enemies scouting for player would loop through prior path
- All ammo now have individual object-penetration (separate from flesh penetration) values
- Reduced grid-size for both the VZ-58 and VZ-54 in-inventory by 1 row from the bottom
- Player now gets adrenaline rush from seeing ACTIVE enemies, not test dummies
- Fixed bug where liquids could be transferred and exceed carrying capacity
- Added visual representation of pills in water bottle
- Added gas can
- Added gasoline liquid
- Player dies if they drink gasoline
- Can apply gasoline to medical items
- Added flammability to wounds
- Applying gasoline to open wounds increases flammability
- Areas with high flammability can ignite when shot
- Ignited body parts increase treatment level but cause burning based on flammability
- Added cauterization function

- Fixed bug which did not allow player to drink gasoline
- Added car object & sprite
- Pouring sound actually stops when done pouring
- Added gas fill sound
- Added ability to open gas tank of car
- Added ability to fuel car
- Player can enter car
- Player can accelerate, brake, steer, drift, and reverse car
- Added car lighting
- Added car ignition

- More accurate car steering based on straightening out wheels after turn
- Just headlights flicker on during ignition
- Car reverses accurately based on direction of wheels
- Temporarily disabled physics until resolving bullet velocity issue

- Added halogen flicker sound
- Fixed physics issue where bullets were affect by room-physics
- Car now runs off of traditional velocity system instead of room-physics
- Main music has been reduced in volume
- Car idle sound amplified
- Backup lights now light when braking (even when still maintaining forward velocity)
- Fixed one of the songs being the car ignition
- Idle sound dynamically changes in pitch based on speed
- Added ground friction for car
- Added engine sputter on low fuel
- Added fuel usage
- Added engine sputtering on empty tank
- Car cannot drive on an empty tank

- Speedometer and fuel gauge read more accurately with the dials
- Added RPM dial
- Added car RPMs
- Added car gear
- Pitch of engine blips with gear shifts
- Car automatically shifts at red-line
- Added idle RPM flutter
- Car has a different resistance of friction when accelerating allowing it to still reach max speeds
- Car has RPM resistance which enables it to struggle to get up to higher speeds
- Sudden steer changes are smoother
- Better engine-off sound
- Overall smoother handling changes
- Added startup dial loading

- Made the door a separate component of the car
- Made the gas cap a separate component of the car
- The door can open and close when individually hovered on
- The gas cap can be opened and closed individually
- To enter the car, the door must be opened (left click) and then the main car left clicked
- To fill the car, the tank must be opened (left click) and then the main car left clicked (held)
- To exit the car, simply left click
- Changed visual hover outline and parameters
- Car now no longer rolls after re-entering car from previously high speeds
- Player no longer gets stuck after exiting vehicle
- Changed color of fuel gauge ticks

- Car speed is now dependent on FPS, so it is proportional no matter framerate
- Gamepad controls no longer interfere with main controls

- Changed inventory handling slightly so in-mouse item goes back to in-hand if left click is released (drag & drop vs pickup putdown)
- All inventory functions have been converted to drag and drop
- All box-colliding armor interactables now have distinct objects that allow for more dynamic use and optimization without tracking mouse
- Slight visual size increase when items are inside inventory grid
- Slightly changed collider for gun-rack

- Fixed coat armor-interactive pickup bug
- Added plate carrier slot in inventory
- Fully implemented plate carrier slot
- Added Hacksaw Plate Carrier item
- Fixed issue with transferring items to different hands with new drag and drop in-inventory system
- Clothing items now appear correctly on-hover in-inventory
- Added simple modifier allowing only certain items to go in plate carriers
- Added NIJ-III Polyethylene Armor Plate
- Added "(+{number})" on descriptor for armor protection for plate carrier that changes based on the plate currently in the carrier

- Rebalanced damage for bullet impacts
- Plate carrier protection has been fully implemented
- Multi-layer torso protection improved drastically
- Numerous multi-layer torso protection bugs have been solved
- Added the Yetti plate carrier, designed for tundra performance and protection

- Added mag pouch
- Added small mag pouch
- Mag Pouches are plate carrier applicable
- Frameworked magazine-holding system for mag pouches

- Mag pouches can now be right clicked in the plate carrier to either insert or remove a magazine
- Added orange outline to show that magazine can be put in pouch
- Magazines have size values
- Small magazines can fit in both pouches while medium can only fit in regular sized ones
- Large magazines (none added yet) do not fit in either pouch
- Added framework sprites for new armor plate types and levels

- Resized plate carrier in-hand and in-inventory and in-grid sizes
- Resized armor plate size in-hand and in-inventory
- Added the POLY-IIIA, POLY-III+, KEV-II, KEV-IIA, KEV-III, STEEL-IV, TITAN-IV, and CERAM-IV Armor Plates
- Added fragility to armor plates which determines their level of damage from bullet impacts
- Fixed bug where car did not slow due to friction when neither accelerating nor decelerating
- Improved friction mechanic
- Improved car handling
- Car friction based on FPS
- Fixed crash when being shot wearing plate carrier without armor plate
- Recolored armor plates for designation

- RPM now takes time to shift down dial instead of instantly moving to 0 on shift
- Items with liquid content now display in-inventory with corresponding background
- Lowered muzzle velocity of VZ54 so it actually damages
- Dropping bullets plays a different sound
- Bullet shell drop dynamically plays when fired
- Bullet shell drop quieter in detection
- Added arm stamina
- Arm stamina now lowers when aiming
- As arm stamina lowers, shake becomes larger
- Lowered maximum shake from 10 to 4
- Continued updating player guide
- Moved around room
- Removed lighting in gun room
- Resprited some gun components

- Added chinook for later implementation

- Chinook functionality implemented
- Added Chinook gas tank
- Added Chinook door
- Revised Chinook movement
- Added unique Chinook startup
- Added antialiasing to settings