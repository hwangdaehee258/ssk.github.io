---
title: Characters
permalink: /docs/characters/
---

## Character Inheritance Relationship

![logo](https://hwangdaehee258.github.io/ssk.github.io/img/relation ship res 5.png "blueprint relationship")

### BaseCharBP

BaseCharBP has the health system and displaying health and a damage effect.

## Heroes(Player Character)
### BaseHeroBP

BaseHeroBP's parent blueprint is BaseCharBP. It has several additional features. 
This blueprint has basic left / right movement, multi-jump, roll, combo attack, item picking, shooting, ladder riding, wall riding, bow shooting and weapon replacement.
 So when you create a new hero character you can inherit this blueprint. A sample blueprint is CouchHeroBP.
 
### CouchHeroBP


It is a hero character that basically provides. This character is a blueprint created by inheriting from BaseHeroBP. You can create a new Hero (Player Character) by replacing or adding skeleton meshes, animations, weapons, and more.

![couch_hero_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/couch_hero_bp_icon.png "CouchHeroBP")

## Monsters(AI)

### BaseMonsterBP

BaseMonsterBP inherits BaseCharBP. So, it has basic character function and it has additional basic Monater (AI) function. It has the ability to detect when a player is nearby and follow or attack.
If you want to create a completely new type of monster, you can create it by inheriting it.

### HMoveMonsterBP

HMoveMonsterBP move left and right and deal damage to the player character. This monster is created by inheriting BaseMonsterBP.

![hmove_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/hmove_monster_bp_icon.png "HMoveMonsterBP")

### DefaultMeleeMonsterBP

DefaultMeleeMonsterBP can use a melee attack weapon. This monster is created by inheriting BaseMonsterBP. If you want to create a new near-attack monster, you can inherit this blueprint.

### DefaultRangeMonsterBP

DefaultRangeMonsterBP can use Ranged attack weapons. This monster is created by inheriting BaseMonsterBP. If you want to create a new ranged monster, you can inherit this blueprint.

### DefaultTypeAMonsterBP

DefaultTypeAMonsterBP can use a melee attack weapon. This monster is created by inheriting BaseMonsterBP. However, it does not play a impact animation during an attack.

### MannequinMeleeMonsterBP

MannequinMeleeMonsterBP is created by inheriting BaseMonsterBP.
It is example blueprint.

![mannequin_melee_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/mannequin_melee_monster_bp_icon.png "MannequinMeleeMonsterBP")

### MannequinRangeMonsterBP

MannequinRangeMonsterBP is created by inheriting BaseMonsterBP.
It is example blueprint.

![mannequin_range_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/mannequin_range_monster_bp_icon.png "MannequinRangeMonsterBP")

### MannequinTypeAMonsterBP

MannequinTypeAMonsterBP is created by inheriting BaseMonsterBP.
It is example blueprint.

![mannequin_typea_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/mannequin_typea_monster_bp_icon.png "MannequinTypeAMonsterBP")

### BossMonsterS1BP

BossMonsterS1BPis the Boss Monster. This monster is created by inheriting BaseMonsterBP. As well as basic attacks, it also has a skill attack function.

![boss_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/boss_monster_bp_icon.png "BossMonsterBP")

