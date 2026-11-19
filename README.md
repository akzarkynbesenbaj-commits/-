
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Мир природы и путешествий</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f4f8f5;
    color: #333;
}

header {
    background: #247a58;
    color: white;
    text-align: center;
    padding: 45px 20px;
}

header h1 {
    font-size: 36px;
}

nav {
    background: #194d3a;
    padding: 18px;
    text-align: center;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 15px;
    font-weight: bold;
}

nav a:hover {
    color: #a8e6c3;
}

section {
    padding: 35px 20px;
    text-align: center;
}

.intro {
    max-width: 850px;
    margin: auto;
    line-height: 1.7;
}

.photos {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
}

.photos img {
    width: 280px;
    height: 200px;
    object-fit: cover;
    border-radius: 12px;
    transition: 0.3s;
}

.photos img:hover {
    transform: scale(1.05);
}

.card {
    background: white;
    padding: 20px;
    border-radius: 12px;
    width: 280px;
    box-shadow: 0 3px 10px #00000015;
}

.cards {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
}

button {
    background: #247a58;
    color: white;
    padding: 12px 25px;
    border: none;
    border-radius: 7px;
    cursor: pointer;
}

button:hover {
    background: #194d3a;
}

footer {
    background: #194d3a;
    color: white;
    text-align: center;
    padding: 25px;
}

@media(max-width: 600px) {
    header h1 {
        font-size: 26px;
    }

    nav a {
        display: inline-block;
        margin: 8px;
    }

    .photos img {
        width: 100%;
    }
}
</style>
</head>

<body>

<header id="home">
    <h1>🌿 Мир природы и путешествий</h1>
    <p>Открой для себя красоту нашей планеты!</p>
</header>

<nav>
    <a href="#home">Главная</a>
    <a href="#about">О природе</a>
    <a href="#photos">Галерея</a>
    <a href="#places">Путешествия</a>
    <a href="#contact">Контакты</a>
</nav>

<section id="about">
    <div class="intro">
        <h2>Добро пожаловать!</h2>
        <p>
        Природа — это удивительный мир, который окружает нас каждый день.
        В нём есть красивые горы, зелёные леса, чистые озёра,
        реки и множество удивительных животных.
        </p>
        <p>
        Наш сайт создан для тех, кто любит путешествовать,
        узнавать новое и любоваться красотой окружающего мира.
        </p>
    </div>
</section>

<section>
    <h2>Почему важно беречь природу?</h2>

    <div class="cards">
        <div class="card">
            <h3>🌳 Чистый воздух</h3>
            <p>Деревья помогают очищать воздух и поддерживать жизнь на Земле.</p>
        </div>

        <div class="card">
            <h3>💧 Чистая вода</h3>
            <p>Вода необходима всем живым организмам.</p>
        </div>

        <div class="card">
            <h3>🐾 Защита животных</h3>
            <p>Каждое животное играет важную роль в природе.</p>
        </div>
    </div>
</section>

<section id="photos">
    <h2>Фотогалерея природы</h2>
    <p>Посмотрите, насколько прекрасен наш мир!</p>

    <div class="photos">
        <img src="https://picsum.photos/id/10/500/350" alt="Лес">
        <img src="https://picsum.photos/id/15/500/350" alt="Природа">
        <img src="https://picsum.photos/id/29/500/350" alt="Горы">
        <img src="https://picsum.photos/id/28/500/350" alt="Озеро">
        <img src="https://picsum.photos/id/17/500/350" alt="Пейзаж">
        <img src="https://picsum.photos/id/19/500/350" alt="Водопад">
    </div>
</section>

<section id="places">
    <h2>Интересные места для путешествий</h2>

    <div class="cards">
        <div class="card">
            <h3>🏔 Горы</h3>
            <p>Горы привлекают туристов своими красивыми пейзажами и свежим воздухом.</p>
        </div>

        <div class="card">
            <h3>🌊 Озёра</h3>
            <p>Озёра — прекрасные места для отдыха и знакомства с природой.</p>
        </div>

        <div class="card">
            <h3>🌲 Леса</h3>
            <p>Леса дарят спокойствие, чистый воздух и удивительные впечатления.</p>
        </div>
    </div>
</section>

<section>
    <h2>Наш интересный факт</h2>
    <p>На Земле существует огромное разнообразие растений и животных.</p>
    <button onclick="showFact()">Узнать интересный факт</button>
    <p id="fact"></p>
</section>

<section id="contact">
    <h2>Свяжитесь с нами</h2>
    <p>Спасибо, что посетили наш сайт!</p>
    <p>Изучайте природу, путешествуйте и берегите нашу планету ❤️</p>
</section>

<footer>
    <p>© 2026 Мир природы и путешествий</p>
    <p>Создано с помощью HTML и CSS</p>
</footer>

<script>
function showFact() {
    let facts = [
        "Океаны покрывают большую часть поверхности Земли!",
        "Бамбук может расти очень быстро!",
        "В лесах живёт огромное количество животных!",
        "Самое большое животное на Земле — синий кит!"
    ];

    let random = Math.floor(Math.random() * facts.length);
    document.getElementById("fact").innerText = facts[random];
}
</script>

</body>
</html>
