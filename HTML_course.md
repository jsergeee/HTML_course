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

___



---

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

---

Существует несколько способов создания графических элементов в HTML, помимо использования CSS для стилизации элементов, как в приведенном вами примере. Вот некоторые из них:

### 1. SVG (Scalable Vector Graphics)
SVG — это формат векторной графики, который позволяет создавать графику с помощью XML. SVG идеально подходит для создания масштабируемых изображений, таких как иконки и иллюстрации.

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SVG Квадрат</title>
</head>
<body>
    <svg width="100" height="100">
        <rect width="100" height="100" style="fill:blue;" />
    </svg>
</body>
</html>
```

### 2. Canvas
Canvas позволяет рисовать графику с помощью JavaScript. Это подходит для динамической графики, такой как игры или анимации.

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Canvas Квадрат</title>
</head>
<body>
    <canvas id="myCanvas" width="100" height="100" style="border:1px solid #000000;"></canvas>
    <script>
        var canvas = document.getElementById('myCanvas');
        var ctx = canvas.getContext('2d');
        ctx.fillStyle = 'blue';
        ctx.fillRect(0, 0, 100, 100);
    </script>
</body>
</html>
```

### 3. CSS Shapes
CSS также позволяет создавать различные формы с помощью свойств, таких как `border-radius`, `clip-path` и т.д.

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Круг</title>
    <style>
        .circle {
            width: 100px;
            height: 100px;
            background-color: blue;
            border-radius: 50%; /* Создает круг */
        }
    </style>
</head>
<body>
    <div class="circle"></div>
</body>
</html>
```

### 4. Использование изображений
Вы можете использовать изображения в формате PNG, JPEG, GIF и других, чтобы создавать графические элементы. Это можно сделать с помощью элемента `<img>` или как фон с помощью CSS.

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Изображение</title>
</head>
<body>
    <img src="path/to/image.png" alt="Пример изображения" width="100" height="100">
</body>
</html>
```

### 5. CSS Gradients
CSS позволяет создавать градиенты, которые также могут служить фоном или цветом для элементов.

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Градиент</title>
    <style>
        .gradient {
            width: 100px;
            height: 100px;
            background: linear-gradient(to right, red, blue); /* Градиент от красного к синему */
        }
    </style>
</head>
<body>
    <div class="gradient"></div>
</body>
</html>
```

### 6. WebGL
WebGL — это JavaScript API для рендеринга 2D и 3D графики в браузере. Он более сложен в использовании, но позволяет создавать интерактивную 3D графику.

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WebGL Пример</title>
</head>
<body>
    <canvas id="glCanvas" width="640" height="480"></canvas>
    <script>
        var canvas = document.getElementById('glCanvas');
        var gl = canvas.getContext('webgl');
        if (!gl) {
            console.log('WebGL не поддерживается');
        }
        // Здесь можно добавить код для отрисовки графики с помощью WebGL
    </script>
</body>
</html>```
```







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





### Урок 6. Структура HTML5

На этом уроке

1. Новые семантические элементы
2. Модерация стандартной html формы
3. Добавление аудио и видео на страницу

---

Вот более полный и исчерпывающий перечень семантических и структурных элементов HTML5, которые помогают организовать контент на веб-страницах:

▎Семантические элементы

1. article - независимый блок контента.

2. section - секция, содержащая тематически связанный контент.

3. nav - навигационное меню.

4. header - заголовок секции или страницы.

5. footer - нижняя часть секции или страницы.

6. aside - контент, связанный с основным, но не являющийся его частью. Можно убрать без потери смысла страницы.

7. h1, h2, h3, h4, h5, h6 - заголовки различных уровней.

8. figure - иллюстрация или графика с возможной подписью.

9. figcaption - подпись к элементу figure.

10. main - основной контент документа.

11. time - дата или время.

12. mark - выделенный текст.

13. progress - прогресс выполнения задачи.

14. meter - измерение в пределах диапазона.

15. details - скрытый контент, который можно раскрыть.

16. summary - заголовок для элемента details.

17. dialog - диалоговое окно.

18. address - контактная информация.

19. template - шаблон для динамического контента.

20. slot - используется в Web Components для определения мест вставки.

▎Элементы для графики и мультимедиа

21. canvas - для рисования графики с помощью JavaScript.

22. svg - для векторной графики.

23. audio - для встраивания аудиофайлов.

24. video - для встраивания видеопотоков.

25. track - для добавления текстовых дорожек к элементам video и audio.

▎Формы и элементы управления

26. form - форма для ввода данных.

27. input - элемент для ввода данных.

28. textarea - многострочное текстовое поле.

29. button - кнопка для взаимодействия.

30. select - выпадающий список.

31. option - элемент выбора в списке.

32. label - метка для элемента формы.

33. fieldset - группа элементов формы.

34. legend - заголовок для элемента fieldset.

▎Интерактивные элементы

35. iframe - встраивание другого HTML-документа.

36. embed - встраивание внешнего контента (например, Flash).

37. object - для встраивания мультимедийных объектов.

38. param - параметры для элемента object.

▎Дополнительные элементы

39. script - для встраивания JavaScript.

40. noscript - контент, отображаемый, если JavaScript отключен.

41. link - связь с внешним ресурсом, например, CSS.

42. meta - метаданные о документе.

43. title - заголовок документа.

Этот перечень охватывает большинство семантических и структурных элементов HTML5, которые могут быть использованы для создания веб-страниц. Однако стоит отметить, что HTML продолжает развиваться, и новые элементы могут быть добавлены в будущих версиях.

---



 # Урок 7. Новые возможности CSS3



## На этом уроке:

1. Псевдоклассы и псевдоэлементы

2. Работа с svg

3. Эффекты перехода

4. Эффекты трансформации

5. Эффекты анимации

   ---

   

HTML эффекты наведения и трансформации можно реализовать с помощью CSS. Ниже приведены примеры простых эффектов наведения и трансформации, которые можно использовать в ваших проектах.

▎Пример 1: Эффект наведения на кнопку

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Эффект наведения</title>
    <style>
        .button {
            padding: 15px 30px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }

        .button:hover {
            background-color: #0056b3;
            transform: scale(1.1);
        }
    </style>
</head>
<body>

    <button class="button">Наведи на меня</button>

</body>
</html>


▎Пример 2: Эффект наведения на изображение

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Эффект наведения на изображение</title>
    <style>
        .image-container {
            overflow: hidden;
            border-radius: 10px;
            transition: transform 0.3s;
        }

        .image-container img {
            width: 100%;
            transition: transform 0.3s;
        }
    
        .image-container:hover img {
            transform: scale(1.1);
        }
    </style>
</head>
<body>

    <div class="image-container">
        <img src="https://via.placeholder.com/300" alt="Пример изображения">
    </div>

</body>
</html>


▎Пример 3: Эффект наведения на карточку

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Эффект наведения на карточку</title>
    <style>
        .card {
            width: 300px;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            border-radius: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
            margin: 20px;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body>

    <div class="card">
        <h3>Заголовок карточки</h3>
        <p>Некоторый текст внутри карточки.</p>
    </div>

</body>
</html>


▎Объяснение:

1. Эффект наведения на кнопку: При наведении на кнопку изменяется цвет фона и масштабируется кнопка.

2. Эффект наведения на изображение: При наведении изображение увеличивается, создавая эффект "приближения".

3. Эффект наведения на карточку: При наведении карточка поднимается и увеличивается тень, создавая эффект "подъема".

Вы можете адаптировать эти примеры под свои нужды, изменяя цвета, размеры и другие свойства.