# Resume Guide — Denys Ismaylov, Unity Developer

Гайд по оформлению резюме. Внутри: как сделать так, чтобы оно хорошо парсилось (ATS),
и готовые формулировки по каждому блоку под твой реальный опыт (3.5 года, mobile games).

---

## 0. Как сделать, чтобы резюме лучше парсилось (ATS)

Твой текущий PDF при автоматическом разборе разваливается — разделы перемешиваются.
Это значит, что часть систем (Greenhouse, Lever, Workday, Recruitee) прочитают мусор и
отсеют тебя ещё до того, как резюме увидит человек.

**Правила «ATS-friendly» PDF:**

1. **Одна колонка, а не две.** Многоколоночные шаблоны (как у тебя сейчас: skills слева,
   experience справа) ломаются при парсинге — текст читается построчно слева направо и
   перемешивается. Делай в одну колонку сверху вниз.
2. **Текст, а не картинка.** Убедись, что текст выделяется и копируется из PDF. Если резюме
   экспортировано как изображение (часто бывает из Canva/Figma) — ATS не прочитает ничего.
   Проверка: открой PDF, попробуй выделить и скопировать абзац. Копируется → ок.
3. **Стандартные заголовки разделов:** `Summary`, `Experience`, `Skills`, `Education`,
   `Projects`, `Languages`. Не выдумывай креативные названия.
4. **Без таблиц, текстбоксов, иконок вместо текста.** Контакты — обычным текстом
   (email, телефон, город, ссылки), а не иконками.
5. **Простые шрифты**, без хитрых лигатур. Маркеры — обычные `•` или `-`.
6. **Даты в одном формате:** `2023 – 2024`, `2025 – Present`.
7. **Имя файла:** `Denys_Ismaylov_Unity_Developer.pdf` — у тебя уже правильно.

**Практический вывод:** собери резюме в одну колонку (Google Docs / простой шаблон в Canva
без боковой панели / LaTeX-шаблон вроде `moderncv` в single-column). Экспортируй в PDF
именно как текст. Это самое важное техническое улучшение.

---

## 1. Header

**Фото — нужно ли?**
- Для рынка **СНГ / Польша / Германия / большинство EU-студий** — фото скорее норма, можно
  оставить. Деловое, нейтральный фон, без селфи.
- Для **US / UK / Канада / Нидерланды / Ирландия** — фото лучше **убрать** (анти-дискриминационные
  практики, многие ATS его всё равно вырежут).
- **Компромисс:** держи две версии PDF — с фото (EU/локально) и без (международные отклики).
  Если лень — делай **без фото**, это безопаснее и нигде не навредит.

**Что писать в шапке:**

Только «Имя + Unity Developer» — мало. Добавь подзаголовок с позиционированием и контакты
в строку.

```
DENYS ISMAYLOV
Unity Developer · Mobile F2P (Hyper-casual & Hybrid-casual) · 3.5 years

Warsaw, Poland · ismaylov.den@gmail.com · +380 98 792 75 96
LinkedIn: linkedin.com/in/<...>  ·  Portfolio: <...>  ·  GitHub: <...>
```

- Позиция «Unity Developer» — оставляй, она целевая.
- Вторая строка = твой грейд + специализация. Это сразу отвечает рекрутеру «кто ты».
- Контакты — текстом, в строку, со ссылками (portfolio/LinkedIn/GitHub обязательно кликабельны).

---

## 2. Summary

Цель summary — за 4 строки показать: грейд, специализацию, ключевые технологии и **1 цифру-достижение**.
Не «лью воду» про себя, а факты.

**Готовый вариант (бери и правь):**

```
Unity Developer with 3.5 years of experience building mobile F2P games — hyper-casual,
casual, and hybrid-casual — for Android, iOS, and Amazon (tablets & TV). Shipped and
supported live titles including Street Dude (5M+ downloads on Google Play), built rapid
prototypes to validate gameplay hypotheses, integrated ad/analytics/IAP SDKs, and ported
live projects across platforms with constant performance optimization for low-end hardware.
Comfortable working in unfamiliar codebases and shipping features fast into existing projects.
```

**Короткая версия (если нужно ужать):**

```
Unity Developer, 3.5 years in mobile F2P (hyper-casual, casual, hybrid-casual).
Shipped Street Dude (5M+ downloads), integrated ads/analytics/IAP SDKs, ported live
games to Amazon (tablets/TV) with deep performance optimization, and built battle pass
& new game modes. Fast at picking up legacy codebases and delivering features into them.
```

**Что здесь работает и почему:**
- `3.5 years` — конкретный грейд (Middle-ориентированный).
- `Street Dude (5M+ downloads)` — главное достижение, его обязательно в первые 2 строки.
- Перечислены ровно те вещи, которые ищут вакансии: SDK, optimization, porting, live ops.
- «Comfortable in unfamiliar codebases» — твоё реальное преимущество, ценится для LiveOps.

---

## 3. Что делать с NDA-проектами

Это нормальная ситуация, у 80% game-разработчиков так. Решения:

1. **Называй то, что публично.** `Street Dude` есть в Google Play под издателем —
   значит, его можно называть и линковать на стор. Проверь, что именно публично у каждой
   игры, и называй только это.
2. **Где NDA — описывай тип, а не название.** «a hyper-casual runner with 5M+ installs»,
   «a casual merge title», «live hybrid-casual project». Жанр + метрики + что ты делал —
   этого достаточно, NDA не нарушается.
3. **Метрики разрешено называть почти всегда** (загрузки, +23% LTV, FPS, % оптимизации) —
   они не раскрывают код. Это твой главный актив, не прячь его.
4. **Пет-проект:** старый проект 2-летней давности с неплохой архитектурой — **лучше показать,
   чем ничего.** Не выкладывай как «вот моя гордость», а оформи честно: «Personal project
   demonstrating clean architecture with Zenject DI, [feature]». Можно за пару часов:
   - почистить README (что это, стек, скриншот/гиф, что демонстрирует),
   - убрать мёртвый код,
   - запинить в GitHub.
   Даже средний, но аккуратно оформленный проект показывает, что ты умеешь структурировать код.
5. **Альтернатива пет-проекту, если нет времени:** небольшой **technical write-up** —
   1 страница про реальную инженерную задачу (без NDA-кода): «Как я портировал игру на Amazon
   Fire TV: input remapping, UI под пульт, оптимизация под слабое железо». Это показывает
   инженерное мышление лучше, чем полупустой репозиторий.

---

## 4. Technical Skills

Сгруппируй по категориям — так читабельнее и лучше для ATS (ключевые слова рядом с контекстом).
Убери «процессные» пункты из навыков (Code Review, Agile как навык) — им место в experience.

```
Languages & Core:    C#, OOP, SOLID, Design Patterns, Data Structures
Unity:               Zenject, UniTask, UniRx, DOTween, Addressables, AssetBundles,
                     UGUI, Shader Graph, Editor Tooling, Odin Inspector
Mobile & Platforms:  Android, iOS, Amazon (Fire Tablet / Fire TV);
                     performance profiling & memory optimization for low-end devices
SDK & Monetization:  Ads mediation, IAP / In-App Purchases, Analytics, AppsFlyer,
                     OneSignal, A/B Testing, Battle Pass / subscriptions
Networking & Web:    REST API, UnityWebRequest, WebView integration
Backend & Infra:     AWS (S3, CloudFront), CI/CD
AI-Assisted Dev:     GitHub Copilot, Cursor, ChatGPT — code generation, refactoring,
                     debugging, and faster navigation in legacy codebases
Tools & Process:     Git, Xcode, Agile/Scrum, Code Review
```

> **AI tools — почему стоит указать:** вакансия Plarium прямо требует «практичний досвід
> застосування ШІ-інструментів для оптимізації процесів розробки». Это ключевое слово для ATS,
> а не украшение. Правило: пиши не «использую ChatGPT», а ЧТО это дало в разработке.
> Указывай 2–3 реально используемых инструмента — на собесе спросят, как применял.

**Что добавил/исправил по сравнению с текущим резюме:**
- Поднял `Addressables`, `DOTween`, `UGUI` в явные skills (раньше были только в tech-строках).
- Добавил `UnityWebRequest` / `WebView` — твой реальный опыт из второй компании, важное ключевое слово.
- Добавил `IAP`, `A/B Testing`, `Battle Pass` явно — это ключевые слова вакансий.
- Убрал «Math, Linear Algebra» как отдельный навык (звучит как строка из учебного плана) —
  если хочется, замени на `Game Math` внутри Core.

**Чего у тебя пока НЕТ, но просят вакансии (Plarium / Fishing Planet) — пробелы для роста:**
- `Multiplayer / Networking` (UDP/TCP, Photon/Mirror) — главный пробел для шутеров/мультиплеера.
- `ECS / DOTS`, `Burst` — упоминаются как плюс почти везде.
- `MVVM` как явный паттерн (Plarium просит) — если применял, добавь.
- `HLSL` шейдеры (у тебя только Shader Graph).
- Конкретные профайлеры: `Unity Profiler`, `Memory Profiler`, `Frame Debugger` — назови поимённо.

> Не выдумывай то, чего не знаешь. Но `MVVM`, `Unity Profiler`, `Memory Profiler` —
> если реально использовал (а судя по оптимизации Amazon — да), обязательно впиши.

---

## 5. Experience — готовые формулировки

Принцип каждого буллета: **что сделал → как (технология/подход) → какой эффект**.
Глаголы в прошедшем времени, по одному действию на строку, метрики где возможно.

### Vira Games — Unity Developer · 2025 – Present
*Tech: Unity, C#, Zenject, UniRx, Odin Inspector, Addressables, AWS S3/CloudFront, Editor Tooling, CI/CD*

- Ported live iOS/Google Play titles to the Amazon platform (Fire Tablet & Fire TV),
  adapting input handling, UI/navigation for TV, and store/SDK integration
- Optimized ported games for low-end hardware (tablets/TV): reduced memory footprint and
  stabilized frame rate using Unity Profiler & Memory Profiler
- Supported multiple live projects (LiveOps) with different codebases and architectures,
  shipping features fast into unfamiliar legacy code
- Implemented subscription monetization (battle pass) and new game modes, contributing to
  a ~23% LTV increase across projects
- Built an internal Editor tooling package automating cross-project tasks, reducing
  repetitive setup time
- Adopted AI-assisted tools (Cursor / Copilot) for boilerplate generation, refactoring,
  and debugging — speeding up feature delivery across unfamiliar legacy codebases

> Если LTV +23% и automation package относятся к этой компании — оставь их здесь.
> Если к другой — перенеси. Главное, чтобы цифра стояла рядом с реальной фичей.

### Playnatic — Unity Developer · 2024 – 2025
*Tech: Unity, C#, Zenject, DOTween, AppsFlyer, OneSignal, Xcode*

- Developed gameplay prototypes for casual titles, integrating ad, analytics, and push
  SDKs (AppsFlyer, OneSignal) for monetization and retention testing
- Implemented WebView features via UnityWebRequest to serve remote content and offers
  inside the app
- Built and iterated on game mechanics in short cycles, collaborating with designers and
  artists to integrate assets and polish UX

### 24Play — Unity Developer · 2023 – 2024
*Tech: Unity, C#, Zenject, DOTween, UniTask, Ads, IAP, Analytics*

- Contributed to Street Dude (5M+ downloads on Google Play): implemented core gameplay
  mechanics and meta-game features
- Built rapid prototypes to validate gameplay hypotheses and identify scalable,
  high-retention mechanics
- Integrated a wide SDK stack (ads mediation, IAP, analytics) and ran A/B tests to refine
  monetization
- Worked across a large technology stack, implementing intuitive, easy-to-pick-up mechanics
  for casual players

> Сверь распределение проектов по компаниям — я расставил по твоему рассказу
> (24Play = старт, Street Dude; Playnatic = прототипы + WebView; Vira = Amazon + LiveOps + порт).
> Если в реальности иначе — поменяй местами, формулировки переносятся как есть.

---

## 6. Education

```
M.S. in Computer Engineering — National Technical University of Ukraine "Igor Sikorsky KPI"
2020 – 2025
```

## 7. Courses (бывший «K-Syndicate Courses»)

Расшифруй, что это за курс — иначе строка выглядит загадочно.

```
K-Syndicate — <Unity / Game Development course>, <год>
```

## 8. Languages

```
Ukrainian — Native    English — B2 / Upper-Intermediate
```

- Если реально владеешь английским лучше «intermediate» — пиши `B2 / Upper-Intermediate`.
  Многие вакансии (Plarium, международные команды) требуют именно Upper-Intermediate+.
- `Russian — native` рекомендую **убрать** или не выносить отдельно: для части EU/израильских
  работодателей в текущем контексте это нейтрально-негативный сигнал, а пользы для вакансии не несёт.

---

## 9. Итоговый порядок разделов (одна колонка)

1. Header (имя · Unity Developer · специализация · контакты)
2. Summary
3. Technical Skills
4. Experience
5. Projects (пет-проект + ссылки на сторы)
6. Education
7. Courses
8. Languages

---

## 10. Чек-лист перед отправкой

- [ ] PDF в одну колонку, текст копируется (не картинка)
- [ ] Street Dude (5M+) есть в Summary и в Experience
- [ ] У каждой компании ≥ 3 буллета «действие → способ → эффект», не голый tech-list
- [ ] Vira Games описана (не оставлять пустой!)
- [ ] Есть хотя бы 2–3 метрики (5M+, +23% LTV, FPS/memory, % времени)
- [ ] Ссылки на Portfolio / LinkedIn / GitHub кликабельны
- [ ] English = B2 / Upper-Intermediate (если соответствует)
- [ ] Skills сгруппированы, добавлены Addressables / WebView / IAP / A/B
- [ ] Курс K-Syndicate расшифрован
- [ ] Две версии PDF: с фото (EU) и без (международные) — опционально
