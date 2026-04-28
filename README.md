<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Webflix & O Chefe | Entretenimento Ilimitado</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #e50914; /* Vermelho Estilo Netflix */
            --secondary: #25d366; /* Verde WhatsApp */
            --dark: #000000;
            --gray-dark: #141414;
            --white: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: var(--dark);
            color: var(--white);
            overflow-x: hidden;
        }

        /* --- CABEÇALHO --- */
        header {
            display: flex;
            justify-content: space-between;
            padding: 20px 5%;
            align-items: center;
            background: linear-gradient(to bottom, rgba(0,0,0,0.9), transparent);
            position: fixed;
            width: 100%;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
            text-transform: uppercase;
        }

        /* --- HERO SECTION --- */
        .hero {
            height: 90vh;
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.9)), url('https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: clamp(2rem, 5vw, 4rem);
            margin-bottom: 20px;
            max-width: 900px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            color: #ccc;
        }

        .btn-main {
            background-color: var(--primary);
            color: white;
            padding: 15px 40px;
            text-decoration: none;
            font-weight: 700;
            border-radius: 5px;
            transition: 0.3s;
            font-size: 1.1rem;
        }

        .btn-main:hover {
            transform: scale(1.05);
            background-color: #f40612;
        }

        /* --- RECURSOS --- */
        .features {
            padding: 80px 5%;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            background-color: var(--dark);
        }

        .card {
            background: var(--gray-dark);
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            border-bottom: 3px solid var(--primary);
        }

        .card h3 { margin-bottom: 15px; color: var(--primary); }

        /* --- PLANOS --- */
        .pricing {
            padding: 80px 5%;
            text-align: center;
        }

        .grid-plans {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .plan-card {
            background: var(--gray-dark);
            padding: 40px 20px;
            border-radius: 15px;
            position: relative;
            transition: 0.3s;
        }

        .plan-card.highlight {
            border: 2px solid var(--primary);
            transform: scale(1.05);
        }

        .price {
            font-size: 2.5rem;
            font-weight: 700;
            margin: 20px 0;
            display: block;
        }

        .plan-card ul {
            list-style: none;
            margin-bottom: 30px;
            color: #aaa;
        }

        .plan-card ul li { margin: 10px 0; }

        .btn-plan {
            background-color: var(--white);
            color: var(--dark);
            padding: 12px 0;
            display: block;
            text-decoration: none;
            font-weight: 700;
            border-radius: 5px;
        }

        .highlight .btn-plan {
            background-color: var(--primary);
            color: white;
        }

        /* --- WHATSAPP FIXO --- */
        .whatsapp-float {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: var(--secondary);
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.5);
            z-index: 1000;
            text-decoration: none;
            font-size: 30px;
        }

        footer {
            padding: 40px;
            text-align: center;
            border-top: 1px solid #333;
            color: #777;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">WEBFLIX & O CHEFE</div>
    </header>

    <section class="hero">
        <h1>Filmes, Séries e Canais sem Limites.</h1>
        <p>A maior estabilidade do mercado com o melhor conteúdo 4K.</p>
        <a href="https://wa.me/5584999999999?text=Quero+um+teste+gratis" class="btn-main">SOLICITAR TESTE GRÁTIS</a>
    </section>

    <section class="features">
        <div class="card">
            <h3>+60.000 Conteúdos</h3>
            <p>O maior catálogo de filmes e séries atualizado diariamente.</p>
        </div>
        <div class="card">
            <h3>Servidor Premium</h3>
            <p>Tecnologia anti-travamento para você ver futebol sem stress.</p>
        </div>
        <div class="card">
            <h3>Multi-Dispositivos</h3>
            <p>Assista na Smart TV, Celular, TV Box, Tablet ou Computador.</p>
        </div>
    </section>

    <section class="pricing">
        <h2>Escolha o seu Plano</h2>
        <div class="grid-plans">
            <div class="plan-card">
                <h3>MENSAL</h3>
                <span class="price">R$ 25,00</span>
                <ul>
                    <li>1 Tela</li>
                    <li>Canais, Filmes e Séries</li>
                    <li>Qualidade SD/HD/FHD/4K</li>
                </ul>
                <a href="https://wa.me/5584999999999?text=Quero+o+plano+Mensal" class="btn-plan">CONTRATAR</a>
            </div>

            <div class="plan-card highlight">
                <span style="position:absolute; top:-15px; left:50%; transform:translateX(-50%); background:var(--primary); padding:5px 15px; border-radius:20px; font-size:0.8rem;">MAIS VENDIDO</span>
                <h3>TRIMESTRAL</h3>
                <span class="price">R$ 49,90</span>
                <ul>
                    <li>1 Tela (Preço Promocional)</li>
                    <li>Todo Catálogo Liberado</li>
                    <li>Suporte Prioritário</li>
                </ul>
                <a href="https://wa.me/5584999999999?text=Quero+o+plano+Trimestral" class="btn-plan">CONTRATAR</a>
            </div>

            <div class="plan-card">
                <h3>MASTER</h3>
                <span class="price">R$ 70,00</span>
                <ul>
                    <li>3 Telas Simultâneas</li>
                    <li>Acesso VIP</li>
                    <li>Ideal para Família</li>
                </ul>
                <a href="https://wa.me/5584999999999?text=Quero+o+plano+Master" class="btn-plan">CONTRATAR</a>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Webflix & O Chefe. Todos os direitos reservados.</p>
    </footer>

    <a href="https://wa.me/5584999999999?text=Ol%C3%A1%21+Vim+pelo+site+e+quero+um+teste." class="whatsapp-float" target="_blank">
        <span style="font-family: Arial;">WP</span>
    </a>

</body>
</html>
