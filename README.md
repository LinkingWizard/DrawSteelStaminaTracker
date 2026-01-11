Draw Steel Companion – Stamina Tracker

Usage
1. Enter the character's maximum stamina in the Max Stamina input.
2. Adjust stamina via the input box and Apply button.
3. Use +1/+5/+10 buttons to add temporary stamina.
4. Press "Reset Temp Stamina" to clear temp stamina.
5. Press "Recover" to regain stamina according to your recovery value.
7. Press "Reset Stamina" to restore base stamina to max and clear temp stamina.
8. Observe the stamina bar and condition text to monitor character health.

Max Stamina Input
- Players can set the maximum stamina for their character.
- Adjusting the max stamina does not reset the current base stamina.

Base Stamina Adjustment
- Users can adjust the character's base stamina using the input box.
- Positive or negative values can be entered (e.g., +10, -5).
- Damage is applied to temporary stamina first, then base stamina.
- Stamina can go above the max or below zero.

Temporary Stamina
- Temp stamina can be added using +1, +5, or +10 buttons.
- Temporary stamina cannot go below zero.
- The "Reset Temp Stamina" button sets temp stamina to zero.
- Temp stamina is displayed separately above the base stamina.

Recovery
- The "Recover" button allows spending a recovery to regain stamina.
- Recovery restores one-third of the max stamina (rounded down).
- Recovery cannot raise base stamina above the maximum.
  
Reset Stamina
- The "Reset Stamina" button sets base stamina to max and clears temp stamina.

Conditions
- Based on Draw Steel rules, the app displays the character's condition:
  - Winded: base stamina ≤ half of max stamina.
  - Dying: base stamina ≤ 0.
  - Dead: base stamina ≤ negative half of max stamina.
- Condition text is bold; Dying and Dead are displayed in red, Winded in yellow.
- The player can continue adjusting stamina even if Dead.

Stamina Bar
- A horizontal bar represents the current stamina state visually.
- Green: normal stamina above half max.
- Yellow: Winded (≤ half max).
- Red: damage below zero.
- Black: you died, sorry bro.
- The bar dynamically adjusts segment widths and positions to reflect damage, temp stamina, and over-max stamina.

Technical Details
- HTML based, no external libraries required.
- Uses absolute positioning within the stamina bar for segment layers.
- Updates DOM dynamically with `updateDisplay()` function to reflect changes in real time.
- Event listeners handle user input and button clicks.
