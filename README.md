# rogue-trader-sheet-improved-improved
rogue trader sheet for roll20, modified from a modified sheet

# Why?
The improved sheet under roguetradermago's original repo had some issues I'm aiming to correct, plus some formatting weirdness that was not displaying properly on some browsers.

Most of this is likely going to be for my own usage, but I wanted to have an archive of my edits in case of catastrophe.

# Fixes
- Skillgroups can be rolled now *(see first entry on to-do)* by adding a button to do the rolling. Janky, but it works. Would rather have a click-number like the original sheet *intended*.
- Characteristic advances are no longer misaligned
- Characteristic bonuses are now auto-calculated, with unnatural characteristic support *(but see to-do)*
- Flexbox with vertical table elements ensures that characteristics will remain in their proper places
- ae and oe are replaced with their respective ligatures in html code to make it look a little fancier
- ranged weapon no longer says "shoot" when rolling the template, as the character may be throwing a grenade. New phrasing is more generic.
- some uses of American English are replaced with British spellings *(desirable only because WH40K is made by brits lol)*
- all ampersands and "ands" in raw text are replaced with the html ampersand code. Cleaner and more consistent.
- characteristics and skillgroups (rest of skills are next) are now radios with little purity seals in place of the dots! Also display the name of the rank above the radio. Looks quite nice imo.

# To-Do
- finish skill rank updates to radio inputs with custom dots (spacing and some other aspects are a little strange, so they need to be tweaked)
- Fix weird problem of ``<input>`` tags inside ``<button>`` tags preventing clicking of said button (characteristic rolls, skillgroup rolls). Button added on side of skillgroups as a quick-fix, and it doesn't look *terrible*, but it is still an undesirable solution. Perhaps ``<span>`` tags are a way to go? Initial testing is inconclusive
- set up flexboxes for better sheet viewing in nonstandard viewports
- add a repeatingSum function for ship point calculation
- add method for applying unnatural characteristic and extra characteristic modifiers without it looking convoluted/clunky *(unnatural is* implemented, *but the field is currently hidden and can only be modified through the **Attributes & Abilities** tab of the journal entry for the character)*.
- figure out what to do with the Alt. Career entries that are currently hidden (as they have no use for my players)
- add quantity entries for gear/items
- add entries for power usage/ship points/etc onto weapon batteries for ship such that a placeholder isn't necessary
- style checkboxes for show/hide descriptions to look like buttons