git clone https://github.com/ditt-brukernavn/verkstedweb.git
cd verkstedweb
<!DOCTYPE html>
<html lang="no">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Verkstedweb - Design av nettsider</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Velkommen til Verkstedweb!</h1>
        <nav>
            <ul>
                <li><a href="#services">Tjenester</a></li>
                <li><a href="#about">Om Oss</a></li>
                <li><a href="#contact">Kontakt</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="services">
            <h2>Våre Tjenester</h2>
            <p>Vi designer nettsider for mindre bedrifter med fokus på kvalitet og kreativitet.</p>
        </section>
        <section id="about">
            <h2>Om Oss</h2>
            <p>Vi er et dedikert team av webdesignere som har som mål å hjelpe små bedrifter med å etablere en profesjonell tilstedeværelse på nettet.</p>
        </section>
        <section id="contact">
            <h2>Kontakt Oss</h2>
            <p>Send oss en e-post på <a href="mailto:kontakt@verkstedweb.no">kontakt@verkstedweb.no</a> eller fyll ut skjemaet nedenfor:</p>
            <form action="submit_form.php" method="post">
                <label for="name">Navn:</label>
                <input type="text" id="name" name="name" required>
                <label for="email">E-post:</label>
                <input type="email" id="email" name="email" required>
                <label for="message">Melding:</label>
                <textarea id="message" name="message" required></textarea>
                <button type="submit">Send</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Verkstedweb. Alle rettigheter reservert.</p>
    </footer>
    <script src="scripts.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
    text-align: center;
}

header h1 {
    margin: 0;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

main {
    padding: 20px;
}

section {
    margin-bottom: 20px;
}

form {
    display: grid;
    gap: 10px;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    bottom: 0;
    width: 100%;
}
// Her kan du legge til JavaScript-kode hvis nødvendig.
console.log('Verkstedweb nettside lastet.');
git add index.html styles.css scripts.js
git commit -m "Initial commit med grunnleggende nettsideoppsett"
git push origin main
