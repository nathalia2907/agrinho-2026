<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro Forte, Futuro Sustentável - Agrinho 2026</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>

    <header class="main-header">
        <div class="container header-container">
            <div class="logo">Agrinho<span>2026</span></div>
            <nav class="main-nav">
                <ul>
                    <li><a href="#inicio" class="active">Início</a></li>
                    <li><a href="#sobre">O Projeto</a></li>
                    <li><a href="#sustentabilidade">Sustentabilidade</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="inicio" class="hero-section">
        <div class="container hero-content">
            <h1>Agro Forte, Futuro Sustentável</h1>
            <p>Conectando a força do campo à preservação do amanhã.</p>
            <a href="#sobre" class="btn-primary">Saiba Mais</a>
        </div>
    </section>

    <section id="sobre" class="content-section">
        <div class="container">
            
            <div class="info-row">
                <div class="info-text">
                    <h2>A Força do Agro e o Compromisso com o Amanhã</h2>
                    <p>O Agrinho 2026 traz como pilar central a união entre a alta produtividade do campo e a conservação ambiental. Ser um "Agro Forte" hoje significa adotar práticas agrícolas inteligentes, que protegem o solo, otimizam o uso da água e reduzem as emissões de carbono, garantindo alimento e qualidade de vida para as próximas gerações.</p>
                </div>
                <div class="info-image">
                    <img src="https://images.unsplash.com/photo-1628085449712-4217346fa013?auto=format&fit=crop&q=80&w=800" alt="Araucária imponente na paisagem do campo">
                </div>
            </div>

            <div class="info-row reverse">
                <div class="info-text">
                    <h2>A Araucária como Símbolo de Resiliência</h2>
                    <p>Assim como a Araucária (<i>Araucaria angustifolia</i>) ergue suas copas imponentes rumo ao céu, sustentada por raízes profundas e fortes, o desenvolvimento sustentável do ecossistema agrícola precisa ser sólido e duradouro. Preservar as espécies nativas e integrar a biodiversidade ao manejo agrícola é a chave para um futuro equilibrado.</p>
                </div>
                <div class="info-image">
                    <img src="https://images.unsplash.com/photo-1502082553048-f009c37129b9?auto=format&fit=crop&q=80&w=800" alt="Detalhe das folhas e galhos da Araucária">
                </div>
            </div>

        </div>
    </section>

    <footer class="main-footer">
        <div class="container">
            <p>&copy; 2026 Agrinho - Agro Forte, Futuro Sustentável. Todos os direitos reservados.</p>
        </div>
    </footer>

</body>
</html># 
/* ==========================================================================
   Variáveis de Cores (Paleta solicitada: Verde claro amarelado e Marrom claro)
   ========================================================================== */
:root {
    --primary-green: #a3b86c;       /* Verde claro com tom levemente amarelado */
    --light-green-bg: #f4f7ee;     /* Fundo verde bem suave */
    --accent-brown: #8e7355;       /* Marrom claro */
    --dark-brown: #4a3b2c;         /* Marrom escuro para textos principais */
    --white: #ffffff;
    --transition: all 0.3s ease;
}

/* ==========================================================================
   Resets e Estilos Globais
   ========================================================================== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Montserrat', sans-serif;
    background-color: var(--white);
    color: var(--dark-brown);
    line-height: 1.6;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
}

img {
    max-width: 100%;
    height: auto;
    display: block;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
}

/* ==========================================================================
   Cabeçalho
   ========================================================================== */
.main-header {
    background-color: var(--white);
    border-bottom: 3px solid var(--primary-green);
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
}

.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}

.logo {
    font-size: 24px;
    font-weight: 700;
    color: var(--dark-brown);
}

.logo span {
    color: var(--primary-green);
}

.main-nav ul {
    display: flex;
    list-style: none;
    gap: 20px;
}

.main-nav a {
    text-decoration: none;
    color: var(--dark-brown);
    font-weight: 600;
    font-size: 15px;
    transition: var(--transition);
}

.main-nav a:hover, 
.main-nav a.active {
    color: var(--accent-brown);
}

/* ==========================================================================
   Seção Hero (Banner Principal)
   ========================================================================== */
.hero-section {
    background: linear-gradient(rgba(74, 59, 44, 0.6), rgba(74, 59, 44, 0.4)), 
                url('https://images.unsplash.com/photo-1500382017468-9049fed747ef?auto=format&fit=crop&q=80&w=1600') no-repeat center center/cover;
    height: 60vh;
    display: flex;
    align-items: center;
    text-align: center;
    color: var(--white);
}

.hero-content h1 {
    font-size: 42px;
    font-weight: 700;
    margin-bottom: 15px;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
}

.hero-content p {
    font-size: 18px;
    margin-bottom: 25px;
    text-shadow: 1px 1px 3px rgba(0,0,0,0.5);
}

.btn-primary {
    display: inline-block;
    background-color: var(--primary-green);
    color: var(--dark-brown);
    padding: 12px 30px;
    text-decoration: none;
    font-weight: 600;
    border-radius: 25px;
    transition: var(--transition);
}

.btn-primary:hover {
    background-color: var(--accent-brown);
    color: var(--white);
    transform: translateY(-2px);
}

/* ==========================================================================
   Seção de Conteúdo (Layout Intercalado)
   ========================================================================== */
.content-section {
    padding: 80px 0;
    background-color: var(--light-green-bg);
}

.info-row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 50px;
    margin-bottom: 80px;
}

/* Inverte a ordem dos fatores no segundo bloco (Imagem na esquerda) */
.info-row.reverse {
    flex-direction: row-reverse;
}

.info-row:last-child {
    margin-bottom: 0;
}

.info-text {
    flex: 1;
}

.info-text h2 {
    font-size: 28px;
    color: var(--dark-brown);
    margin-bottom: 20px;
    position: relative;
}

/* Detalhe estético marrom abaixo dos títulos */
.info-text h2::after {
    content: '';
    display: block;
    width: 60px;
    height: 4px;
    background-color: var(--accent-brown);
    margin-top: 10px;
    border-radius: 2px;
}

.info-text p {
    font-size: 16px;
    color: #5a4b3c;
    text-align: justify;
}

.info-image {
    flex: 1;
}

/* ==========================================================================
   Rodapé
   ========================================================================== */
.main-footer {
    background-color: var(--dark-brown);
    color: var(--white);
    text-align: center;
    padding: 30px 0;
    font-size: 14px;
    border-top: 4px solid var(--accent-brown);
}

/* ==========================================================================
   Responsividade (Mobile First/Adaptável)
   ========================================================================== */
@media (max-width: 768px) {
    .header-container {
        flex-direction: column;
        gap: 15px;
    }

    .hero-content h1 {
        font-size: 32px;
    }

    .info-row, .info-row.reverse {
        flex-direction: column;
        gap: 30px;
        margin-bottom: 50px;
    }
    
    .info-text h2 {
        font-size: 24px;
    }
}
