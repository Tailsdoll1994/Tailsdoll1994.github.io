Почти всё было написано с помощью GitHub Copilot и локальной [LLM](https://huggingface.co/Jackrong/Qwopus-GLM-18B-Merged-GGUF) [Q4_K_M 9.84GB + Ollama] — это эксперимент по быстрому созданию одностраничного сайта с минимальным количеством графики.

> Переключение языка в этом файле реализовано через якоря: выберите нужную версию ниже.
>
> [Русский](#русский) · [English](#english)

## Русский

## О проекте

Это одностраничное портфолио/резюме в стиле digital CV. Проект показывает:
- профиль с фото и базовой информацией;
- опыт работы и ключевые достижения;
- список навыков и специализаций;
- ссылки на соцсети и работы в ArtStation;
- интерфейс с поддержкой переключения языка.

## Что именно есть на странице

Сайт состоит из нескольких блоков:

1. **Шапка с действиями** — кнопка скачивания резюме и переключатель языка.
2. **Фоновое изображение** — декоративный фон с мягким градиентным эффектом.
3. **Аватар** — фото профиля.
4. **Раздел "Обо мне"** — короткое описание профессионального направления.
5. **Раздел "Опыт"** — история работы, обязанности и стек технологий.
6. **Раздел "Навыки"** — специализации, инструменты и технологии.
7. **Раздел "Работы на ArtStation"** — карточки с выбранными проектами.
8. **Раздел "Ссылки"** — быстрые переходы к профилям в соцсетях.

## Переключение языка

В интерфейсе есть кнопка `EN / RU`, которая меняет текст на странице между английским и русским вариантами. Поддерживаются:
- заголовки разделов;
- описание профиля;
- текст по опыту и навыкам;
- надписи кнопок и сообщений модального окна.

Также реализован выбор языка резюме: при клике по кнопке скачивания открывается окно, где можно выбрать английскую или русскую версию документа.

## Как это устроено

### Технологический стек

- **HTML5** — семантическая разметка страницы;
- **CSS3** — стили, анимации, сетка, адаптивность;
- **JavaScript** — логика переключения языка, загрузка работ и интерактивные элементы;
- **particles.js** — анимированный фон;
- **ArtStation API / RSS** — загрузка работ в блок портфолио.

### Структура проекта

```text
/
├── index.html          # основная разметка страницы
├── styles.css          # стили и визуальные эффекты
└── src/
    ├── avatar/         # изображения профиля
    ├── background/     # фоновые картинки
    ├── files/          # PDF/резюме
    ├── icons/          # SVG/PNG-иконки
    └── spec/           # вспомогательные документы и заметки
```

## Ключевые особенности

1. **Двуязычный интерфейс** — поддержка русского и английского текста через data-атрибуты.
2. **Минимум зависимостей** — основной контент хранится в одном HTML-файле, а внешние библиотеки подключаются по CDN.
3. **Семантическая разметка** — структура страницы подходит для чтения как человеком, так и браузером.
4. **Модульный стиль** — CSS-разметка разделена на логические блоки и легко меняется.
5. **Интерактивные элементы** — анимация фона, переключатель языка и модальное окно для резюме.

## Как редактировать контент

Для обновления текста или структуры:

1. Измените HTML в [index.html](index.html).
2. При необходимости поправьте стили в [styles.css](styles.css).
3. Добавьте нужные картинки или файлы в папку [src](src).
4. Если нужно добавить новые переводы — используйте атрибуты `data-en` и `data-ru`.

---

## English

## Project Overview

This is a single-page portfolio/CV in a digital resume style. The project showcases:
- a profile section with a photo and basic information;
- work experience and key achievements;
- a list of skills and specializations;
- links to social profiles and ArtStation work;
- an interface with language switching support.

## What is on the page

The site consists of several sections:

1. **Top actions bar** — resume download button and language switcher.
2. **Background image** — decorative background with a soft gradient effect.
3. **Avatar** — profile photo.
4. **About me section** — a short description of the professional focus.
5. **Experience section** — work history, responsibilities, and technology stack.
6. **Skills section** — specializations, tools, and technologies.
7. **ArtStation works section** — cards with selected projects.
8. **Links section** — quick access to social profiles.

## Language switching

The interface includes a `EN / RU` button that changes the page text between English and Russian. Supported content includes:
- section headings;
- profile descriptions;
- experience and skills text;
- button labels and modal messages.

There is also a resume language selector: clicking the download button opens a modal where you can choose either the English or Russian version.

## How it works

### Technology stack

- **HTML5** — semantic page structure;
- **CSS3** — styles, animations, layout, and responsiveness;
- **JavaScript** — language switching logic, work loading, and interactive behavior;
- **particles.js** — animated background;
- **ArtStation API / RSS** — loading portfolio works.

### Project structure

```text
/
├── index.html          # main page markup
├── styles.css          # styles and visual effects
└── src/
    ├── avatar/         # profile images
    ├── background/     # background images
    ├── files/          # PDF/resume files
    ├── icons/          # SVG/PNG icons
    └── spec/           # notes and supporting docs
```

## Key features

1. **Bilingual interface** — support for Russian and English text through data attributes.
2. **Minimal dependencies** — the main content is stored in a single HTML file, while external libraries are loaded via CDN.
3. **Semantic markup** — the structure is readable for both humans and browsers.
4. **Modular styling** — CSS is organized into logical blocks and is easy to adjust.
5. **Interactive elements** — animated background, language switcher, and resume modal.

## How to update content

To update text or structure:

1. Edit the HTML in [index.html](index.html).
2. Adjust styles in [styles.css](styles.css) if needed.
3. Add images or files to [src](src).
4. If new translations are needed, use the `data-en` and `data-ru` attributes.

---
