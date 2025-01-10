# Основное

Основные блоки сайта могут варьироваться в зависимости от его назначения и дизайна, но обычно включают в себя следующие элементы:

1. Шапка (Header): верхняя часть страницы, которая обычно содержит логотип, навигационное меню, контактную информацию и, возможно, кнопки для входа или регистрации.

2. Основной контент (Main Content): центральная часть страницы, где размещается основная информация, статьи, изображения или другие материалы.

3. Боковая панель (Sidebar): дополнительная область, которая может содержать ссылки на другие страницы, виджеты, рекламу или дополнительную информацию.

4. Подвал (Footer): нижняя часть страницы, которая часто включает в себя информацию о компании, ссылки на политику конфиденциальности, условия использования, контактные данные и социальные сети.

5. Форма обратной связи (Contact Form): блок, позволяющий пользователям отправлять сообщения или запросы.

6. Слайдер (Slider): элемент, который отображает изображения или информацию в виде слайдов, часто используется для акций или новостей.

7. Галерея (Gallery): блок для отображения изображений или видео.

8. Отзывы (Testimonials): раздел, где пользователи могут оставить свои отзывы о продукте или услуге.

9. Кнопки призыва к действию (Call to Action, CTA): элементы, которые побуждают пользователя выполнить определенное действие, например, подписаться на рассылку или сделать покупку.

Эти блоки могут комбинироваться и адаптироваться в зависимости от специфики сайта и потребностей его аудитории.

## Фиргуры	

В HTML для создания фигур можно использовать различные подходы, включая CSS для стилизации элементов. Вот несколько примеров, как создать простые фигуры с помощью HTML и CSS:

▎1. Квадрат

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Квадрат</title>
    <style>
        .square {
            width: 100px;
            height: 100px;
            background-color: blue;
        }
    </style>
</head>
<body>
    <div class="square"></div>
</body>
</html>


▎2. Прямоугольник

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Прямоугольник</title>
    <style>
        .rectangle {
            width: 200px;
            height: 100px;
            background-color: green;
        }
    </style>
</head>
<body>
    <div class="rectangle"></div>
</body>
</html>


▎3. Круг

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Круг</title>
    <style>
        .circle {
            width: 100px;
            height: 100px;
            background-color: red;
            border-radius: 50%;
        }
    </style>
</head>
<body>
    <div class="circle"></div>
</body>
</html>


▎4. Треугольник

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Треугольник</title>
    <style>
        .triangle {
            width: 0;
            height: 0;
            border-left: 50px solid transparent;
            border-right: 50px solid transparent;
            border-bottom: 100px solid orange;
        }
    </style>
</head>
<body>
    <div class="triangle"></div>
</body>
</html>



▎5. Эллипс

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Эллипс</title>
    <style>
        .ellipse {
            width: 150px;
            height: 100px;
            background-color: purple;
            border-radius: 75px / 50px;
        }
    </style>
</head>
<body>
    <div class="ellipse"></div>
</body>
</html>


Эти примеры демонстрируют, как с помощью HTML и CSS можно создать базовые фигуры. Вы можете изменять размеры, цвета и другие свойства, чтобы адаптировать фигуры под ваши нужды.



# Урок 4. Основы позиционирования

 

В HTML и CSS существует несколько способов выравнивания элементов. Вот основные методы и их применение:

### 1. Выравнивание текста

Выравнивание текста можно осуществить с помощью свойства `text-align`:

```css
.container {
    text-align: center; /* center, left, right, justify */
}
```

### 2. Выравнивание с помощью Flexbox

Flexbox позволяет легко выравнивать элементы как по горизонтали, так и по вертикали.

```css
.container {
    display: flex;
    justify-content: center; /* center, flex-start, flex-end, space-between, space-around, space-evenly */
    align-items: center; /* center, flex-start, flex-end, baseline, stretch */
    height: 100vh; /* Установите высоту контейнера для вертикального выравнивания */
}
```

### 3. Выравнивание с помощью Grid

CSS Grid также предлагает мощные инструменты для выравнивания.

```css
.container {
    display: grid;
    place-items: center; /* Центрирование по обеим осям */
    height: 100vh; /* Установите высоту контейнера для вертикального выравнивания */
}
```

### 4. Выравнивание с помощью Margin

Для блочных элементов можно использовать `margin` для центрирования:

```css
.element {
    margin: 0 auto; /* Центрирование по горизонтали */
    width: 50%; /* Установите ширину элемента */
}
```

### 5. Выравнивание с помощью Position

С помощью абсолютного позиционирования можно выровнять элемент в родительском контейнере:

```css
.container {
    position: relative;
    height: 100vh;
}

.element {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%); /* Центрирование по обеим осям */
}
```

### 6. Выравнивание в таблицах

Если вы используете таблицы, выравнивание можно задать с помощью атрибутов или CSS:

```css
table {
    width: 100%;
}

td {
    text-align: center; /* center, left, right */
    vertical-align: middle; /* top, middle, bottom */
}
```

### 7. Использование `line-height`

Для вертикального выравнивания текста внутри элемента можно использовать `line-height`:

```css
.element {
    height: 100px; /* Установите высоту элемента */
    line-height: 100px; /* Установите line-height равным высоте для вертикального выравнивания */
    text-align: center; /* Центрирование текста по горизонтали */
}
```

### 8. Flexbox для колонок

Если вы хотите выровнять элементы в колонках:

```css
.container {
    display: flex;
    flex-direction: column; /* Вертикальное выравнивание */
    justify-content: space-between; /* space-between, space-around, center */
}
```

### Пример использования

Вот пример, который объединяет несколько методов выравнивания:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Выравнивание в HTML и CSS</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #f0f0f0;
        }
        .container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
        }
        .item {
            background-color: #007BFF;
            color: white;
            padding: 20px;
            text-align: center;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">Элемент 1</div>
        <div class="item">Элемент 2</div>
        <div class="item">Элемент3</div>
</body>
</html>
```

В этом примере используется Flexbox для центрирования контейнера, а также CSS Grid для выравнивания элементов внутри контейнера. Вы можете комбинировать эти методы в зависимости от требований вашего дизайна.



# Урок 5. Основы создания адаптивного сайта

Основные инструменты для сохранения размеров элементов сайта для всех размеров экрана используются

in-height: 

max-height: 

min-width: 

max-width: 

можно использовать единицы измерения в % тогда элемент будет изменять свои размеры, при изменении разрешения браузера

Помимо этого очень эффективны единицы  vw vh - означают пропорцию от ширину экрана и высоту экрана 

  width: 100vw;

  height: 100vh;



### Медиазапросы

Синтаксис Все запросы начинаются с правила @media, после чего следует условие, в котором используются типы носителей, логические операторы и медиафункции.

