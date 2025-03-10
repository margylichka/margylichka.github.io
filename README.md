# margylichka.github.io
Визитка для QA
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link href="./normalize.css" rel="stylesheet" />
    <link href="./ios.css" rel="stylesheet" />
    <title>Document</title>
  </head>
  <body>
    <header class="header">
      <img src="./avatar.png.png" alt="avatar" class="header__avatar" />
      <div class="header__textContainer">
        <h1 class="header__title">Маргарита Рудкевич</h1>
        <h3 class="header__subtitle">QA Engineer</h3>
      </div>
    </header>
    <main>
      <section class="links">
        <h2 class="links__header">Для связи со мной</h2>
        <ul class="links__container">
          <li class="links__link">
            <p class="links__title">Телеграм</p>
            <a class="linsk__link" href="https://t.me/mrs_margarita">@mrs_margarita</a>
          </li>
          <li class="links__link">
            <p class="links__title">Эл. почта</p>
            <a class="linsk__link" href="https://mail.yandex.ru/?uid=2072145673#tabs/relevant?current_folder=1"
              >margylichka@yandex.ru</a
            >
          </li>
        </ul>
      </section>
      <section class="links">
        <h2 class="links__header">Какие инструменты использую для тестирования</h2>
        <ul class="links__container">
          <li class="links__link">
            <p class="links__title">Клиент</p>
            <a class="linsk__title" >DevTools</a>
          </li>
          <li class="links__link">
            <p class="links__title">Бекэнд</p>
            <a class="linsk__title">Postman</a>
          </li>
          <li class="links__link">
            <p class="links__title">Мобилки</p>
            <a class="linsk__title">Charles</a>
          </li>
          <li class="links__link">
            <p class="links__title">Чек-листы</p>
            <a class="linsk__title">Miro</a>
          </li>
          <li class="links__link">
            <p class="links__title">Тест-кейсы</p>
            <a class="linsk__title">Yandex Tracker</a>
          </li>
        </ul>
      </section>
    </main>
   <footer>
      <button type = "button" class="button-link" href=""> В чем сила, брат?  </button>
    </footer>
    <script type="text/javascript" src="js.js"></script>
  </body>
</html>
body {
  font-family: "Helvetica";
  background-color: #f2f1f6;
  color: #000000;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.header {
  box-sizing: border-box;
  margin: 40px 0 20px 0;
  display: flex;

  width: 320px;
  column-gap: 20px;
  row-gap: 10px;
  border-radius: 20px;
  padding: 20px;
  background-color: #ffffff;
}

.header__textContainer {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.header__avatar {
  border-radius: 50%;
  width: 80px;
  height: 80px;
}

.header__title {
  margin: 0;
  font-weight: 700;
  font-size: 22px;
  line-height: 1.2;
  font-family: "Helvetica Neue";
  align-items: center;
}

.header__subtitle {
  color: #7d7d7f;
  font-weight: 400;
  font-size: 14px;
  line-height: 1.4;
  margin: 0;
}

.links {
  width: 320px;
  margin-bottom: 20px;
}

.links__header {
  font-size: 23px;
  line-height: 1.4;
  margin: 0 0 15px 0;
  font-family: "Helvetica Neue";
  align-items: center
}

.links__container {
  list-style-type: none;
  background: #ffffff;
  border-radius: 20px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 20px 20px 10px;
  gap: 10px;
  flex: none;
  order: 1;
  flex-grow: 0;
  box-sizing: border-box;
  margin: 0;
}

.links__link,
.links__title {
  font-size: 15px;
  font-size: 1.4;
}

.links__link {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  padding: 0px 0px 10px;
  gap: 30px;
  border-bottom: 1px solid #dedede;
  width: 280px;
}

.links__link:last-child {
  border-bottom: none;
}

.linsk__link,
.links__link:visited {
  text-decoration: none;
  color: #0c79ff;
}

.links__title {
  margin: 0;
  min-width: 100px;
}

footer {
  margin: 0 0 40px 0;
}
.button-link {
  margin-top: 10px;
  box-sizing: border-box;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 50px;
  width: 320px;
  background: #ffffff;
  border-radius: 10px;

  font-size: 14px;
  line-height: 1.4;

  color: #0c79ff;
  text-decoration: none;
}

button {
  border: justify-content: center;
  align-items: center;;
}
/* Это объявление переменной, мы наши кнопку по тегу */
const button = document.querySelector('button');

/* Тут на кнопку навешиваем обрабочик, который ждёт клика и тогда запустит логику */
button.addEventListener('click', function() {
	alert('Сайт без багов')
})
/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */

/* Документ
   ========================================================================== */

/**
 * 1. Исправьте высоту строки во всех браузерах.
 * 2. Запретить изменение размера шрифта после изменения ориентации в iOS.
 */

html {
  line-height: 1.15; /* 1 */
  -webkit-text-size-adjust: 100%; /* 2 */
}

/* Разделы
   ========================================================================== */

/**
 * Уберите поля во всех браузерах.
 */

body {
  margin: 0;
}

/**
 * Последовательно визуализируйте `основной` элемент в IE.
 */

main {
  display: block;
}

/**
 * Исправьте размер шрифта и поля для элементов `h1` в контекстах `section` и
 * `article` в Chrome, Firefox, and Safari.
 */

h1 {
  font-size: 2em;
  margin: 0.67em 0;
}

/* Группировка содержимого
   ========================================================================== */

/**
 * 1. Добавьте правильный 'box sizing' в Firefox.
 * 2. Покажите переполнение в Edge и IE.
 */

hr {
  box-sizing: content-box; /* 1 */
  height: 0; /* 1 */
  overflow: visible; /* 2 */
}

/**
 * 1. Исправьте наследование и масштабирование размера шрифта во всех браузерах.
 * 2. Исправьте нечетный размер шрифта "em" во всех браузерах.
 */

pre {
  font-family: monospace, monospace; /* 1 */
  font-size: 1em; /* 2 */
}

/* Семантика на уровне текста
   ========================================================================== */

/**
 * Удалите серый фон для активных ссылок в IE 10.
 */

a {
  background-color: transparent;
}

/**
 * 1. Удалите нижнюю границу в Chrome 57-
 * 2. Добавьте правильное оформление текста в Chrome, Edge, IE, Opera и Safari.
 */

abbr[title] {
  border-bottom: none; /* 1 */
  text-decoration: underline; /* 2 */
  text-decoration: underline dotted; /* 2 */
}

/**
 * Добавьте правильный 'font weight' в Chrome, Edge и Safari.
 */

b,
strong {
  font-weight: bolder;
}

/**
 * 1. Исправьте наследование и масштабирование размера шрифта во всех браузерах.
 * 2. Исправьте нечетный размер шрифта "em" во всех браузерах.
 */

code,
kbd,
samp {
  font-family: monospace, monospace; /* 1 */
  font-size: 1em; /* 2 */
}

/**
 * Добавьте правильный размер шрифта во всех браузерах.
 */

small {
  font-size: 80%;
}

/**
 * Не допускайте, чтобы элементы `sub` и `sup` влияли на высоту строки во
 * всех браузерах.
 */

sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}

sub {
  bottom: -0.25em;
}

sup {
  top: -0.5em;
}

/* Встроенное содержимое
   ========================================================================== */

/**
 * Удалите границы на изображениях внутри ссылок в IE 10.
 */

img {
  border-style: none;
}

/* Формы
   ========================================================================== */

/**
 * 1. Измените стили шрифтов во всех браузерах.
 * 2. Удалите поля в Firefox и Safari.
 */

button,
input,
optgroup,
select,
textarea {
  font-family: inherit; /* 1 */
  font-size: 100%; /* 1 */
  line-height: 1.15; /* 1 */
  margin: 0; /* 2 */
}

/**
 * Показать переполнение в IE.
 * 1. Показать переполнение в Edge.
 */

button,
input { /* 1 */
  overflow: visible;
}

/**
 * Удалите наследование 'text transform' в Edge, Firefox и IE.
 * 1. Удалите наследование 'text transform' в Firefox.
 */

button,
select { /* 1 */
  text-transform: none;
}

/**
 * Исправьте невозможность стилизовать кликабельные типы в iOS и Safari.
 */

button,
[type="button"],
[type="reset"],
[type="submit"] {
  -webkit-appearance: button;
}

/**
 * Удалите внутреннюю границу и отступы в Firefox.
 */

button::-moz-focus-inner,
[type="button"]::-moz-focus-inner,
[type="reset"]::-moz-focus-inner,
[type="submit"]::-moz-focus-inner {
  border-style: none;
  padding: 0;
}

/**
 * Восстановите стиль фокусировки, установленный предыдущим правилом.
 */

button:-moz-focusring,
[type="button"]:-moz-focusring,
[type="reset"]:-moz-focusring,
[type="submit"]:-moz-focusring {
  outline: 1px dotted ButtonText;
}

/**
 * Исправьте отступы в Firefox.
 */

fieldset {
  padding: 0.35em 0.75em 0.625em;
}

/**
 * 1. Исправьте перенос текста в Edge и IE.
 * 2. Исправьте наследование цвета от элементов `fieldset` в IE.
 * 3. Удалите отступы, чтобы разработчики не были застигнуты врасплох, когда они обнулятся
 *    * элементы `fieldset` во всех браузерах.
 */

legend {
  box-sizing: border-box; /* 1 */
  color: inherit; /* 2 */
  display: table; /* 1 */
  max-width: 100%; /* 1 */
  padding: 0; /* 3 */
  white-space: normal; /* 1 */
}

/**
 * Добавьте правильное выравнивание по вертикали в Chrome, Firefox и Opera.
 */

progress {
  vertical-align: baseline;
}

/**
 * Удалите вертикальную полосу прокрутки по умолчанию в IE 10+.
 */

textarea {
  overflow: auto;
}

/**
 * 1. Добавьте правильный размер поля в IE 10.
 * 2. Удалите отступы в IE 10.
 */

[type="checkbox"],
[type="radio"] {
  box-sizing: border-box; /* 1 */
  padding: 0; /* 2 */
}

/**
 * Исправьте стиль курсора кнопок увеличения и уменьшения в Chrome.
 */

[type="number"]::-webkit-inner-spin-button,
[type="number"]::-webkit-outer-spin-button {
  height: auto;
}

/**
 * 1. Исправьте странный внешний вид в Chrome и Safari.
 * 2. Исправьте стиль контура в Safari.
 */

[type="search"] {
  -webkit-appearance: textfield; /* 1 */
  outline-offset: -2px; /* 2 */
}

/**
 * Удалите внутреннюю прокладку в Chrome и Safari на mac OS.
 */

[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}

/**
 * 1. Исправьте невозможность стилизовать кликабельные типы в iOS и Safari.
 * 2. Измените свойства шрифта на `наследование` в Safari.
 */

::-webkit-file-upload-button {
  -webkit-appearance: button; /* 1 */
  font: inherit; /* 2 */
}

/* Интерактивность
   ========================================================================== */

/*
 * Добавьте правильное отображение в Edge, IE 10+ и Firefox.
 */

details {
  display: block;
}

/*
 * Добавьте правильное отображение во всех браузерах.
 */

summary {
  display: list-item;
}

/* Разное
   ========================================================================== */

/**
 * Добавьте правильное отображение в IE 10+.
 */

template {
  display: none;
}

/**
 * Добавьте правильное отображение в IE 10.
 */

[hidden] {
  display: none;
}
![avatar png](https://github.com/user-attachments/assets/c14e4e70-67e9-4530-b1e6-1cc197253b21)
