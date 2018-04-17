---
title: Characters
permalink: /docs/home/
redirect_from: /docs/index.html
---

## Character 상속 구조



## BaseHeroBP

BaseHeroBP는 BaseCharBP를 상속 받았습니다. 그렇기 때문에 기본적인 캐릭터 기능을 가지고 있고 추가로 Hero(Player Character) 기능을 가지고 있습니다.
이 블루프린트는 기본 좌우 이동, 멀티 점프, 구르기, 콤보 공격, 아이템 줍기, 피격, 사다리 타기, 벽 타기, 활 쏘기, 무기 바꾸기 기능등을 가지고 있습니다.
 그래서 새로운 영웅 캐릭터를 만들때 이 블루프린트를 상속 받아서 만들 수 있습니다. 샘플로 CouchHeroBP가 있습니다.
 
## Writing content

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
