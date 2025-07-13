System Update - Memory, Journaling, Mapping, Patches, & More

- Vsync disabled default
- Constructed base screen for player memories
- Player stats screen now has 3-dot option implementation for multiple pages
- Implemented memory screen into player stats
- Added the "Allergy Test" test memory

- Memories now have dates, text, and more
- All base-visible memory attributes now display
- Memory short/long-term definition displayed as colored dot (orange = short, green = long)
- Trigger sensitivity now no longer displays in-inventory on-hover for firearms
- Resized the VZ58 sprite to save resources and fit new character
- Resized the VZ54 sprite to save resources and fit new character
- Changed rotation of shotgun and bat sprite to match other firearms
- Implemented new sprite centering in-inventory on-hover closeup
- Goliath Red-Dot and Zenith Holosights are now color-coded
- All attachments, sights, and scopes have resized sprites to match the new centered sprite system
- Descriptions now center in-inventory on-hover
- Resized and trimmed all ammo sprites to now fit in-hand and in-inventory on-hover display

- Added images for memories
- Added new draw system for unique font and text modification

- Base memories lengthened
- Formatted coloring and effects for base memories
- Implemented alignment for memory text

- Memory screen now closes when switching back to main health screen
- Added head-injury and world-entry sprite backgrounds for memory screen
- Added blood-test memory
- Can now close all menus with "C"
- Pressing Tab in-health or in-stats causes jump-back to inventory
- Added journal (press "J" to open)
- Memory is now moved to the player journal (page 1)
- Added new journal background UI
- Shifted the memory components over by 32 pixels
- The journal has its own unique font

- Added milestone page to journal which shows kill stats
- Added base map-editing system

- Changed map drawing point to a white dot
- Pen size can be increased/decreased with W and S
- Pen size is proportional to map zoom

- Map now defaults in the middle of the screen
- Each consecutive draw on the map draws on top of that last
- Added full color selection, color display, and size display in-map drawing

- Resprited the overlay for the zenith holosight
- Resprited the 2x scope overlay
- Optics now have dynamic foveation like iron sight
- Added dynamic spriting for broken optics
- Resized collisions for all optic overlays
- In-hand display of condition now colors correctly

- Fixed bug where firearm chamber status was not persistent when swapping the gun between hands by dropping it and picking it back up
- Goliath red dot now fully resprited

- Fixed default bullet speed for the VZ58 from 164 to 64 (like others)
- Added in-engine variable which can turn on and off screenshaking when shooting (defaults on)
- Added in-engine magnitude variable for screenshake when shooting (changed from 15 to default 5)
- Gunshot line now does not extend its X-Scale by 3
- All firearm attachments now reset all modifiers when attached
- A filter now applies to memories which intensifies as their stability lowers
- Memories below a stability of 0 now are forgotten and removed from the memory interface
- Spinning load sign is now a higher resolution
- Redid some loading screen UI elements
- Notifications now have a darker UI background to distinguish it
- Notifications now play sounds depending on their reason for conception

- Reset default health values as preperation for Public Demo 2 in near future
- Load screen has minor additions and changes
- Clock hands have been resized to match the clock face
- Adrenaline is now accurately depicted on the player-energy quick-stat
- Adrenaline can now no longer exceed the maximum player energy
- Fixed some UI texture drawing bugs in fullscreen
