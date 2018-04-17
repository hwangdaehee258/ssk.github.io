---
title: Characters
permalink: /docs/home/
redirect_from: /docs/index.html
---

## Character 상속 구조

![logo](https://hwangdaehee258.github.io/ssk.github.io/img/relation ship res 5.png "blueprint relationship")

### BaseCharBP

HP와 HP를 표시하는 UI와 데미지 이펙트를 가지고 있습니다.

## Heroes(Player Character)
### BaseHeroBP

BaseHeroBP는 BaseCharBP를 상속 받았습니다. 그렇기 때문에 기본적인 캐릭터 기능을 가지고 있고 추가로 Hero(Player Character) 기능을 가지고 있습니다.
이 블루프린트는 기본 좌우 이동, 멀티 점프, 구르기, 콤보 공격, 아이템 줍기, 피격, 사다리 타기, 벽 타기, 활 쏘기, 무기 바꾸기 기능등을 가지고 있습니다.
 그래서 새로운 영웅 캐릭터를 만들때 이 블루프린트를 상속 받아서 만들 수 있습니다. 샘플로 CouchHeroBP가 있습니다.
 
### CouchHeroBP

기본적으로 제공해주는 영웅 캐릭터 입니다. 이 캐릭터는 BaseHeroBP를 상속 받아서 생성된 블루프린트 입니다. 스켈레톤 메시와 애니메이션, 무기등을 바꿔주거나 추가해 줘서 새로운 Hero(Player Character)를 만들 수 있습니다.

![couch_hero_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/couch_hero_bp_icon.png "CouchHeroBP")

## Monsters(AI)

### BaseMonsterBP

BaseMonsterBP는 BaseCharBP를 상속 받았습니다. 그렇기 때문에 기본적인 캐릭터를 가지고 있고 추가로 기본적인 Monater(AI) 기능을 가지고 있습니다. 플레이어가 가까이 왔는지 감지해서 쫒아가거나 공격하는 기능을 가지고 있습니다.
완전 새로운 타입의 몬스터를 만들고 싶으면 이것을 상속 받아서 만들 수 있습니다.

### HMoveMonsterBP

좌우 이동하고 플레이어와 충돌 되었을 때 데미지를 줍니다. BaseMonsterBP를 상속 받아서 만들어진 몬스터 입니다.

![hmove_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/hmove_monster_bp_icon.png "HMoveMonsterBP")

### DefaultMeleeMonsterBP
 
근거리 공격 기능을 가지고 있습니다. BaseMonsterBP를 상속 받아서 만들어진 몬스터입니다. 근거리 공격 몬스터를 새로 만들고 싶으면 이 블루프린트를 상속 받아야 합니다. 

### DefaultRangeMonsterBP

원거리 공격 기능을 가지고 있습니다. BaseMonsterBP를 상속 받아서 만들어진 몬스터입니다. 원거리 공격 몬스터를 새로 만들고 싶으면 이 블루프린트를 상속 받아야 합니다.

### DefaultTypeAMonsterBP

근거리 공격 기능을 가지고 있습니다. BaseMonsterBP를 상속 받아서 만들어진 몬스터입니다. 하지만 공격하는 동안은 피격 동작을 하지 않습니다.

### MannequinMeleeMonsterBP

기본적으로 제공해주는 근거리 몬스터입니다. DefaultMeleeMonsterBP를 상속 받았습니다. 

![mannequin_melee_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/mannequin_melee_monster_bp_icon.png "MannequinMeleeMonsterBP")

### MannequinRangeMonsterBP

기본적으로 제공해주는 원거리 몬스터입니다. DefaultRangeMonsterBP를 상속 받았습니다.

![mannequin_range_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/mannequin_range_monster_bp_icon.png "MannequinRangeMonsterBP")

### MannequinTypeAMonsterBP

기본적으로 제공해주는 TypeA 몬스터 입니다. DefaultTypeAMonsterBP를 상속 받았습니다.

![mannequin_typea_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/mannequin_typea_monster_bp_icon.png "MannequinTypeAMonsterBP")

### BossMonsterS1BP
보스 몬스터입니다. BaseMonsterBP를 상속 받아서 만들어 진 몬스터입니다. 기본 공격뿐만 아니라 스킬공격기능도 가지고 있습니다.

![boss_monster_bp_icon](https://hwangdaehee258.github.io/ssk.github.io/img/boss_monster_bp_icon.png "BossMonsterBP")

