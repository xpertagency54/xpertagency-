# xpertagency-<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Xpert Agency</title>
<link rel="icon" href="https://upload.wikimedia.org/wikipedia/commons/7/7e/Globe_icon.svg" type="image/png">
<style>
    body {
        margin: 0;
        font-family: 'Poppins', sans-serif;
        background: linear-gradient(135deg, #0D1B2A, #1E90FF);
        color: white;
        scroll-behavior: smooth;
    }
    header {
        position: fixed;
        width: 100%;
        top: 0;
        background: rgba(0, 0, 0, 0.6);
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 30px;
        z-index: 1000;
    }
    header img {
        height: 50px;
        animation: zoomIn 1s ease-in-out;
    }
    nav a {
        color: white;
        margin-left: 20px;
        text-decoration: none;
        font-weight: bold;
    }
    nav a:hover {
        color: #1E90FF;
    }
    section {
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 50px;
    }
    h1 {
        font-size: 3em;
        margin-bottom: 10px;
        text-shadow: 2px 2px 8px rgba(0,0,0,0.6);
        animation: fadeInUp 1s ease-in-out;
    }
    p {
        max-width: 700px;
        font-size: 1.2em;
        animation: fadeIn 1.2s ease-in-out;
    }
    .btn {
        margin-top: 20px;
        padding: 15px 25px;
        background: #1E90FF;
        color: white;
        border: none;
        border-radius: 5px;
        text-decoration: none;
        font-size: 1em;
        transition: background 0.3s ease;
    }
    .btn:hover {
        background: #0D1B2A;
    }
    #topBtn {
        display: none;
        position: fixed;
        bottom: 20px;
        right: 30px;
        z-index: 99;
        background-color: #1E90FF;
        color: white;
        padding: 10px 15px;
        border-radius: 5px;
        cursor: pointer;
    }
    #topBtn:hover {
        background-color: #0D1B2A;
    }
    @keyframes zoomIn {
        from { transform: scale(0.8); opacity: 0; }
        to { transform: scale(1); opacity: 1; }
    }
    @keyframes fadeInUp {
        from { transform: translateY(20px); opacity: 0; }
        to { transform: translateY(0); opacity: 1; }
    }
    @keyframes fadeIn {
        from { opacity: 0; }
        to { opacity: 1; }
    }
</style>
</head>
<body>

<header>
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/7e/Globe_icon.svg" alt="Xpert Agency Logo">
    <nav>
        <a href="#services">Services</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section id="home">
    <h1>Votre image en ligne, sublimée par l’expertise.</h1>
    <p>Sites web, logos et stratégies digitales haut de gamme – Nancy, France.</p>
    <a href="https://wa.me/33760507044" class="btn">Contact WhatsApp</a>
    <a href="https://wa.me/33760507044?text=Je%20souhaite%20demander%20un%20devis" class="btn">Demander un devis</a>
</section>

<section id="services">
    <h1>Nos Services</h1>
    <p>Création de sites web, conception de logos, communication digitale et plus encore.</p>
</section>

<section id="portfolio">
    <h1>Portfolio</h1>
    <p>Découvrez nos projets récents et notre savoir-faire.</p>
</section>

<section id="contact">
    <h1>Contact</h1>
    <p>Localisation : Nancy, France</p>
    <a href="https://wa.me/33760507044" class="btn">Nous écrire sur WhatsApp</a>
</section>

<button onclick="topFunction()" id="topBtn">↑ Haut</button>

<script>
    let mybutton = document.getElementById("topBtn");
    window.onscroll = function() {scrollFunction()};
    function scrollFunction() {
        if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
            mybutton.style.display = "block";
        } else {
            mybutton.style.display = "none";
        }
    }
    function topFunction() {
        document.body.scrollTop = 0;
        document.documentElement.scrollTop = 0;
    }
</script>

</body>
</html>
