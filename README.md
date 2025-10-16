# Site-de-cosm-tico
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beleza Pura | Cosméticos Naturais</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <header class="cabecalho">
        <h1>Beleza Pura</h1>
        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Skincare</a></li>
                <li><a href="#">Maquiagem</a></li>
                <li><a href="#">Promoções</a></li>
                <li><a href="#">Meu Carrinho (0)</a></li>
            </ul>
        </nav>
    </header>

    <main class="conteudo-principal">
        <section class="banner">
            <h2>Cosméticos Naturais e Veganos</h2>
            <p>Descubra o poder da natureza para a sua pele. Frete grátis na primeira compra!</p>
        </section>

        <section class="vitrine">
            <h2>Nossos Mais Vendidos</h2>
            <div class="lista-produtos">

                <div class="produto">
                    <img src="serum_facial.jpg" alt="Sérum Facial Hidratante de Ácido Hialurônico">
                    <h3>Sérum Renovador</h3>
                    <p class="categoria">Skincare</p>
                    <p class="preco">R$ 120,00</p>
                    <p class="descricao">Hidratação profunda com Ácido Hialurônico e Vitamina C.</p>
                    <button class="botao-comprar">Adicionar à Sacola</button>
                </div>

                <div class="produto">
                    <img src="mascara_capilar.jpg" alt="Máscara Capilar de Manteiga de Karité">
                    <h3>Máscara Nutritiva</h3>
                    <p class="categoria">Cabelos</p>
                    <p class="preco">R$ 85,00</p>
                    <p class="descricao">Restaura e dá brilho aos fios secos e danificados.</p>
                    <button class="botao-comprar">Adicionar à Sacola</button>
                </div>

                <div class="produto">
                    <img src="batom_liquido.jpg" alt="Batom Líquido Matte na cor Nude">
                    <h3>Batom Matte Longa Duração</h3>
                    <p class="categoria">Maquiagem</p>
                    <p class="preco">R$ 45,00</p>
                    <p class="descricao">Cor intensa com acabamento aveludado que não resseca.</p>
                    <button class="botao-comprar">Adicionar à Sacola</button>
                </div>

            </div>
        </section>
    </main>

    <footer class="rodape">
        <p>&copy; 2025 Beleza Pura Cosméticos. | Design Estático (Apenas HTML/CSS).</p>
        <div class="contato-info">
            <p>Siga-nos: Instagram | Facebook</p>
        </div>
    </footer>

</body>
</html>
/* Paleta de Cores: Suave e Feminina */
:root {
    --cor-primaria: #ff69b4; /* Pink (Rosa Choque) */
    --cor-secundaria: #f8c0e0; /* Rosa Claro */
    --cor-fundo: #fffafa; /* Branco Gelo */
    --cor-texto: #444;
    --cor-destaque-preco: #008080; /* Teal (Verde Azulado) */
}

/* Reset Básico */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Georgia', serif;
}

body {
    background-color: var(--cor-fundo);
    color: var(--cor-texto);
    line-height: 1.6;
}

/* Cabeçalho */
.cabecalho {
    background: var(--cor-primaria);
    color: #fff;
    padding: 15px 30px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.cabecalho h1 {
    font-size: 2em;
    font-family: 'Times New Roman', serif;
}

.cabecalho nav ul {
    list-style: none;
    display: flex;
}

.cabecalho nav ul li {
    margin-left: 25px;
}

.cabecalho nav ul li a {
    color: #fff;
    text-decoration: none;
    padding: 8px 12px;
    border-radius: 5px;
    transition: background-color 0.3s;
}

.cabecalho nav ul li a:hover {
    background-color: var(--cor-secundaria);
    color: var(--cor-primaria);
}

/* Conteúdo Principal */
.conteudo-principal {
    padding: 30px 20px;
    max-width: 1200px;
    margin: 0 auto;
}

/* Banner de Promoção */
.banner {
    background-color: var(--cor-secundaria);
    color: var(--cor-texto);
    padding: 50px;
    text-align: center;
    margin-bottom: 40px;
    border-radius: 10px;
    border: 1px solid var(--cor-primaria);
}

.banner h2 {
    margin-bottom: 10px;
    font-size: 2.2em;
    color: var(--cor-primaria);
}

/* Vitrine de Produtos */
.vitrine h2 {
    text-align: center;
    margin-bottom: 35px;
    color: var(--cor-primaria);
    font-size: 1.8em;
}

.lista-produtos {
    display: grid;
    /* 3 colunas em telas maiores, ou ajuste automaticamente */
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
}

.produto {
    background-color: #fff;
    border: 1px solid #eee;
    padding: 20px;
    text-align: center;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    transition: box-shadow 0.3s, transform 0.3s;
}

.produto:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.1);
}

.produto img {
    width: 100%;
    max-height: 250px;
    object-fit: contain; /* Para cosméticos, melhor `contain` para ver o frasco inteiro */
    border-radius: 8px;
    margin-bottom: 15px;
}

.produto h3 {
    margin-bottom: 5px;
    color: var(--cor-primaria);
    font-size: 1.3em;
}

.produto .categoria {
    font-size: 0.85em;
    color: #888;
    margin-bottom: 10px;
}

.produto .preco {
    font-size: 1.6em;
    color: var(--cor-destaque-preco);
    font-weight: bold;
    margin-bottom: 15px;
}

.produto .descricao {
    margin-bottom: 20px;
    font-size: 0.9em;
    color: #666;
    height: 40px; /* Garante altura uniforme */
    overflow: hidden;
}

.botao-comprar {
    background-color: var(--cor-primaria);
    color: #fff;
    border: none;
    padding: 12px 25px;
    border-radius: 50px; /* Botão arredondado */
    cursor: pointer;
    font-size: 1em;
    font-weight: bold;
    letter-spacing: 0.5px;
    transition: opacity 0.3s, background-color 0.3s;
}

.botao-comprar:hover {
    background-color: #ff3399; /* Um rosa mais escuro no hover */
}

/* Rodapé */
.rodape {
    background: var(--cor-primaria);
    color: #fff;
    text-align: center;
    padding: 25px;
    margin-top: 40px;
    font-size: 0.9em;
}

.rodape .contato-info {
    margin-top: 10px;
}