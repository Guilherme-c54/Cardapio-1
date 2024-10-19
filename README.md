<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cardápio</title> <!-- Título alterado para "Cardápio" -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            background: linear-gradient(135deg, #1e1e1e, #4a4a4a); /* Gradiente de fundo */
            color: white; /* Cor do texto */
            font-family: 'Poppins', sans-serif; /* Fonte padrão */
            margin: 0; /* Remove a margem padrão do body */
            padding: 40px 20px; /* Aumenta o padding superior para evitar cortes */
            display: flex; /* Usar flexbox para centralizar o conteúdo */
            justify-content: center; /* Centraliza horizontalmente */
            align-items: flex-start; /* Alinha ao topo da tela */
            min-height: 100vh; /* Garante que a altura mínima seja a altura total da viewport */
        }

        .menu-container {
            max-width: 800px; /* Largura máxima do container do menu */
            background-color: rgba(255, 255, 255, 0.1); /* Fundo semi-transparente para o cardápio */
            border-radius: 10px; /* Arredondar bordas */
            padding: 20px; /* Adiciona espaçamento interno ao cardápio */
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5); /* Sombra ao redor do cardápio */
        }

        h1 {
            text-align: center; /* Centraliza o título */
            font-family: 'Playfair Display', serif; /* Fonte do título */
            margin-bottom: 20px; /* Espaçamento inferior do título */
            font-size: 2.5em; /* Tamanho da fonte do título */
        }

        .menu-section {
            margin-bottom: 30px; /* Espaço entre as seções do menu */
            border: 1px solid white; /* Borda branca ao redor das seções */
            padding: 15px; /* Espaçamento interno nas seções */
            border-radius: 8px; /* Arredonda as bordas das seções */
            transition: transform 0.3s; /* Transição suave para hover */
        }

        .menu-section:hover {
            transform: scale(1.02); /* Leve aumento ao passar o mouse */
        }

        .menu-header {
            border-bottom: 1px solid white; /* Linha inferior ao cabeçalho da seção */
            padding-bottom: 10px; /* Espaçamento inferior do cabeçalho */
        }

        .menu-title {
            margin: 0; /* Remove a margem do título */
        }

        .menu-items {
            list-style: none; /* Remove os marcadores da lista */
            padding: 0; /* Remove o padding padrão da lista */
        }

        .menu-items li {
            display: flex; /* Usa flexbox para alinhar os itens */
            justify-content: space-between; /* Distribui os itens */
            margin-bottom: 8px; /* Espaçamento entre os itens */
            padding: 5px; /* Adiciona espaçamento interno */
            border-radius: 5px; /* Arredonda as bordas dos itens */
            transition: background-color 0.3s; /* Transição suave para hover */
        }

        .menu-items li:hover {
            background-color: rgba(255, 255, 255, 0.2); /* Efeito de hover nos itens */
        }

        .menu-time {
            font-weight: 600; /* Peso da fonte negrito */
        }

        @media (max-width: 600px) {
            h1 {
                font-size: 2em; /* Reduz o tamanho do título em telas pequenas */
            }
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <header>
            <h1>Cardápio</h1> <!-- Título do cardápio -->
        </header>

        <!-- Primeira seção: Comidas 13h às 15h -->
        <section class="menu-section" aria-label="Comidas das 13h às 15h">
            <div class="menu-header">
                <p class="menu-time">13h às 15h</p>
                <h2 class="menu-title">Comidas</h2>
            </div>
            <ul class="menu-items">
                <li>Risoto de Cogumelos <span>R$42,00</span></li>
                <li>Filé Mignon ao Molho <span>R$55,00</span></li>
                <li>Salada Caesar <span>R$30,00</span></li>
                <li>Linguine ao Pesto <span>R$38,00</span></li>
                <li>Frango Grelhado <span>R$34,00</span></li>
            </ul>
        </section>

        <!-- Segunda seção: Comidas 15h às 17h -->
        <section class="menu-section" aria-label="Comidas das 15h às 17h">
            <div class="menu-header">
                <p class="menu-time">15h às 17h</p>
                <h2 class="menu-title">Comidas</h2>
            </div>
            <ul class="menu-items">
                <li>Camarão Empanado <span>R$68,00</span></li>
                <li>Steak ao Poivre <span>R$75,00</span></li>
                <li>Bacalhau à Brás <span>R$60,00</span></li>
                <li>Peixe Grelhado <span>R$65,00</span></li>
                <li>Carpaccio de Carne <span>R$48,00</span></li>
                <li>Costelinha BBQ <span>R$50,00</span></li>
                <li>Ravioli de Queijo <span>R$42,00</span></li>
                <li>Sopa de Tomate <span>R$28,00</span></li>
                <li>Gnocchi de Batata <span>R$38,00</span></li>
                <li>Quiche Lorraine <span>R$30,00</span></li>
            </ul>
        </section>

        <!-- Terceira seção: Bebidas e Gelados -->
        <section class="menu-section">
            <div class="menu-header">
                <h2 class="menu-title">Bebidas e Gelados</h2>
            </div>
            <ul class="menu-items">
                <li>Suco de Laranja Natural <span>R$12,00</span></li>
                <li>Smoothie de Morango <span>R$18,00</span></li>
                <li>Café Espresso <span>R$8,00</span></li>
                <li>Mojito <span>R$22,00</span></li>
                <li>Sorvete Artesanal <span>R$15,00</span></li>
            </ul>
        </section>
    </div>
</body>
</html>
