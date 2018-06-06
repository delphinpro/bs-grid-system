# bs-grid-system
Модифицированная bootstrap-сетка.

##Установка
```cmd
bower i -S bs-grid-system

npm i -S bs-grid-system
```

##Подключение
Импортируйте файлы пакета и вызовите миксин `make-grid-system()` для генерации стилей сетки.
Для изменения настроек скопируйте в вашу source директорию файл `_grid.cfg.scss`, подключите его перед файлами пакета
и задайте нужные опции.
```cmd
@import ./my-custom-settings.scss

@import ./bower_components/bs-grid-system/source/scss/bs-grid.scss
// or
@import ./node_modules/bs-grid-system/source/scss/bs-grid.scss

@include make-grid-system();
```

##Опции
| Опция           | Описание
| ---:|:---
| `$grid-breakpoint`        | Список точек переключения. По умолчанию задано пять точек, вы можете задать ихх сколько угодно.
| `$container-max-widths`   | Список ширин контейнера для каждой точки переключения, кроме минимальной (ноль)
| `$grid-columns`           | Количество колонок в сетке
| `$grid-gutter-width-base` | Базовая ширина промежутка между колонками. Не рекомендуется к использованию. См. опцию `$grid-gutter-widths`
| `$grid-gutter-widths`     | Ширины промежутков между колонками для каждой точки переключения
| `$grid-use-rem`           | Включает генерацию сетки с точками переключения, выраженными в единицах `rem`. Для работы необходим пакет vRhythm
| `$grid-use-flex`          | Включает генерацию сетки с использованием flex-раскладки
| `$grid-add-box-sizing`    | Добавляет правило `box-sizing: border-box` для колонок. Вы можете отключить эту опцию, если у вас, например, задано глобальное правило `*{box-sizing:border-box}`

| Опция                         | По умолчанию        | Описание
| ---:|:---:|:---
| `$grid-container-class`       | `'container'`       | Css-класс для блоков-контейнеров
| `$grid-container-fluid-class` | `'container-fluid'` | Css-класс для блоков-контейнеров без ограничения ширины
| `$grid-row-class`             | `'row'`             | Css-класс для блоков-строк
| `$grid-col-class`             | `'col'`             | Префикс css-класса для блоков-колонок
| `$grid-col-push-classes`      | `true`              | Включает генерацию классов `.col-*-push-*`
| `$grid-col-pull-classes`      | `true`              | Включает генерацию классов `.col-*-pull-*`
| `$grid-col-offset-classes`    | `true`              | Включает генерацию классов `.col-*-offset-*`

##Использование

Использование классов и миксинов практически не отличается от bootstrap. См. документацию к bootstrap.
