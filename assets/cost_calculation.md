# Mana Cost
For all percentage cost calculations, the results are rounded _down_ after the final cost is calculated.

## Factors that influnce Mana cost
### List of factors
- [Item Type](#item-type)
- [Activation Cost](#activation-cost)
- [Target](#target)
- [Range](#range)
- [Duration](#duration)
- [Effect](#effect)

## Item Type
### Weapon Mana Cost
Weapon mana cost depends on the weapons attributes and the damage it deals, along with any special effects it holds.  
See [Damage](#damage) section.
### Feature Mana Cost
Feature mana cost depends on the effect of the feature.
### Spell Mana Cost
Spell mana cost follows the spell level base cost, along with any modifications made to that based on the the spell's details.

| Spell Level | Base Cost |
| ----------- | --------- |
| Cantrip     | 0         |
| 1st         | 50        |
| 2nd         | 120       |
| 3rd         | 200       |
| 4th         | 290       |
| 5th         | 380       |
| 6th         | 520       |
| 7th         | 760       |
| 8th         | 1100      |
| 9th         | 1800      |
<!-- *Note: press `Alt+Shift+F` to align the table.* -->

## Activation Cost
| Activation Cost | Mana Cost                  |
| --------------- | -------------------------- |
| Action          | Base cost unaffected.      |
| Bonus Action    | Base cost reduced by `10%` |
| Rection         | Base cost unaffected.      |
| Special Action  | Base cost unaffected.      |

## Target
| Target Type | Mana Cost                                                                                                                                                                             |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Self        | Base cost reduced by `10%`                                                                                                                                                            |
| Creature(s) | Single creature: base cost unaffected.<br>Multiple creatures: base cost increased by `2.5%` for every additional creature. If unlimited targets, then base cost is `doubled` instead. |
| Object(s)   | Single object: const unaffected.<br>Multiple objects: cost increased by `0.25%` for every additional object. If unlimited targets, then base cost is `doubled` instead.               |
| AoE(s)      | See [AoE(s)](#aoes).                                                                                                                                                                  |

### AoE(s)
There are many different types of AoE's. Things to consider when determining the cost of an AoE ability are the following:
- Number of AoE(s): single / multiple
- Origin: centered on caster / any other location.
- Shape: circle / line / cone.
- Targets: allies / self / enemies / all creatures.
- Size: radius / length.
- Mobility: stationary / moveable.
#### Number of AoE(s)
For single AoE abilities:
- Base cost increased by `0.5%`

For multiple AoE abilities:
- Base cost increased by `0.5%` times the number of areas affected.

#### Origin
- Originates from the location of the caster
  - Base cost unaffected.
- Originates from a point within range
  - Base cost increased by `15%`
- Originates from any point.
  - Base cost increased by `50%`

#### Shape
- Sphere / Circle
  - Base cost increased by `5%`
- Square / Cube
  - Base cost increased by `3.5%`
- Cone
  - Base cost increased by `2%`
- Line
  - Base cost increased by `1.5%`

#### Targets
- Allies
  - Base cost unaffected.
- Enemies
  - Base cost unaffected.
- All creatures
  - Base cost increased by `5%`

#### Mobility
- Immoveable
  - Base cost unaffected.
- Moveable
  - Base cost increased by `20%`

## Range
### Melee
Touch abilities' mana cost is unaffected.
### Ranged
Ranged abilities' mana cost increased by `5%`

## Damage
- Physical
  - Base cost unaffected.
- Elemental
  - Base cost increased by `5%` for every damage type

## Duration
- Instanteous
  - Base cost unaffected.
- Minute(s)
  - Base cost increased by `1%`
- Hour(s)
  - Base cost increased by `1%` for every hour of duration
- Day(s)
  - Base cost increased by `10%` for every day of duration
- Permanent
  - Base cost increased by `100%`

## Effect
### Action Type
- Melee Attack
  - Base cost unaffected.
- Ranged Attack
  - Base cost increased by `5%`
- Saving Throw
  - Base cost increased by `2.5%`
- Utility
  - Base cost increased by `2%`

### Damage
- Physical
  - Base cost unaffected.
- Elemental
  - Base cost increased by `5%`
- Instakill
  - Base cost increased by `25%`


### Healing
- Regular HP
  - Base cost increased by `2%`
- Max HP
  - Base cost increased by `2.5%`
- Temporary HP
  - Base cost increased by `2%`

### Ability
- Buff
  - Base cost increased by `5%`
- Debuff
  - Base cost increased by `5%`
- Ally buff + Enemy Debuff
  - Base cost increased by `12%`

### Summon
- Temporary
  - Base cost increased by `5%`
- Permanent
  - Base cost increased by `50%`