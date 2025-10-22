<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        * {
            Box-sizing: border-box;
            Margin: 0;
            Padding: 0;
        }
        
        Body {
            Padding: 15 px;
            Font-family: Arial, sans-serif;
        }
        
        /* Адаптивный Grid */
        .adaptive-grid {
            Display: grid;
            Grid-template-columns: repeat (auto-fit, minmax (150 px, 1 fr));
            Gap: 10 px;
        }
        
        .item {
            Padding: 20 px;
            background: #2196F3 ;
            Color: white;
            Border-radius: 8 px;
            Text-align: center;
        }
        
        /* Медиа-запрос для ОЧЕНЬ маленьких экранов */
        @media (max-width: 360 px) {
            .adaptive-grid {
                Grid-template-columns: 1 fr 1 fr; /* Принудительно 2 колонки */
            }
        }
    </style>
</head>
<body>
    <h1>📱 Умная адаптация</h1>
    
    <div class="adaptive-grid">
        <div class="item">Блок 1</div>
        <div class="item">Блок 2</div>
        <div class="item">Блок 3</div>
        <div class="item">Блок 4</div>
        <div class="item">Блок 5</div>
        <div class="item">Блок 6</div>
    </div>
    
    <p>На обычных телефонах - 2 колонки, на очень узких - тоже 2 колонки</p>
</body>
</html>