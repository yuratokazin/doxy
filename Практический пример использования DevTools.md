## Практический пример использования DevTools

### Структура проекта

Для демонстрации создадим простой проект с файлами:

**index.html**

html

```html
<!DOCTYPE html>
<html>
<head>
    <title>DevTools Demo</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <button class="button">Нажми меня!</button>
        <div class="color-box">
            <p>Измени мой цвет!</p>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
```

**style.css**

css

```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.button {
    padding: 20px 40px;
    background: #007bff;
    color: white;
    border: none;
    cursor: pointer;
}

.color-box {
    width: 200px;
    height: 200px;
    background: #f8f9fa;
    margin-top: 20px;
}
```

**script.js**

javascript

```javascript
document.addEventListener('DOMContentLoaded', () => {
    const button = document.querySelector('.button');
    
    button.addEventListener('click', () => {
        alert('Привет от DevTools!');
    });
});
```

### Демонстрация возможностей

1. **Адаптивная вёрстка**

- Откройте DevTools (F12 или Ctrl+Shift+I)
- Нажмите **Ctrl+Shift+M** для активации режима адаптивности
- Покажите, как меняется макет при разных разрешениях
- Демонстрируйте эмуляцию touch-событий

1. **Отладка CSS**

- Найдите элемент `.container` во вкладке **Elements**
- Покажите, как меняются свойства при наведении
- Демонстрируйте работу с Flexbox
- Покажите, как проверить переопределение стилей

1. **Оптимизация загрузки**

- Перейдите во вкладку **Network**
- Покажите список загружаемых ресурсов
- Проанализируйте время загрузки каждого файла
- Демонстрируйте кэширование

1. **Работа с цветами**

- Выберите элемент `.color-box`
- Кликните на цветовой квадрат в стилях
- Покажите палитру цветов
- Демонстрируйте конвертацию между форматами

1. **Тестирование JavaScript**

- Откройте консоль (**Console**)
- Введите `document.querySelector('.button')`
- Покажите работу с `$0`
- Демонстрируйте отладку событий

### Дополнительные возможности для демонстрации

- **Lighthouse** для анализа производительности
- **Performance** для профилирования
- **Memory** для анализа использования памяти
- **Sources** для отладки JavaScript

### Практические задания

1. Измените цвет кнопки через DevTools
2. Добавьте новый стиль для псевдокласса :hover
3. Проверьте работу сайта на разных устройствах
4. Оптимизируйте размер изображений
5. Добавьте новое событие клика через консоль

Этот пример позволит наглядно продемонстрировать все основные возможности  DevTools и дать студентам практический опыт работы с инструментами  разработчика.