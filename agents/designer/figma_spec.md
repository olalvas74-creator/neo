# Figma-спецификация для ручной отрисовки — NeoFamily Blog

> Версия: 1.0 | Дата: 2026-03-17
> На основе: concept.md v1.1
> FileKey: 2V3f7LR4hyenHFdSdLGArs
> Шрифты: Comfortaa (заголовки) + Nunito (всё остальное)

---

## Глобальные токены

### Цвета

| Токен | HEX | Использование |
|-------|-----|---------------|
| primary | #E9585A | CTA, акценты, прогресс-бар |
| primary-hover | #F27C82 | Hover кнопок |
| primary-active | #D47772 | Active кнопок |
| text-primary | #1D1E1B | Заголовки, основной текст |
| text-body | #333333 | Тело текста |
| text-secondary | #5C5964 | Мета, подписи |
| text-muted | #989898 | Даты, плейсхолдеры |
| text-link | #5CA7D9 | Ссылки |
| bg-white | #FFFFFF | Основной фон |
| bg-light | #F9F8FB | Альтернативный фон секций |
| border-default | #DADADA | Границы полей |
| border-light | #EFEDF2 | Лёгкие разделители |
| success | #A1D236 | Успех, галочки |
| cat-actual | #FFC645 | Категория "Актуальное" |
| cat-ege | #6A5C90 | Категория "ЕГЭ и поступление" |
| cat-bio | #A1D236 | Категория "Биология" |
| cat-chem | #5CA7D9 | Категория "Химия" |
| cat-rus | #E9585A | Категория "Русский язык" |
| dark | #1D1E1B | Footer фон |
| dark-border | #333333 | Footer разделители |
| dark-text | #A5A5A5 | Footer текст ссылок |

### Типографика

| Роль | Шрифт | Вес | Размер | Line-height | Цвет |
|------|-------|-----|--------|-------------|------|
| H1 | Comfortaa | Bold (700) | 36px | 1.2 | #1D1E1B |
| H2 | Comfortaa | SemiBold (600) | 32px | 1.3 | #1D1E1B |
| H3 | Comfortaa | SemiBold (600) | 26px | 1.3 | #1D1E1B |
| Section title | Comfortaa | SemiBold (600) | 26px | 1.3 | #1D1E1B |
| Logo | Comfortaa | Bold (700) | 20px | 1.4 | #1D1E1B |
| Body | Nunito | Regular (400) | 18px | 1.6 | #333333 |
| Body small | Nunito | Regular (400) | 16px | 1.5 | #333333 |
| Nav link | Nunito | Medium (500) | 16px | 1.4 | #333333 |
| Tab | Nunito | SemiBold (600) | 16px | 1.4 | #5C5964 |
| Button | Nunito | Bold (700) | 18px | 1.0 | #FFFFFF |
| Button small | Nunito | Bold (700) | 16px | 1.0 | #FFFFFF |
| Meta | Nunito | Regular (400) | 14px | 1.4 | #5C5964 |
| Caption | Nunito | Regular (400) | 14px | 1.4 | #5C5964 |
| Label | Nunito | SemiBold (600) | 12px | 1.3 | varies |
| Copyright | Nunito | Regular (400) | 12px | 1.4 | #5C5964 |

### Радиусы

| Элемент | Radius |
|---------|--------|
| Карточка | 20px |
| Hero-баннер | 32px |
| CTA-баннер | 24px |
| Поле ввода | 12px |
| Кнопка | 12px |
| Кнопка CTA hero | 16px |
| Таб | 8px |
| Метка категории | 4px |
| Тег | 6px |
| Пагинация | 8px |
| Иконка соцсети | 50% (круг) |
| Изображение в статье | 12px |
| Изображение alignfull | 16px |
| Блок автора | 20px |
| Blockquote | 0 16px 16px 0 |

### Тени

| Токен | Значение |
|-------|----------|
| card-default | 0 1px 3px rgba(0,0,0,0.04) |
| card-hover | 0 8px 24px rgba(0,0,0,0.1) |
| card-active | 0 4px 12px rgba(0,0,0,0.08) |
| header-scroll | 0 2px 8px rgba(0,0,0,0.06) |
| dropdown | 0 8px 24px rgba(0,0,0,0.1) |
| avatar | 0 4px 16px rgba(0,0,0,0.1) |
| social-icon | 0 2px 8px rgba(0,0,0,0.08) |
| btn-hover | 0 4px 12px rgba(233,88,90,0.3) |
| sticky-share | 0 2px 8px rgba(0,0,0,0.06) |

---

## Фрейм 1: Компоненты

> Страница в Figma: "Components"
> Разместить все компоненты на одном канвасе с отступами 100px между группами

---

### 1.1 Component: Header

**Фрейм:** 1440 x 112

**Иерархия слоёв:**
```
Header (Frame, 1440x112)
├── TopBar (Frame, 1440x64)
│   ├── Container (Frame, 1200x64, auto-layout horizontal, padding 0 24px, align center, justify space-between)
│   │   ├── Logo (Frame, auto-layout horizontal, gap 0)
│   │   │   ├── "NeoFamily" (Text) — Comfortaa Bold 20px #1D1E1B
│   │   │   └── ". Блог" (Text) — Comfortaa Regular 20px #5C5964
│   │   └── NavRight (Frame, auto-layout horizontal, gap 32px, align center)
│   │       ├── "Банк заданий" (Text) — Nunito Medium 16px #333333
│   │       ├── "Магазин" (Text) — Nunito Medium 16px #333333
│   │       ├── BtnLogin (Frame, auto-layout, padding 8px 20px, border-radius 12px, border 1.5px #E9585A)
│   │       │   └── "Войти" (Text) — Nunito SemiBold 16px #E9585A
│   │       └── IconSearch (Instance, 24x24, color #333333, touch-target 44x44)
│   └── Fill: #FFFFFF
├── CategoryBar (Frame, 1440x48)
│   ├── Container (Frame, auto-layout horizontal, gap 8px, align center, justify center)
│   │   ├── Tab "Актуальное" (Component)
│   │   ├── Tab "ЕГЭ и поступление" (Component)
│   │   ├── Tab "Биология" (Component)
│   │   ├── Tab "Химия" (Component)
│   │   └── Tab "Русский язык" (Component)
│   └── Fill: #F9F8FB
└── Shadow (Effect, visible on scroll state only): 0 2px 8px rgba(0,0,0,0.06)
```

**Элементы с точными размерами:**

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Header frame | 0 | 0 | 1440 | 112 | — |
| TopBar | 0 | 0 | 1440 | 64 | fill #FFFFFF |
| Container (top) | 120 | 0 | 1200 | 64 | auto-layout horizontal, padding 0 24px |
| Logo text | 144 | 20 | auto | 24 | Comfortaa Bold 20px #1D1E1B |
| NavRight | right-aligned | 16 | auto | 32 | gap 32px |
| BtnLogin | — | — | auto | 36 | border 1.5px #E9585A, radius 12px, padding 8px 20px |
| IconSearch | — | — | 24 | 24 | #333333, внутри touch-target 44x44 |
| CategoryBar | 0 | 64 | 1440 | 48 | fill #F9F8FB |
| Each Tab | — | — | auto | 32 | padding 8px 20px, radius 8px, gap 8px |

**Компонент Tab (вариантный):**

| Variant | Fill | Text color | Border |
|---------|------|------------|--------|
| Default | transparent | #5C5964 | none |
| Hover | rgba(cat-color, 0.1) | cat-color | none |
| Active | cat-color | #FFFFFF (#1D1E1B для жёлтых/зелёных) | none |
| Focus | transparent | cat-color | outline 2px solid cat-color, offset 2px |

---

### 1.2 Component: Footer

**Фрейм:** 1440 x 280 (приблизительно)

**Иерархия слоёв:**
```
Footer (Frame, 1440x~280)
├── MainSection (Frame, 1440x~220, fill #1D1E1B, padding 40px 0)
│   ├── Container (Frame, 1200x~140, auto-layout horizontal, gap auto, justify space-between)
│   │   ├── Col1_Logo (Frame, auto-layout vertical, gap 8px)
│   │   │   ├── "NeoFamily. Блог" (Text) — Comfortaa Bold 20px #FFFFFF
│   │   │   └── "Онлайн-школа подготовки к ЕГЭ\nна 80+ баллов" (Text) — Nunito 14px #A5A5A5
│   │   ├── Col2_Sections (Frame, auto-layout vertical, gap 12px)
│   │   │   ├── "Разделы блога" (Text) — Nunito SemiBold 16px #FFFFFF
│   │   │   ├── "Актуальное" (Text) — Nunito Regular 14px #A5A5A5
│   │   │   ├── "ЕГЭ и поступление" (Text)
│   │   │   ├── "Биология" (Text)
│   │   │   ├── "Химия" (Text)
│   │   │   └── "Русский язык" (Text)
│   │   ├── Col3_Company (Frame, auto-layout vertical, gap 12px)
│   │   │   ├── "Компания" (Text) — Nunito SemiBold 16px #FFFFFF
│   │   │   ├── "О нас" ... "Магазин" (Text links)
│   │   └── Col4_Social (Frame, auto-layout vertical, gap 12px)
│   │       ├── "Соцсети" (Text) — Nunito SemiBold 16px #FFFFFF
│   │       └── SocialIcons (Frame, auto-layout horizontal, gap 12px)
│   │           ├── VK (Circle 44x44, fill #333333, icon #FFFFFF)
│   │           ├── Telegram (Circle 44x44)
│   │           └── YouTube (Circle 44x44)
├── Divider (Line, 1200x1, stroke #333333)
└── BottomBar (Frame, 1440x~60, fill #1D1E1B, padding 20px 0)
    └── Container (Frame, 1200x~20, auto-layout horizontal, justify space-between)
        ├── "© 2026 NeoFamily. Все права защищены." (Text) — Nunito 12px #5C5964
        └── "Политика конфиденциальности" (Text) — Nunito 12px #5C5964
```

**Элементы:**

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Footer frame | 0 | 0 | 1440 | ~280 | fill #1D1E1B |
| Container | 120 | 40 | 1200 | auto | auto-layout horizontal |
| Col1 | 120 | 40 | 270 | auto | — |
| Col2 | 414 | 40 | 210 | auto | — |
| Col3 | 648 | 40 | 210 | auto | — |
| Col4 | 882 | 40 | 210 | auto | — |
| Social icon | — | — | 44 | 44 | radius 50%, fill #333333 |
| Divider | 120 | ~200 | 1200 | 1 | stroke #333333 |
| Copyright | 120 | ~220 | auto | auto | — |

**Hover states social icons:**
- VK hover: fill #0077FF
- Telegram hover: fill #26A5E4
- YouTube hover: fill #FF0000

---

### 1.3 Component: Card (карточка статьи)

**Фрейм:** 276 x ~420 (при 4-колоночной сетке в 1200px с gap 24px)

**Иерархия слоёв:**
```
Card (Frame, 276x~420, radius 20px, fill #FFFFFF, border 1px #EFEDF2, shadow card-default)
├── ImageContainer (Frame, 276x207, radius 20px 20px 0 0, clip content, overflow hidden)
│   └── Image (Rectangle, 276x207, fill image, object-fit cover)
├── Content (Frame, auto-layout vertical, padding 16px, gap 0)
│   ├── TopRow (Frame, auto-layout horizontal, justify space-between, align center)
│   │   ├── CategoryBadge (Frame, auto-layout, padding 4px 10px, radius 4px, fill rgba(cat-color, 0.15))
│   │   │   └── "БИОЛОГИЯ" (Text) — Nunito SemiBold 12px cat-color, uppercase, letter-spacing 0.5px
│   │   └── ReadTime (Frame, auto-layout horizontal, gap 4px, align center)
│   │       ├── ClockIcon (16x16, #5C5964)
│   │       └── "5 мин" (Text) — Nunito Regular 12px #5C5964
│   ├── Spacer (12px)
│   ├── Title (Text) — Nunito SemiBold 18px #1D1E1B, line-clamp 2, line-height 1.4
│   ├── Spacer (8px)
│   ├── Description (Text) — Nunito Regular 14px #5C5964, line-clamp 2, line-height 1.5
│   │   (mobile: 16px)
│   ├── Spacer (12px)
│   └── AuthorRow (Frame, auto-layout horizontal, gap 8px, align center)
│       ├── Avatar (Circle, 32x32, fill image, clip content)
│       ├── AuthorName (Text) — Nunito Medium 14px #333333
│       ├── Dot (Circle, 4x4, fill #DADADA)
│       └── Date (Text) — Nunito Regular 12px #989898
```

**Точные размеры:**

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Card frame | 0 | 0 | 276 | ~420 | radius 20, fill #FFF, border 1px #EFEDF2 |
| Image | 0 | 0 | 276 | 207 | radius 20 20 0 0, aspect-ratio 4:3 |
| Content padding | 16 | 207 | 244 | auto | padding 16px all |
| CategoryBadge | 16 | 223 | auto | 22 | padding 4px 10px, radius 4px |
| ReadTime | right-aligned | 223 | auto | 16 | — |
| Title | 16 | 249 | 244 | ~50 | max 2 lines |
| Description | 16 | 307 | 244 | ~42 | max 2 lines |
| Avatar | 16 | 361 | 32 | 32 | radius 50% |
| AuthorName | 56 | 365 | auto | 20 | — |
| Date | right area | 367 | auto | 16 | — |

**States (variants):**

| State | Shadow | Transform | Image scale |
|-------|--------|-----------|-------------|
| Default | 0 1px 3px rgba(0,0,0,0.04) | none | 1.0 |
| Hover | 0 8px 24px rgba(0,0,0,0.1) | translateY(-4px) | 1.03 |
| Focus | none | none | 1.0, outline 2px #E9585A offset 2px |
| Active | 0 4px 12px rgba(0,0,0,0.08) | translateY(-2px) | 1.0 |

---

### 1.4 Component: Breadcrumbs

**Фрейм:** 1200 x 20

**Иерархия слоёв:**
```
Breadcrumbs (Frame, 1200x20, auto-layout horizontal, gap 0, align center)
├── Link "Блог" (Text) — Nunito Regular 14px #5CA7D9
├── Separator ">" (Text) — Nunito Regular 14px #DADADA, padding 0 8px
├── Link "Биология" (Text) — Nunito Regular 14px #5CA7D9
├── Separator ">" (Text)
└── Current "Строение клетки" (Text) — Nunito Regular 14px #5C5964
```

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Frame | 0 | 0 | 1200 | 20 | auto-layout horizontal |
| Each link | auto | 0 | auto | 20 | Nunito 14px #5CA7D9 |
| Separator | auto | 0 | auto | 20 | Nunito 14px #DADADA, px 8px |
| Current item | auto | 0 | auto | 20 | Nunito 14px #5C5964, no link |

**States:**
- Link hover: underline, #5CA7D9
- Link focus: outline 2px solid #5CA7D9, radius 4px

---

### 1.5 Component: CTA-баннер

**Фрейм:** 720 x 180 (min-height)

**Иерархия слоёв:**
```
CTABanner (Frame, 720x180min, radius 24px, fill gradient 135deg #6A5C90 → #E9585A, padding 32px 40px)
├── Content (Frame, auto-layout horizontal, gap 24px, align center)
│   ├── Image (Rectangle, 160x120, radius 12px, fill image)
│   └── TextBlock (Frame, auto-layout vertical, gap 8px)
│       ├── Title (Text) — Comfortaa SemiBold 24px #FFFFFF
│       ├── Subtitle (Text) — Nunito Regular 16px rgba(255,255,255,0.85)
│       └── BtnCTA (Frame, auto-layout, padding 12px 28px, radius 12px, fill #FFFFFF)
│           └── "Записаться →" (Text) — Nunito Bold 16px #E9585A
```

**Variants фона:**
1. Gradient: 135deg #6A5C90 → #E9585A
2. Solid: cat-color + паттерн точек 5% opacity
3. Image: photo + overlay rgba(29,30,27,0.6)

---

### 1.6 Component: Пагинация

**Фрейм:** auto x 44

```
Pagination (Frame, auto x 44, auto-layout horizontal, gap 8px, justify center)
├── PrevArrow (Frame, 44x44, radius 8px, fill #FFF, border 1px #DADADA)
│   └── ArrowIcon (20x20, #333333)
├── Page "1" (Frame, 44x44, radius 8px, fill #E9585A) — active
│   └── "1" (Text) — Nunito SemiBold 16px #FFFFFF
├── Page "2" (Frame, 44x44, radius 8px, fill #FFF, border 1px #DADADA)
│   └── "2" (Text) — Nunito SemiBold 16px #333333
├── ...
├── Dots "..." (Text) — Nunito 16px #5C5964
├── Page "12" (Frame, 44x44, ...)
└── NextArrow (Frame, 44x44, ...)
```

---

### 1.7 Component: Рейтинг

**Фрейм:** auto x 48

```
Rating (Frame, auto-layout vertical, gap 16px, align center)
├── Label (Text) — Nunito SemiBold 18px #1D1E1B, "Была ли статья полезна?"
└── Buttons (Frame, auto-layout horizontal, gap 16px)
    ├── LikeBtn (Frame, 48x48, radius 12px, border 1.5px #DADADA)
    │   ├── ThumbUpIcon (24x24, #5C5964)
    │   └── Count "45" (Text) — Nunito 14px #5C5964
    └── DislikeBtn (Frame, 48x48, radius 12px, border 1.5px #DADADA)
        ├── ThumbDownIcon (24x24, #5C5964)
        └── Count "3" (Text) — Nunito 14px #5C5964
```

---

### 1.8 Component: Sticky Share (sidebar, desktop)

**Фрейм:** 44 x 200

```
StickyShare (Frame, 44x200, auto-layout vertical, gap 12px)
├── VK (Frame, 44x44, radius 50%, fill #FFFFFF, border 1px #EFEDF2, shadow sticky-share)
│   └── VKIcon (20x20, #5C5964)
├── Telegram (Frame, 44x44, ...)
├── WhatsApp (Frame, 44x44, ...)
└── Copy (Frame, 44x44, ...)
```

---

## Фрейм 2: Главная блога — Desktop

**Размер фрейма:** 1440 x 4200
**Fill:** #FFFFFF

### Иерархия слоёв (полная)

```
HomePage (Frame, 1440x4200, fill #FFFFFF)
├── Header (Instance, 0, 0, 1440x112)
├── HeroSection (Frame, 0, 112, 1440x~488)
│   ├── Container (1200, centered)
│   │   ├── H1 (Text, centered, max-w 700px)
│   │   └── HeroBanner (Frame, 1200x400, radius 32px)
├── CategorySection_1 "Актуальное" (Frame, 0, ~648, 1440x~384, fill #FFFFFF)
├── CategorySection_2 "ЕГЭ и поступление" (Frame, fill #F9F8FB)
├── CategorySection_3 "Биология" (Frame, fill #FFFFFF)
├── CategorySection_4 "Химия" (Frame, fill #F9F8FB)
├── CategorySection_5 "Русский язык" (Frame, fill #FFFFFF)
├── PromoBanner (Frame, 1440x~296)
├── FeedbackBlock (Frame, 1440x~400, fill #F9F8FB)
└── Footer (Instance, 1440x~280)
```

### Посекционная спецификация

#### Section: H1

| Элемент | x | y (от top фрейма) | w | h | Стиль |
|---------|---|---|---|---|-------|
| H1 text | center | 136 | 700 (max) | auto | Comfortaa Bold 36px #1D1E1B, text-align center |

#### Section: Hero Banner

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| HeroBanner container | 120 | 184 | 1200 | 400 | radius 32px, overflow hidden |
| Background image | 120 | 184 | 1200 | 400 | object-fit cover, WebP |
| Overlay gradient | 120 | 184 | 1200 | 400 | linear-gradient(to top, rgba(29,30,27,0.6) 0%, transparent 60%) |
| Content padding | 160 | 384 | auto | auto | padding 40px from bottom-left |
| Hero title | 160 | ~404 | 600 | auto | Comfortaa Bold 32px #FFFFFF |
| Hero subtitle | 160 | ~444 | 600 | auto | Nunito Regular 18px rgba(255,255,255,0.85) |
| Hero CTA button | 160 | ~478 | auto | 50 | fill #E9585A, radius 16px, padding 14px 32px, Nunito Bold 18px #FFF |

#### Section: Category block (repeating x5)

Каждая секция одинаковая по структуре, чередуется фон #FFFFFF / #F9F8FB.

| Элемент | x (от container) | y (внутри секции) | w | h | Стиль |
|---------|---|---|---|---|-------|
| Section frame | 0 | 0 | 1440 | ~384 | padding 48px 0 |
| Section title | 120 | 48 | auto | 32 | Comfortaa SemiBold 26px #1D1E1B |
| "Читать ещё →" | right-aligned to 1320 | 48 | auto | 24 | Nunito SemiBold 16px cat-color |
| Accent bar | 120 | 88 | 40 | 4 | fill cat-color, radius 2px |
| Card grid | 120 | 120 | 1200 | ~420 | CSS Grid 4 cols, gap 24px |
| Card 1 | 120 | 120 | 276 | ~420 | Instance of Card |
| Card 2 | 420 | 120 | 276 | ~420 | Instance of Card |
| Card 3 | 720 | 120 | 276 | ~420 | Instance of Card |
| Card 4 | 1020 | 120 | 276 | ~420 | Instance of Card |

**Auto Layout секции:**
- Direction: vertical
- Padding: 48px 120px (top/bottom 48, left/right 120 from 1440 to get 1200)
- Gap between title row and accent bar: 8px
- Gap between accent bar and cards: 24px

#### Section: Promo Banner

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Container | 120 | 0 | 1200 | 200 | radius 24px, gradient or image |
| Title | inside, 40px padding | — | auto | auto | Comfortaa SemiBold 28px #FFFFFF |
| Email field | — | — | 320 | 48 | radius 12px, fill #FFF |
| Subscribe button | — | — | auto | 48 | fill #E9585A, radius 12px |

#### Section: Feedback Block

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Section | 0 | 0 | 1440 | ~400 | fill #F9F8FB, padding 48px |
| Title | center | 48 | auto | auto | Comfortaa SemiBold 32px #1D1E1B |
| Subtitle | center | ~88 | auto | auto | Nunito Regular 18px #5C5964 |
| Form container | center | ~128 | 560 | auto | — |
| Input "Имя" | center | ~128 | 560 | 48 | radius 12px, border 1.5px #DADADA, fill #FFF |
| Input "Email" | center | ~192 | 560 | 48 | same |
| Textarea | center | ~256 | 560 | 120 | same |
| Button "Отправить" | center | ~400 | 560 | 52 | fill #E9585A, radius 12px, Nunito Bold 18px #FFF |

---

## Фрейм 3: Страница статьи — Desktop

**Размер фрейма:** 1440 x 5200
**Fill:** #FFFFFF

### Иерархия слоёв

```
ArticlePage (Frame, 1440x5200, fill #FFFFFF)
├── Header (Instance, 1440x112)
├── ProgressBar (Frame, 0, 112, 1440x3)
│   ├── Track (Rectangle, 1440x3, fill #EFEDF2)
│   └── Fill (Rectangle, ~500x3, fill #E9585A)
├── Breadcrumbs (Instance, 120, 131, 1200x20)
├── StickyShareLeft (Instance, ~40, 50%vh, 44x200) — fixed, left of content
├── ContentArea (Frame, 120, 167, 1200xauto, auto-layout horizontal, gap 48px)
│   ├── MainContent (Frame, 720xauto, auto-layout vertical)
│   │   ├── H1 (Text)
│   │   ├── MetaBlock (Frame)
│   │   ├── ExpertBadge (Frame)
│   │   ├── ArticleBody (Frame, auto-layout vertical)
│   │   │   ├── H2_1 (Text)
│   │   │   ├── Paragraph (Text)
│   │   │   ├── CTABanner_1 (Instance)
│   │   │   ├── H2_2 (Text)
│   │   │   ├── Paragraph (Text)
│   │   │   ├── ImageStandard (Frame)
│   │   │   ├── ImageAlignFull (Frame, 1200px wide, breaks out of 720)
│   │   │   ├── H2_3 (Text)
│   │   │   ├── Blockquote (Frame)
│   │   │   ├── CTABanner_2 (Instance)
│   │   │   ├── H2_4 (Text)
│   │   │   └── Paragraph (Text)
│   │   ├── RatingBlock (Instance)
│   │   ├── ShareButtons (Instance)
│   │   ├── Tags (Frame)
│   │   ├── AuthorBlock (Frame)
│   │   └── Sources (Frame)
│   └── Sidebar (Frame, 300xauto, position sticky top 139px)
│       ├── TOC (Frame)
│       ├── CTAWidget (Frame)
│       └── Popular (Frame)
├── RelatedSection (Frame, 120, ~4800, 1200xauto)
│   ├── H2 "Читай также" (Text)
│   └── CardGrid (3 cols, gap 24px)
│       ├── Card (Instance, 384x~420)
│       ├── Card (Instance)
│       └── Card (Instance)
└── Footer (Instance)
```

### Посекционная спецификация

#### Progress Bar

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Track | 0 | 112 | 1440 | 3 | fill #EFEDF2, sticky top 112px, z-index 100 |
| Fill | 0 | 112 | ~500 (35%) | 3 | fill #E9585A |

#### H1 + Meta

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| H1 | 120 | 167 | 720 | auto | Comfortaa Bold 36px #1D1E1B, lh 1.2 |
| MetaBlock | 120 | ~227 | 720 | 40 | auto-layout horizontal, gap 12px, align center |
| Avatar | 120 | ~227 | 40 | 40 | radius 50%, border 2px #EFEDF2 |
| Author name | 172 | ~235 | auto | 24 | Nunito SemiBold 16px #333333 |
| Separator | — | — | 1 | 16 | fill #DADADA |
| Date published | — | — | auto | 20 | Nunito 14px #5C5964, e.g. "10 мар 2026" |
| Date updated | — | — | auto | 20 | Nunito 14px #5C5964, "Обновлено: 15 мар 2026" |
| Separator | — | — | 1 | 16 | fill #DADADA |
| Read time | — | — | auto | 20 | Nunito 14px #5C5964, "7 мин чтения" |
| Separator | — | — | 1 | 16 | fill #DADADA |
| Category | — | — | auto | 20 | Nunito SemiBold 14px cat-color |
| ExpertBadge | 120 | ~279 | auto | 24 | fill rgba(161,210,54,0.1), radius 4px, padding 4px 12px |
| Badge icon | — | — | 16 | 16 | checkmark #A1D236 |
| Badge text | — | — | auto | 16 | Nunito SemiBold 12px #A1D236, "Проверено экспертом" |

#### Article Body Typography

| Элемент | w | Стиль |
|---------|---|-------|
| Paragraph | 720 | Nunito Regular 18px #333333, lh 1.6, mb 20px |
| H2 | 720 | Comfortaa SemiBold 32px #1D1E1B, mt 40px, mb 16px |
| H3 | 720 | Comfortaa SemiBold 26px #1D1E1B, mt 32px, mb 12px |
| UL/OL | 720 | pl 24px, Nunito 18px #333333, lh 1.6, gap 8px |
| Link | auto | #5CA7D9, underline, hover #E9585A |
| Blockquote | 720 | fill #F9F8FB, border-left 4px #E9585A, radius 0 16 16 0, padding 20px 24px |
| BQ text | — | Nunito Italic 20px #333333 |
| BQ source | — | Nunito 14px #5C5964, mt 8px |
| Image standard | 720 | radius 12px, margin 24px 0 |
| Image caption | 720 | Nunito 14px #5C5964, center, mt 8px |
| Image alignfull | 1200 | radius 16px, margin 32px 0, breaks out of 720 column |
| Table | 720 | radius 12px, border 1px #DADADA, overflow hidden |
| Table header | — | fill #F9F8FB, Nunito SemiBold 16px #1D1E1B, padding 12px 16px |
| Table cell | — | Nunito Regular 16px #333333, padding 12px 16px, border 1px #EFEDF2 |

#### CTA Banner (in article)

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Banner frame | 0 (in content col) | — | 720 | 180 min | radius 24px, gradient, padding 32px 40px, margin 32px 0 |
| Image | 0 | 0 | 160 | 120 | radius 12px |
| Title | 184 | 32 | auto | auto | Comfortaa SemiBold 24px #FFF |
| Subtitle | 184 | ~64 | auto | auto | Nunito Regular 16px rgba(255,255,255,0.85) |
| Button | 184 | ~96 | auto | 44 | fill #FFF, radius 12px, padding 12px 28px, Nunito Bold 16px #E9585A |

#### Rating Block

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Divider | 0 | 0 | 720 | 1 | fill #EFEDF2 |
| Container | 0 | 25 | 720 | auto | auto-layout vertical, gap 16px, align center |
| Label | center | — | auto | 24 | Nunito SemiBold 18px #1D1E1B |
| Like button | — | — | 48 | 48 | radius 12px, border 1.5px #DADADA |
| Like icon | — | — | 24 | 24 | #5C5964 |
| Like count | — | — | auto | 18 | Nunito 14px #5C5964 |
| Dislike button | — | — | 48 | 48 | same |

#### Share Buttons (bottom)

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Container | center | mt 24px | auto | 44 | auto-layout horizontal, gap 12px |
| Each button | — | — | 44 | 44 | radius 50%, fill #F9F8FB, icon 20px #5C5964 |

#### Sticky Share (left side)

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Container | calc(50% - 600px - 80px) | 50vh | 44 | ~200 | fixed, auto-layout vertical, gap 12px |
| Each button | 0 | — | 44 | 44 | radius 50%, fill #FFF, border 1px #EFEDF2, shadow 0 2px 8px rgba(0,0,0,0.06) |

#### Tags

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Container | 0 | mt 24px | 720 | auto | auto-layout horizontal, flex-wrap, gap 8px |
| Each tag | — | — | auto | 30 | fill #EFEDF2, radius 6px, padding 6px 12px, Nunito 14px #5C5964 |

#### Author Block

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Container | 0 | mt 32px | 720 | auto | fill #F9F8FB, radius 20px, padding 24px, auto-layout horizontal, gap 20px |
| Photo | 24 | 24 | 64 | 64 | radius 50% |
| Name | 108 | 24 | auto | 28 | Nunito SemiBold 20px #1D1E1B |
| Role | 108 | 52 | auto | 24 | Nunito Regular 16px #5C5964 |
| Link | 108 | 80 | auto | 20 | Nunito SemiBold 14px #E9585A, "Все статьи автора →" |

#### Sources

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Title | 0 | mt 32px | auto | 24 | Nunito SemiBold 18px #1D1E1B |
| List | 0 | mt 12px | 720 | auto | numbered, Nunito 14px #5C5964, links #5CA7D9 |

#### Sidebar (sticky)

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Sidebar frame | 768 (120+720+48-120) | 167 | 300 | auto | sticky top 139px, max-height calc(100vh - 139px), overflow-y auto |

**TOC в sidebar:**

| Элемент | x (внутри sidebar) | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Title "Содержание" | 0 | 0 | 300 | 20 | Nunito SemiBold 16px #1D1E1B |
| Item list | 0 | 28 | 300 | auto | padding-left 16px, border-left 2px #EFEDF2 |
| Each item | 16 | — | 284 | auto | Nunito Regular 14px #5C5964, gap 8px |
| Active item | 16 | — | 284 | auto | border-left 2px #E9585A, Nunito SemiBold 14px #E9585A |

**CTA Widget в sidebar:**

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Container | 0 | mt 32px | 300 | auto | gradient 180deg #6A5C90 → #E9585A, radius 20px, padding 24px |
| Title | 24 | 24 | 252 | auto | Nunito Bold 18px #FFFFFF |
| Text | 24 | ~52 | 252 | auto | Nunito Regular 14px rgba(255,255,255,0.85) |
| Button | 24 | ~88 | 252 | 40 | fill #FFF, radius 12px, Nunito Bold 14px #E9585A, width 100% |

**Popular в sidebar:**

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Title | 0 | mt 32px | 300 | 20 | Nunito SemiBold 16px #1D1E1B |
| Each item | 0 | mt 12px | 300 | auto | auto-layout horizontal, gap 12px |
| Number | 0 | — | 24 | 28 | Comfortaa Bold 20px cat-color |
| Article title | 36 | — | 264 | auto | Nunito Regular 14px #333333, hover #E9585A |

#### Related Section ("Читай также")

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Title | 120 | mt 48px | auto | 32 | Comfortaa SemiBold 26px #1D1E1B |
| Card grid | 120 | mt 24px | 1200 | ~420 | 3 cols, gap 24px |
| Card 1 | 120 | — | 384 | ~420 | Instance of Card |
| Card 2 | 528 | — | 384 | ~420 | Instance of Card |
| Card 3 | 936 | — | 384 | ~420 | Instance of Card |

---

## Фрейм 4: Страница категории — Desktop

**Размер фрейма:** 1440 x 3400
**Fill:** #FFFFFF

### Иерархия слоёв

```
CategoryPage (Frame, 1440x3400, fill #FFFFFF)
├── Header (Instance, 1440x112)
├── Breadcrumbs (Instance, 120, 128, 1200x20)
├── HeroSection (Frame, 120, 164, 1200xauto)
│   ├── H1 (Text)
│   ├── AccentBar (Rectangle)
│   ├── Description (Text)
│   └── Filters (Frame, auto-layout horizontal)
├── CardGrid (Frame, 120, ~364, 1200x~1752)
│   ├── Row1 (4 cards, gap 24px)
│   ├── Row2 (4 cards)
│   ├── Row3 (4 cards)
│   └── Row4 (4 cards)
├── Pagination (Instance, center, ~2148)
├── SeeAlso (Frame, 0, ~2228, 1440x~72, fill #F9F8FB)
├── FeedbackBlock (Instance, 0, ~2300, 1440x~400)
└── Footer (Instance, 0, ~2700, 1440x~280)
```

### Посекционная спецификация

#### Breadcrumbs

| Элемент | x | y | w | h |
|---------|---|---|---|---|
| Breadcrumbs | 120 | 128 | 1200 | 20 |

#### Hero Section

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| H1 | 120 | 164 | 1200 | auto | Comfortaa Bold 36px #1D1E1B, text-align left |
| AccentBar | 120 | ~208 | 60 | 4 | fill cat-color, radius 2px |
| Description | 120 | ~220 | 720 | auto | Nunito Regular 18px #5C5964 |
| FilterRow | 120 | ~260 | 1200 | 36 | auto-layout horizontal, gap 8px, overflow-x auto |
| Filter "Все" (active) | 120 | ~260 | auto | 36 | fill cat-color, Nunito Medium 14px #FFF, padding 8px 16px, radius 8px |
| Filter "Строение кл." | — | — | auto | 36 | border 1.5px #DADADA, Nunito Medium 14px #5C5964, padding 8px 16px, radius 8px |
| Filter hover | — | — | — | — | border cat-color, fill rgba(cat-color, 0.08) |

#### Card Grid (16 cards, 4x4)

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Grid container | 120 | ~328 | 1200 | auto | CSS Grid 4 cols, gap 24px horizontal + 24px vertical |
| Row 1 cards | 120, 420, 720, 1020 | ~328 | 276 | ~420 | Instance of Card |
| Row 2 cards | same x | ~772 | 276 | ~420 | — |
| Row 3 cards | same x | ~1216 | 276 | ~420 | — |
| Row 4 cards | same x | ~1660 | 276 | ~420 | — |

#### Pagination

| Элемент | x | y | w | h |
|---------|---|---|---|---|
| Pagination | center | ~2112 | auto | 44 |

#### See Also

| Элемент | x | y | w | h | Стиль |
|---------|---|---|---|---|-------|
| Section | 0 | ~2188 | 1440 | 72 | fill #F9F8FB, padding 24px |
| Label "Смотрите также:" | 120 | — | auto | 24 | Nunito SemiBold 18px #1D1E1B |
| Link "ЕГЭ и поступление" | after label | — | auto | 24 | Nunito Medium 16px cat-color |
| Dot separator | — | — | 4 | 4 | fill #DADADA, radius 50% |
| Link "Химия" | — | — | auto | 24 | Nunito Medium 16px cat-color |

#### Feedback Block

Same as on homepage (see Фрейм 2).

---

## Общие указания для Figma

### Организация страниц

1. **Page "Components"** — все компоненты (Header, Footer, Card, Breadcrumbs, CTA, Pagination, Rating, Share, StickyShare, Tags, AuthorBlock, Inputs, Buttons)
2. **Page "Desktop"** — фреймы страниц (Главная, Статья, Категория)
3. **Page "Tokens"** — цветовые стили, типографические стили, эффекты

### Auto Layout рекомендации

- Все компоненты строить на Auto Layout
- Container (1200px) внутри полноширинных секций (1440px): horizontal padding 120px
- Карточные сетки: использовать Auto Layout с wrap для адаптивности
- Sidebar layout: horizontal auto-layout с fixed width 300px для sidebar

### Naming convention

- Frames: PascalCase (e.g., `HeroBanner`, `CategorySection`, `CardGrid`)
- Components: PascalCase с префиксом (e.g., `Card/Default`, `Tab/Active`, `Button/Primary/Default`)
- Text styles: slash notation (e.g., `H1`, `Body`, `Meta/Regular`, `Label/SemiBold`)
- Color styles: slash notation (e.g., `Primary/Default`, `Text/Body`, `Category/Bio`)

### Variants для компонентов

| Компонент | Свойства вариантов |
|-----------|-------------------|
| Button | Type (Primary, Secondary, Ghost), State (Default, Hover, Active, Focus, Disabled, Loading) |
| Tab | Category (Actual, EGE, Bio, Chem, Rus), State (Default, Hover, Active, Focus) |
| Card | State (Default, Hover, Focus, Active) |
| Input | State (Default, Focus, Error, Filled, Disabled) |
| Pagination Item | State (Default, Active, Hover, Disabled) |
| Rating Button | Type (Like, Dislike), State (Default, Hover, Active/Voted) |
| Share Button | Network (VK, Telegram, WhatsApp, Copy), State (Default, Hover) |
| Social Icon (footer) | Network (VK, Telegram, YouTube), State (Default, Hover) |
