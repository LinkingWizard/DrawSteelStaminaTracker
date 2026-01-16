Draw Steel Companion – Stamina Tracker

Usage
1. Enter required information on launch and press next
2. Press Damage button to open damage menu
3. Press Temp Stamina button to open temp stamina menu
4. Press Settings to adjust Max stamina and recoveries
5. When inputting Damage/Temp Stamina use buttons or enter number into text box
6. Recoveries and Heroic Resources can be adjusted with the +/- buttons
7. Pressing Recover uses one recovery and recovers 1/3 of max stamina.

Max Stamina Input
- Players can set the maximum stamina for their character.
- Adjusting the max stamina does not reset the current base stamina.

Stamina Tracker
- Tracks current stamina relative to max stamina
- Visual stamina bar shows:
  - Green: healthy
  - Yellow: winded
  - Red: dying
  - Black: dead
- Automatically updates condition status
- Current stamina is clamped when max stamina is lowered

Damage System
- “Damage” button opens a dedicated damage menu
- Enter damage via typing or ± buttons
- Damage always removes temp stamina first, then base stamina
- Button controls cannot create negative damage values
- Negative typed values are safely ignored

Temporary Stamina
- Separate Temp Stamina menu
- Adds temporary stamina that absorbs damage first
- Cleanly displayed only when temp stamina is present
- Cannot add negative temp stamina

Recoveries
- Tracks remaining recoveries out of a maximum
- Recoveries are limited and cannot go below 0 or above max
- “Recover” button:
  - Consumes 1 recovery
  - Restores stamina (⅓ of max, capped)
- “Reset” button restores recoveries to max
- Recoveries persist when reopening the settings screen
  
Heroic Resource Tracker
- Simple + / − tracker
- Starts at 0
- Can go negative for strain
- Turns red when below 0

Setup & Adjustment
- On launch, user is prompted for:
  - Max Stamina
  - Max Recoveries
- “Settings” button reopens setup
- Does not reset stamina, temp stamina, or recoveries
- Clamps values if new max is lower

Technical Details
- HTML based, no external libraries required.
- Uses absolute positioning within the stamina bar for segment layers.
- Updates DOM dynamically with `updateDisplay()` function to reflect changes in real time.
- Event listeners handle user input and button clicks.
