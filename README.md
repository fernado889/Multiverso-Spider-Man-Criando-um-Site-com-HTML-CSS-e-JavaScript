# Multiverso-Spider-Man-Criando-um-Site-com-HTML-CSS-e-JavaScript
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Multiverso Spider-Man</title>
</head>
<body>
    <header>
        <h1>Multiverso Spider-Man</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#personagens">Personagens</a></li>
                <li><a href="#filmes">Filmes</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Bem-vindo ao Multiverso!</h2>
            <p>Explore os diferentes universos do Spider-Man.</p>
        </section>

        <section id="personagens">
            <h2>Personagens</h2>
            <div class="card">
                <img src="spiderman1.jpg" alt="Spider-Man 1">
                <h3>Spider-Man 2099</h3>
                <p>Um herói do futuro com habilidades impressionantes.</p>
            </div>
            <div class="card">
                <img src="spiderman2.jpg" alt="Spider-Man 2">
                <h3>Spider-Gwen</h3>
                <p>Uma versão alternativa da Spider-Woman.</p>
            </div>
            <!-- Adicione mais cards conforme necessário -->
        </section>

        <section id="filmes">
            <h2>Filmes</h2>
            <p>Confira os filmes mais populares do Spider-Man!</p>
            <!-- Aqui você pode adicionar uma lista ou links para os filmes -->
        </section>

        <section id="contato">
            <h2>Contato</h2>
            <form id="contact-form">
                <label for="name">Nome:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                
                <label for="message">Mensagem:</label>
                <textarea id="message" name="message" required></textarea>
                
                <button type="submit">Enviar</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Multiverso Spider-Man. Todos os direitos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background: #ff0000;
    color: white;
    padding: 10px 20px;
    text-align: center;
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
    color: white;
    text-decoration: none;
}

main {
    padding: 20px;
}

.card {
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px;
    padding: 10px;
    text-align: center;
    background: white;
}

.card img {
    width: 100px;
    height: auto;
}

footer {
    text-align: center;
    padding: 10px 0;
    background: #222;
    color: white;
}
document.getElementById('contact-form').addEventListener('submit', function(event) {
    event.preventDefault(); // Evita o envio padrão do formulário

    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;

    alert(`Obrigado, ${name}! Sua mensagem foi enviada.`);
