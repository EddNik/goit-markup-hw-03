# 📌 Модуль 3.1: Блокова модель

## 🔹 1. План заняття

- Блокова модель елемента
- Властивості `width` та `height`
- Модель візуального форматування: `box-sizing`
- Геометрія елемента
- Рамки та заокруглені рамки
- "Схлопування" і випадіння вертикальних маржинів
- Горизонтальне центрування блокових елементів
- Типи боксів: блокові, рядкові та рядково-блокові елементи. Властивість `display`

---

## 🔹 2. Box-model

### Основні компоненти блокової моделі:

- **content** — вміст елемента
- **padding** — відступи всередині елемента
- **border** — межа елемента
- **margin** — відступи зовні елемента

### Властивості для управління розмірами та відступами:

- **top, right, bottom, left** — для позиціювання елемента
- **width, height** — ширина та висота елемента (з максимальними та мінімальними значеннями)
- **box-sizing: content-box | border-box | inherit** — управління розмірами елемента з урахуванням
  рамок і відступів

### Стилізація рамок:

- **border**: solid, dotted, dashed, double — типи рамок
- **border-radius** - заокруглення кутів рамки

### Оформлення переповнення:

- **overflow**: visible | hidden | scroll | auto

| Значення  | Опис                                                                      |
| --------- | ------------------------------------------------------------------------- |
| `visible` | 🔹 **За замовчуванням.** Вміст виходить за межі контейнера і **видимий**. |
| `hidden`  | 🔒 Вміст, що виходить за межі, **обрізається** і **не видно**.            |
| `scroll`  | 📜 Завжди додає **прокрутку**, навіть якщо вона **не потрібна**.          |
| `auto`    | ⚙️ Додає **прокрутку лише при потребі**, якщо вміст **не вміщується**.    |

### Типи елементів:

- **display**: block, inline, inline-block, none — управління відображенням елементів

### Центрування елементів на сторінці:

- **margin**: margin: 0 auto; || margin-right: auto; margin-left: auto;

### Налаштування "Гумові картинки":

- display: block;
- max-width: 100%;
- height: auto;

#### Альтернативний спосіб:

- display: block;
- max-width: 100%;
- height: 100%;
- object-fit: cover;

### Приховування заголовків (visually-hidden):

- position: absolute;
- white-space: nowrap;
- width: 1px;
- height: 1px;
- overflow: hidden;
- border: 0;
- padding: 0;
- clip: rect(0 0 0 0);
- clip-path: inset(50%);
- margin: -1px;

---

## 🔹 3. Flexbox

### Властивість display:

- **display:** — flex | inline-flex

### Властивості flex контейнера:

- **gap:** — відступ між flex елементами
- **flex-direction:** — row | row-reverse | column | column-reverse
- **justify-content:** — flex-start | flex-end | center | space-between | space-around |
  space-evenly
- **align-items:** — stretch | flex-start | flex-end | center | baseline
- **flex-wrap:** — nowrap | wrap | wrap-reverse
- **align-content:** — flex-start | flex-end | center | space-between | space-around | space-evenly
  | stretch

- **CSS-функція calc():** — calc((100% - 20px \* 2) / 3);

### Властивості flex елементів:

- **flex-basis:** — auto | значення
- **flex-grow:** — значення
- **flex-shrink:** — значення
- **align-self:** — auto | flex-start | flex-end | center | baseline | stretch
- **order:** — позиція

## 🔹 3. Структурні псевдокласи

**Стани елементів** (інтерактивні):

- **:hover** — коли курсор на елементі
- **:focus** — коли елемент у фокусі (наприклад, інпут)
- **:active** — під час кліку
- **:visited** — для відвіданих посилань

**Положення в DOM**:

- **:first-child** — перший елемент у батьківському
- **:last-child** — останній
- **:nth-child(n)** — n-ий за рахунком (number | odd | even)

** Фільтрація**:

- **:not(selector)** — все, крім вказаного
- **:empty** — елемент без дітей
- **:is()** — групування селекторів (новіший синтаксис)

### Оформлення переповнення:

- **overflow**: visible | hidden | scroll | auto

| Значення  | Опис                                                                      |
| --------- | ------------------------------------------------------------------------- |
| `visible` | 🔹 **За замовчуванням.** Вміст виходить за межі контейнера і **видимий**. |
| `hidden`  | 🔒 Вміст, що виходить за межі, **обрізається** і **не видно**.            |
| `scroll`  | 📜 Завжди додає **прокрутку**, навіть якщо вона **не потрібна**.          |
| `auto`    | ⚙️ Додає **прокрутку лише при потребі**, якщо вміст **не вміщується**.    |

### Типи елементів:

- **display**: block, inline, inline-block, none — управління відображенням елементів

### Налаштування "Гумові картинки":

- display: block;
- max-width: 100%;
- height: auto;

#### Альтернативний спосіб:

- display: block;
- max-width: 100%;
- height: 100%;
- object-fit: cover;

## 🧷 Додаткові ресурси 📚

- Особливості inline-block елементів -
  https://css-tricks.com/fighting-the-space-between-inline-block-elements/
- Повний посібник з Flexbox - https://css-tricks.com/snippets/css/a-guide-to-flexbox/
- Гра по Flexbox - http://flexboxfroggy.com/
- Ще одна гра на вивчення флексів https://mastery.games/flexboxzombies/
- Специфікація - https://developer.mozilla.org/en-US/docs/Web/CSS
- Слова, які часто використовуються в CSS-класах - https://github.com/YK911/basic-dictionary
- Плагін, який аналізує відразу всі шрифти макета https://www.youtube.com/watch?v=6nKQsgiNIFc
- Шукати плагін можна як у відео чи простіше: Головне меню Figma -> Plugins -> Manage plugins ->
  Font Fascia
- Посилання на довідник по HTML і CSS https://css.in.ua/
- https://cdnjs.com/libraries/modern-normalize

- 🖼 [Remove.bg](https://www.remove.bg/) – сервіс для видалення фону із зображень
- 🛠 [iLoveIMG](https://www.iloveimg.com/) – інструменти для обробки зображень
- ✅ [W3C Validator](https://validator.w3.org/) – перевірка HTML-коду на
  помилки -[CSS Validator](https://jigsaw.w3.org/css-validator/) - CSS validator
- 📖 [MDN HTML Docs](https://developer.mozilla.org/en-US/docs/Web/HTML) – офіційна документація HTML

- 🖼 [toptal.com](https://www.toptal.com/designers/htmlarrows/symbols/) – спеціальні символи
- 🛠 [Caninclude](https://caninclude.glitch.me/) – чи можу вкласти тег в інший тег
- 📖 [Emmet commands](https://docs.emmet.io/cheat-sheet/) – швидкі команди emmet
- 📖 [MDN HTML Docs](https://developer.mozilla.org/en-US/docs/Web/HTML) – офіційна документація

- 🛠 [Squoosh](https://squoosh.app/) – Оптимізація картинок (jpeg)
- 🛠 [Tiny PNG](https://tinypng.com/) – Оптимізація картинок (png)

- 📖
  [Figma Template](https://www.figma.com/design/LWMTodUscRGMcbTpxE3kgI/Simply-Chocolate?node-id=1-5060&t=FZ9D8VYSe7z6EkSG-0)
  – Figma

- [HTML reference](https://htmlreference.io/) - безкоштовний інтерактивний довідник з HTML від
  творців
