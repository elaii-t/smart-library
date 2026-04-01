<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Library</title>
    <style>
        body { font-family: 'Segoe UI', sans-serif; margin: 0; background-color: #ffffff; color: #444; padding-bottom: 80px; }
        
        /* Шапка */
        header { 
            padding: 20px; 
            background-color: #e3f2fd; /* Голубой */
            border-bottom-left-radius: 25px; 
            border-bottom-right-radius: 25px; 
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
        }

        .search-bar { 
            background: white; padding: 12px; border-radius: 12px; 
            display: flex; align-items: center; color: #999; font-size: 0.9rem;
            cursor: pointer;
        }

        .container { padding: 20px; }
        h2 { font-size: 1.1rem; text-transform: uppercase; color: #555; margin: 25px 0 10px 0; }

        /* Ленты книг */
        .book-row { display: flex; overflow-x: auto; gap: 15px; padding: 10px 5px; scrollbar-width: none; }
        .book-row::-webkit-scrollbar { display: none; }

        .book-card { 
            min-width: 115px; height: 170px; 
            background-color: #fce4ec; /* Розовый */
            border-radius: 15px; overflow: hidden;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            transition: 0.2s;
            border: 1px solid #f8bbd0;
            cursor: pointer;
        }

        /* Эффект нажатия */
        .book-card:active { transform: scale(0.92); }

        .book-card img { width: 100%; height: 100%; object-fit: cover; }
        
        /* Меню внизу */
        nav { 
            position: fixed; bottom: 0; width: 100%; background: white; 
            display: flex; justify-content: space-around; padding: 15px 0; 
            border-top: 1px solid #eee; box-shadow: 0 -2px 10px rgba(0,0,0,0.05);
        }

        .nav-icon { font-size: 1.7rem; color: #d4a5b2; cursor: pointer; transition: 0.2s; }
        .nav-icon:active { color: #f06292; transform: scale(1.2); }
    </style>
</head>
<body>

<header>
    <div class="search-bar" onclick="alert('Поиск скоро заработает! 🔎')">
        🔍 Найти книгу...
    </div>
</header>

<div class="container">
    <h2>Детективы</h2>
    <div class="book-row">
        <div class="book-card" onclick="alert('Открываем книгу: Шерлок Холмс')">
            <img src="https://m.media-amazon.com/images/I/719SshS3p9L.jpg" alt="Sherlock">
        </div>
        <div class="book-card" onclick="alert('Открываем книгу: Убийство в Восточном экспрессе')">
            <img src="https://m.media-amazon.com/images/I/71YvU5pXfWL.jpg" alt="Agatha">
        </div>
        <div class="book-card" onclick="alert('Открываем книгу: Черный кот')">
            <img src="https://m.media-amazon.com/images/I/81vR11p48eL.jpg" alt="Poe">
        </div>
    </div>

    <h2>Романтика</h2>
    <div class="book-row">
        <div class="book-card" onclick="alert('Открываем книгу: Гордость и предубеждение')">
            <img src="https://m.media-amazon.com/images/I/91p5D8Vst9L.jpg" alt="Austen">
        </div>
        <div class="book-card" onclick="alert('Открываем книгу: Сумерки')">
            <img src="https://m.media-amazon.com/images/I/615ZIxED8YL.jpg" alt="Twilight">
        </div>
        <div class="book-card" onclick="alert('Открываем книгу: Маленькие женщины')">
            <img src="https://m.media-amazon.com/images/I/91mS39G-u0L.jpg" alt="Alcott">
        </div>
    </div>

    <h2>Психология</h2>
    <div class="book-row">
        <div class="book-card" onclick="alert('Этот раздел наполнится завтра! 📚')">
            <div style="padding: 50px 10px; text-align: center; font-size: 0.8rem; color: #d4a5b2;">Скоро здесь будут обложки...</div>
        </div>
    </div>
</div>

<nav>
    <span class="nav-icon" onclick="alert('Ваш список прочитанного пока пуст 📋')">📋</span>
    <span class="nav-icon" onclick="alert('Вы уже на Главной странице 🏠')">🏠</span>
    <span class="nav-icon" onclick="alert('Книга добавлена в избранное! ⭐')">⭐</span>
</nav>

</body>
</html>
