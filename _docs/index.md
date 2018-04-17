---
title: Characters
permalink: /docs/home/
redirect_from: /docs/index.html
---

## Character 상속 구조

![logo](https://hwangdaehee258.github.io/ssk.github.io/img/relation ship res 5.png "blueprint relationship")

## Heroes(Player Character)
### BaseHeroBP

BaseHeroBP는 BaseCharBP를 상속 받았습니다. 그렇기 때문에 기본적인 캐릭터 기능을 가지고 있고 추가로 Hero(Player Character) 기능을 가지고 있습니다.
이 블루프린트는 기본 좌우 이동, 멀티 점프, 구르기, 콤보 공격, 아이템 줍기, 피격, 사다리 타기, 벽 타기, 활 쏘기, 무기 바꾸기 기능등을 가지고 있습니다.
 그래서 새로운 영웅 캐릭터를 만들때 이 블루프린트를 상속 받아서 만들 수 있습니다. 샘플로 CouchHeroBP가 있습니다.
 
### CouchHeroBP

기본적으로 제공해주는 영웅 캐릭터 입니다. 이 캐릭터는 BaseHeroBP를 상속 받아서 생성된 블루프린트 입니다. 스켈레톤 메시와 애니메이션, 무기등을 바꿔주거나 추가해 줘서 새로운 Hero(Player Character)를 만들 수 있습니다.

## Monsters
### BaseMonsterBP

BaseMonsterBP는 BaseCharBP를 상속 받았습니다. 그렇기 때문에 기본적인 캐릭터를 가지고 있고 추가로 기본적인 Monater(AI) 기능을 가지고 있습니다. 플레이어가 가까이 왔을 때 쫒아가거나 공격하는 기능을 가지고 있습니다.
완전 새로운 타입의 몬스터를 만들고 싶으면 이것을 상속 받아서 만들 수 있습니다.

### HMoveMonsterBP

좌우 이동하고 플레이어와 충돌 되었을 때 데미지를 줍니다.

### DefaultMeleeMonsterBP
 
근거리 공격하는 기능을 가지고 있습니다. 근거리 공격 몬스터를 새로 만들고 싶으면 이 블루프린트를 상속 받아야 합니다.

### DefaultRangeMonsterBP

### Docs

Docs are [collections](https://jekyllrb.com/docs/collections/) of pages stored under `_docs` folder. To create a new page:

**1.** Create a new Markdown as `_docs/my-page.md` and write [front matter](https://jekyllrb.com/docs/frontmatter/) & content such as:

```
---
title: My Page
permalink: /docs/my-page/
---

Hello World!
```

**2.** Add the pagename to `_data/docs.yml` file in order to list in docs navigation panel:

```
- title: My Group Title
  docs:
  - my-page
```

### Blog posts

Add a new Markdown file such as `2017-05-09-my-post.md` and write the content similar to other post examples.

### Pages

The homepage is located under `index.html` file. You can change the content or design completely different welcome page for your taste. (You can use [bootstrap components](http://getbootstrap.com/components/))

In order to add a new page, create a new `.html` or `.md` (markdown) file under root directory and link it in `_includes/topnav.html`.
