<!DOCTYPE html>
<html lang="no">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Verkstedweb - Webdesign for små bedrifter</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="scripts.js"></script>
</head>
<body>
    <header>
        <nav class="navbar">
            <a href="#" class="logo">Verkstedweb</a>
            <ul class="nav-links">
                <li><a href="#services">Tjenester</a></li>
                <li><a href="#about">Om Oss</a></li>
                <li><a href="#contact">Kontakt</a></li>
            </ul>
            <button class="nav-toggle" aria-label="Toggle navigation">
                <span class="hamburger"></span>
            </button>
        </nav>
    </header>

    <main>
        <section id="hero">
            <div class="hero-content">
                <h1>Design som skiller seg ut</h1>
                <p>Vi lager nettsider som er skreddersydd for små bedrifter.</p>
                <a href="#contact" class="cta-button">Start Prosjekt</a>
            </div>
        </section>

        <section id="services" class="section">
            <h2>Våre Tjenester</h2>
            <div class="cards">
                <div class="card">
                    <h3>Nettsidedesign</h3>
                    <p>Vi skaper vakre og funksjonelle nettsider som representerer din bedrift.</p>
                </div>
                <div class="card">
                    <h3>SEO Optimalisering</h3>
                    <p>Gjør din nettside synlig på søkemotorer og tiltrekk flere kunder.</p>
                </div>
                <div class="card">
                    <h3>Rådgivning</h3>
                    <p>Vi hjelper deg med å forstå hva din bedrift trenger for å lykkes på nett.</p>
                </div>
            </div>
        </section>

        <section id="about" class="section">
            <h2>Om Oss</h2>
            <p>Verkstedweb er et kreativt byrå som spesialiserer seg på å lage tilpassede nettsider for små bedrifter. Vårt mål er å gi hver klient en unik webopplevelse.</p>
        </section>

        <section id="contact" class="section">
            <h2>Kontakt Oss</h2>
            <form id="contact-form">
                <input type="text" id="name" placeholder="Navn" required>
                <input type="email" id="email" placeholder="E-post" required>
                <textarea id="message" placeholder="Melding" required></textarea>
                <button type="submit">Send Melding</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Verkstedweb. Alle rettigheter reservert.</p>
    </footer>
</body>
</html>
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background-color: #333;
}

.navbar .logo {
    color: #fff;
    text-decoration: none;
    font-size: 1.5rem;
}

.nav-links {
    display: flex;
    list-style: none;
}

.nav-links li {
    margin-left: 20px;
}

.nav-links a {
    color: #fff;
    text-decoration: none;
}

.nav-toggle {
    display: none;
}

#hero {
    background: url('https://source.unsplash.com/random/1600x900') no-repeat center center/cover;
    height: 100vh;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.hero-content h1 {
    font-size: 3rem;
}

.cta-button {
    background-color: #ff4500;
    color: #fff;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

.cta-button:hover {
    background-color: #e63900;
}

.section {
    padding: 50px 20px;
    text-align: center;
}

.cards {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
    justify-content: center;
}

.card {
    background-color: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    width: 300px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

footer {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
    text-align: center;
}
// Mobile navigation toggle
const navToggle = document.querySelector('.nav-toggle');
const navLinks = document.querySelector('.nav-links');

navToggle.addEventListener('click', () => {
    navLinks.classList.toggle('nav-links-visible');
});

// Contact form submission (placeholder for backend integration)
document.getElementById('contact-form').addEventListener('submit', function (event) {
    event.preventDefault();
    alert('Takk for at du kontaktet oss! Vi vil svare deg snarest mulig.');
});
git add index.html styles.css scripts.js
git commit -m "La til avansert nettside for Verkstedweb"
git push origin main
