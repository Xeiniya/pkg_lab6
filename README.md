# 3D БУКВА "H" С ОРТОГРАФИЧЕСКИМИ ПРОЕКЦИЯМИ

Этот проект реализует отображение трехмерной буквы "H" с возможностью управления её трансформациями и отображения ортографических проекций. Веб-приложение использует библиотеку Three.js для рендеринга 3D объектов и их проекций.

## Описание задачи

Задача проекта заключается в создании интерактивной веб-страницы, на которой отображается трехмерная буква "H", и предоставляется возможность управлять её трансформациями: вращением, масштабированием и перемещением. Также предусмотрены ортографические проекции этой буквы на три основные плоскости: Oxy, Oxz и Oyz. Для управления используются ползунки для изменения параметров трансформаций, а также отображается матрица преобразования текущего состояния объекта.

## Установка и использование

Чтобы запустить приложение, выполните следующие шаги:

1. Скачайте или скопируйте HTML-файл на ваш компьютер.
2. Откройте файл в браузере, поддерживающем WebGL (например, Google Chrome, Firefox или Edge).

### Управление:

- **Вращение**: Используйте ползунки для изменения углов вращения по осям X и Y.
- **Масштабирование**: Изменяйте масштаб буквы по осям X, Y и Z.
- **Перемещение**: Используйте ползунки для перемещения буквы по осям X, Y и Z.

Проекции будут автоматически обновляться при изменении параметров трансформации.

### Проекции:
- **Oxy**: Проекция на плоскость X-Y.
- **Oxz**: Проекция на плоскость X-Z.
- **Oyz**: Проекция на плоскость Y-Z.

### Матрица преобразования:
- В разделе "Матрица преобразования текущего состояния объекта" будет отображаться текущая матрица трансформаций буквы "H". Каждый элемент матрицы отображается с точностью до одного знака после запятой.

## Используемые технологии

- **Three.js**: JavaScript библиотека для рендеринга 3D-графики в браузере с использованием WebGL.
- **OrbitControls.js**: Расширение для управления камерой с помощью мыши (поворот, зум, панорамирование).
- **HTML5 Canvas**: Используется для рендеринга 3D-объектов и их проекций.

## Структура проекта

Проект состоит из одного HTML файла, который включает:
- Веб-страницу с элементами управления (ползунки для трансформаций).
- Основной рендер для отображения 3D буквы.
- Канвас для отображения ортографических проекций.

### Основные функции:
- **createThickAxes()**: Функция для создания и добавления координатных осей в сцену.
- **fontLoader.load()**: Загрузка шрифта и создание 3D текста (буквы "H").
- **updateTransform()**: Обновление трансформаций объекта на основе значений ползунков.
- **animate()**: Анимация и рендеринг сцены, обновление всех проекций.

## Пример использования:

1. Откройте файл в браузере.
2. Используйте ползунки для изменения параметров трансформации.
3. Наблюдайте за тем, как буква "H" меняет своё положение, масштаб и ориентацию.
4. Просматривайте ортографические проекции буквы на разные плоскости.
5. Матрица преобразования будет отображаться в реальном времени, показывая текущие изменения.

## Примечания

- Для корректного отображения 3D-графики необходима поддержка WebGL в вашем браузере.
- Для лучшего опыта рекомендуется использовать современные браузеры, такие как Chrome или Firefox.

Этот проект предоставляет базовую платформу для визуализации и изучения трансформаций 3D объектов, а также их проекций в различных плоскостях.
