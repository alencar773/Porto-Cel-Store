# Porto-Cel-Store

<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Porto Cel</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

<style>
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    background-color: #0b0c14;
    color: #cce6ff;
    text-align: center;
    overflow-x: hidden;
    position: relative;
}

/* Fundo neon animado */
.neon-lines {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    overflow: hidden;
    z-index: 0;
}

.neon-lines div {
    position: absolute;
    width: 2px;
    height: 100%;
    background: linear-gradient(to bottom, #00f0ff, #ff00ff);
    opacity: 0.15;
    animation-name: moveLine;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
}

@keyframes moveLine {
    0% { transform: translateX(0); }
    100% { transform: translateX(100vw); }
}

/* Conteúdo principal acima do fundo */
.content {
    position: relative;
    z-index: 1;
}

/* Topo */
.topo {
    background: linear-gradient(90deg, #ffffff, #0077cc);
    padding: 10px;
}

.topo a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    margin: 0 15px;
}

h1, h2 {
    font-family: 'Orbitron', sans-serif;
    letter-spacing: 2px;
    text-shadow: 0 0 10px #00aaff;
}

.banner {
    padding: 40px 20px;
}

/* Produtos */
.produtos {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    padding: 20px;
}

.card {
    background-color: #1a1a1a;
    width: 140px;
    margin: 15px;
    padding: 15px;
    border-radius: 10px;
    border: 1px solid #00aaff;
    transition: 0.4s;
    opacity: 0;
    transform: translateY(30px);
}

.card.show {
    opacity: 1;
    transform: translateY(0);
}

.card:hover {
    transform: scale(1.05);
    box-shadow: 0 0 20px #00aaff;
}

.card img {
    width: 100%;
    border-radius: 8px;
}

.preco {
    color: #00aaff;
    font-weight: bold;
}

button {
    background-color: #00aaff;
    color: black;
    border: none;
    padding: 10px;
    width: 100%;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
}

button:hover {
    box-shadow: 0 0 15px #00aaff;
}

/* Avaliações */
.avaliacoes {
    padding: 40px 20px;
    background-color: #000;
}

.avaliacoes p {
    color: #ccc;
    max-width: 600px;
    margin: 10px auto;
}

/* Localização */
.localizacao {
    padding: 40px 20px;
}

/* WhatsApp fixo */
.whatsapp-fixo {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #25D366;
    color: white;
    padding: 15px 18px;
    border-radius: 50px;
    text-decoration: none;
    font-weight: bold;
    box-shadow: 0 0 15px #25D366;
}

/* Responsivo */
@media (max-width: 768px) {
    .produtos {
        flex-direction: column;
        align-items: center;
    }
    .card {
        width: 90%;
    }
}
</style>
</head>
<body>

<!-- Fundo Neon -->
<div class="neon-lines">
    <div style="left:5%; animation-duration:12s;"></div>
    <div style="left:20%; animation-duration:15s;"></div>
    <div style="left:35%; animation-duration:18s;"></div>
    <div style="left:50%; animation-duration:20s;"></div>
    <div style="left:65%; animation-duration:14s;"></div>
    <div style="left:80%; animation-duration:17s;"></div>
</div>

<!-- Conteúdo principal -->
<div class="content">

<div class="topo">
    <a href="https://wa.me/5592986319253" target="_blank">📱 WhatsApp</a>
    <a href="https://instagram.com/porto.cell_" target="_blank">📸 Instagram</a>
</div>

<header>
    <img src="portocel.jpeg" width="250">
    <h1>Porto Cel</h1>
    <p>A melhor loja e assistência para seu celular!</p>
</header>

<div class="banner">
    <h2>Tecnologia e acessórios premium</h2>
    <p>Capinhas, carregadores, fones e muito mais!</p>
</div>

<h2>🎧 Fones</h2>
<section class="produtos">
    <div class="card">
        <img src="fonebranco.jpeg">
        <h3>Fone AirDots Pro 3 Branco</h3>
        <p class="preco">R$ 45,00</p>
        <a href="https://wa.me/5592986319253?text=Olá,%20quero%20comprar%20o%20Fone%20Bluetooth%20da%20Porto%20Cel" target="_blank">
            <button>Comprar</button>
        </a>
    </div>
    <div class="card">
        <img src="fonerosa.jpeg">
        <h3>AirDots Pro 3 rosa</h3>
        <p class="preco">R$ 45,00</p>
        <a href="https://wa.me/5592986319253?text=Olá,%20quero%20comprar%20o%20Headset%20Gamer%20da%20Porto%20Cel" target="_blank">
            <button>Comprar</button>
        </a>
    </div>
    <div class="card">
        <img src="fonepreto.jpeg">
        <h3>Fone AirDots Pro </h3>
        <p class="preco">R$ 40,00</p>
        <a href="https://wa.me/5592986319253?text=Olá,%20quero%20comprar%20o%20Fone%20Bluetooth%20da%20Porto%20Cel" target="_blank">
            <button>Comprar</button>
        </a>
    </div>
</section>

<h2>🔌 Carregadores</h2>
<section class="produtos">
    <div class="card">
        <img src="caboiphone.png">
        <h3>Cabo USB-Iphone</h3>
        <p class="preco">R$ 15,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="caboiphone.png">
        <h3>Cabo USB-C</h3>
        <p class="preco">R$ 15,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="caboct.png">
        <h3>Carregador completo Iphone</h3>
        <p class="preco">R$ 35,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="caboct.png">
        <h3>Carregador completo TIPO-C</h3>
        <p class="preco">R$ 35,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="adadad.png"
        ">
        <h3>Carregador Veicular</h3>
        <p class="preco">R$ 20,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
</section>

<h2>📱 Capinhas</h2>
<section class="produtos">
    <div class="card">
        <img src="https://via.placeholder.com/200">
        <h3>Capinha Verde escura iphone 12</h3>
        <p class="preco">R$ 25,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="https://via.placeholder.com/200">
        <h3>Capinha Vermelha Iphone 12</h3>
        <p class="preco">R$ 25,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="https://via.placeholder.com/200">
        <h3>Capinha Amarela Iphone 12</h3>
        <p class="preco">R$ 25,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="https://via.placeholder.com/200">
        <h3>Capinha Lilás Iphone 12</h3>
        <p class="preco">R$ 25,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
</section>

<h2>🦾 Acessórios</h2>
<section class="produtos">
    <div class="card">
        <img src="rosa.jpeg">
        <h3>Ventosa rosa</h3>
        <p class="preco">R$ 20,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="pink.jpeg">
        <h3>Ventosa Rosa pink</h3>
        <p class="preco">R$ 20,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="azul.jpeg">
        <h3>Ventosa Azul escuro</h3>
        <p class="preco">R$ 20,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="bebe.jpeg">
        <h3>Ventosa Azul bebê</h3>
        <p class="preco">R$ 20,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
    <div class="card">
        <img src="stanley.jpeg">
        <h3>Copo Stanley 520ml</h3>
        <p class="preco">R$ 35,00</p>
        <a href="https://wa.me/5592986319253" target="_blank"><button>Comprar</button></a>
    </div>
</section>

<!-- Localização -->
<section class="localizacao">
    <h2>📍 Onde Estamos</h2>
    <p>Porto de Manaus - AM</p>
    <p>🕒 Segunda a Sábado: 8h às 18h</p>
    <p>📱 +55 92 98631-9253</p>
</section>

<a class="whatsapp-fixo" href="https://wa.me/5592986319253" target="_blank">
💬 Fale Conosco
</a>

<script>
// Mostrar cards com animação
const cards = document.querySelectorAll('.card');

function mostrarCards() {
    const trigger = window.innerHeight * 0.85;
    cards.forEach(card => {
        const top = card.getBoundingClientRect().top;
        if (top < trigger) {
            card.classList.add('show');
        }
    });
}

window.addEventListener('scroll', mostrarCards);
window.addEventListener('load', mostrarCards);

// Garantir que todos os cards novos fiquem visíveis ao carregar
cards.forEach(card => card.classList.add('show'));
</script>

</div> <!-- fim content -->
</body>
</html>
