# Mana System for DnD

Level-up your gameplay by putting the outdated spell-slot system aside and embrance Mana! Use Mana to cast spells in place of spell-slots, use magical weapons and trinkets, and every other item imaginable. Infinitely customizable, robust, and designed with an install-and-forget principle in mind.

Make spellcasters feel deadly again by allowing them your players - and villains - to utilize their most powerful and terrifying magic more often! Make magic even more interactive with Mana Recovery mechanics, and create scenarios where conditions affect the mana reserve!

Unlock an entirely new way to experience magic.

## Features
- Infinitely customizable Mana reserve calculation: 4 preset formulas and write-your-own!
- Non-interfering: Cast With Mana or Cast with Spellslots!
- Automatic Mana cost calculation for spells, weapons, and items!
- Blood Magic: use health to cast spells in place of mana! (also known as Health-as-Mana)

<img src="./src/assets/readme/character_preview.png" width="620px">

## Instructions
### Add Mana Cost
- Go to the Item's **Details** tabs and scroll all the way down.
- In the **Mana Section** enable **Active Effects**.
  
  If the item is a spell, then the *Automatic Mana Cost* cost is automatically added.  
  Customize how much Mana and Health the item costs by using the small plus (**+**) button on the right hand side of each section.

<img src="./src/assets/readme/enable_mana_item.png" width="620px">

### Hiding Spell slots
If you wish to hide the Spell Slot options from item usage dialogs, you can select the *Hide the "Cast With Spellslots"* option in the module's settings page.  
This will keep spell slot-related functionality enabled, but it will hide any visual clutter making the UI a lot cleaner.

<img src="./src/assets/readme/hide_spellslots.png" width="620px">

### Understanding Customization Options
Mana System offers an incredible level of customization. The module has an number of small fields and values that can be fine-tuned to make it behave exactly as you desire. As a result, for new users this amount of information might be overwheling. Each section and their respective settings are as follows:

> Note: if the "Use Default Mana System Settings" option is enabled, most options will have the default value locked. If you want to customize these values, make sure to disable this setting first.

#### Formula
This section controls the universal formula that is used to calculate a character's max mana reserve. There are 4 preset formulas (A, B, C, and D) and a final custom formula (CUSTOM). All variables of the preset formulas can be customized from the settings page.

The custom formula allows you to write your own formula using [Foundry's Formulas](https://foundryvtt.com/article/dice-modifiers/) notation. This means you can use rolls and reference attribute using `@attribute` like your normally would inside Foundry.

<img src="./src/assets/readme/settings_2.png" width="620px">

#### Base Stats
This section controls the base mana and mana growth for all characters, regardless if they use magic or not. You can also control how much each ability score contributes to calculations.

#### Racial Modifiers
This section controls modifiers that are specific to the Race of a character. It allows you to make it so that different races start with a different amount of base mana, and have a different mana growth per level.

In the *Identifier* field of the table, make sure to include the **race identifier** of the race you want to add. You can group races together by separating them with a comma (`,`), but make sure not to include any other special characters.

<img src="./src/assets/readme/settings_3.png" width="620px">

#### Upcasting
This section controls the amount by which upcasting is calculated.

#### Health as Mana
This section controls the Health-as-Mana (also known as *Blood Magic*) part of the module. You can toggle this feature by default for all characters, and set the universal health-to-mana conversion ratio.

#### Recovery
This section controls recovery percentages for several actions a character can take, such as resting.

#### Automatic Cost
This section is probably the most advanced and intricate. It controls how mana cost for items is automatically calculated. It has a number of fields organized in categories that you can tweak.

> Note: most values are *multipliers* any changes are very sensitive. As such, increasing a value from `1` to `1.2` might effectivelly make an item `20%` more expensive. Try to experiment with small changes when you tweak these settings.

#### Base Spell Cost
This section is the one most dungeon master's will probably want to experiment with when installing the module for the first time. This section has the Mana cost equivalent for every spell level. This setting is universal, and also functions as the base in automatic calculations before any modifiers or multipliers are applied.