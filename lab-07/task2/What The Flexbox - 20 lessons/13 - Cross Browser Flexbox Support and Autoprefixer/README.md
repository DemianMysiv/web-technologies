# Скриншоти №72–80: Autoprefixer + Gulp

**№72.** Онлайн-інструмент Autoprefixer: ліворуч CSS без префіксів, праворуч з `-webkit-` і `-ms-` для старих браузерів. У лівому полі випадково присутня некоректна незавершена декларація `align-content:;` — вона збережена тільки в `examples/online-autoprefixer-input-as-shown.css`. У робочому `css/styles.css` вона замінена на `align-content: center;` як приклад.

**№73–74.** У терміналі показано Node.js `v0.12.2` та команду `npm install gulp -g`; це старі кадри та історичні версії, а не порада для поточного програмування.

**№75.** Перший `gulpfile.js` містить потік `gulp.src('css/styles.css').pipe(autoprefixer()).pipe(gulp.dest('build'))`.

**№76.** `package.json` після `npm init` із полями `name`, `version`, `main`, `scripts`, `author`, `license`.

**№77–78.** Приклад `index.html` з `<link rel="stylesheet" href="build/styles.css">`.

**№79.** Структура: `css/styles.css` як вхід, `build/styles.css` як вихід, `gulpfile.js`, `index.html`, `package.json`, `node_modules`.

**№80.** Початок додавання Gulp-task. Вищенаведений `gulpfile.js` містить повну задачу `styles`; `watch` відтворено за кадром із наступної видимої частини курсу, **не №80**, тому розглядайте цей фрагмент як додатковий навчальний контекст, а не як буквальну реконструкцію цього кадру.

`build/styles.css` — відтворення видимого прикладу результату, а не файл, згенерований тут командою Gulp. Оригінальний Gulp-код демонструє старий інтерфейс `gulp.watch(path, ['styles'])`; у новіших Gulp це слід адаптувати, як і спосіб імпорту сучасного `gulp-autoprefixer`. Залежності не встановлювалися і автоматичний build не запускався.

**№81–84:** доведено `gulpfile.js` до прикладу з `gulp.task('watch', ...)`, повторно показано вхідний CSS поруч із CSS з префіксами, і HTML, що підключає `build/styles.css`. Раніше реконструйований `gulpfile.js` уже містив `watch`; ці скріншоти підтверджують цей фрагмент, тому дублікати файлів не додаються.

Оригінальні `css/styles.css`, `build/styles.css`, `gulpfile.js` та `package.json` збережені; `index.html` та `style.css` додатково оформлено як видимий навчальний приклад.
