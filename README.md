# element-atelier-img-2

[element-atelier](https://github.com/polos0117/element-atelier) 의 **둘째** 그림 저장소다(2026-11-13 부터 열림).
첫 저장소는 [element-atelier-img](https://github.com/polos0117/element-atelier-img)(0 번, 닫힘 — 이미 있는 이름의 교체만).

## 왜 하나 더 두나

GitHub Pages 사이트 한 개는 1 GB 까지다. 첫 저장소가 거의 차서 **새 그림(webp)은 여기 `img/` 에** 올린다.
앞 저장소의 그림은 지우지도 옮기지도 않는다 — 옛 주소가 그대로 산다.

어느 그림이 어느 저장소에 있는지는 등록기가 `element-atelier` 의 `data/img.json` 에 `"where": {"<파일>": 1}` 로 적고,
화면(`lib/img.js` 의 `BASES`)이 그 번호로 주소를 고른다: `https://polos0117.github.io/element-atelier-img-2/img/<파일>`.

## 자리

```
img/<카드>_<세계>_<화풍>_f.webp       세계 그림 — 파일 이름 규칙은 첫 저장소 README · 코드 저장소 IMAGE_RULES.md 와 같다
img/<카드>_<화풍>_f_casualN.webp      일상컷
img/thumb/<같은 이름>                 목록용. 워크플로가 만든다
```

여기에는 **그림만** 둔다. 기록(`records/`) · 잠금(`records/automation/claims/`) · 배경(`backgrounds/`) · 화풍 비교(`style-test/`)는
첫 저장소에 그대로 둔다(도구들이 거기를 읽는다). 같은 이름의 그림을 두 저장소에 두지 않는다 — 등록기가 멈춘다.

## 올린 뒤에 할 일

없다. `img/` 에 webp 를 올리면 `썸네일` 워크플로가 `img/thumb/` 를 만들어 되커밋하고, 코드 저장소의 `그림 등록` 을 깨운다
(Actions 비밀 `CODE_REPO_TOKEN` — 없으면 코드 저장소가 한 시간마다 스스로 돈다).
