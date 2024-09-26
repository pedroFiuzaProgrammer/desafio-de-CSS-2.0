<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clonando a Página do YouTube</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="header">
        <div class="logo">YouTube Clone</div>
        <div class="search-bar">
            <input type="text" placeholder="Pesquisar">
            <button>Buscar</button>
        </div>
    </header>
    
    <nav class="sidebar">
        <ul>
            <li>Início</li>
            <li>Em alta</li>
            <li>Inscrições</li>
            <li>Biblioteca</li>
            <li>Histórico</li>
            <li>Favoritos</li>
        </ul>
    </nav>
    
    <main class="main-content">
        <div class="video-card">
            <iframe src="https://embed.figma.com/design/nF24mVjne5MCGDoiwCN3H0/Untitled?node-id=0-1&embed-host=share" allowfullscreen></iframe>
            <div class="video-info">
                <h3>Título do Vídeo 1</h3>
                <p class="channel">Canal XYZ</p>
                <p class="description">Descrição do vídeo 1. Um resumo interessante sobre o conteúdo apresentado.</p>
                <div class="stats">
                    <span>1M visualizações</span> • <span>1 dia atrás</span>
                </div>
            </div>
        </div>

        <div class="video-card">
            <iframe src="https://embed.figma.com/design/nF24mVjne5MCGDoiwCN3H0/Untitled?node-id=0-1&embed-host=share" allowfullscreen></iframe>
            <div class="video-info">
                <h3>Título do Vídeo 2</h3>
                <p class="description">Descrição do vídeo 2. Um resumo interessante sobre o conteúdo apresentado.</p>
            </div>
        </div>

        <!-- Adicione mais vídeos conforme necessário -->
        
    </main>
    
    <footer class="footer">Rodapé do YouTube Clone</footer>
</body>
</html>

- styles.css

* {
    box-sizing: border-box; /* Para incluir padding e border na largura total */
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    display: flex;
    flex-direction: column;
    height: 100vh;
    background-color: #181818; /* Fundo escuro */
    color: #ffffff; /* Texto claro */
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #282828; /* Fundo do cabeçalho */
    padding: 10px 20px;
    border-bottom: 1px solid #444;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.search-bar {
    display: flex;
}

.search-bar input {
    padding: 5px;
    border: 1px solid #444;
    border-radius: 3px;
    background-color: #333; /* Fundo do input */
    color: #ffffff; /* Texto do input */
}

.search-bar button {
    padding: 5px 10px;
    margin-left: 5px;
    background-color: #cc0000;
    color: white;
    border: none;
    border-radius: 3px;
    cursor: pointer;
}

.sidebar {
    display: flex;
    flex-direction: column; /* Coloca os itens em coluna */
    width: 240px;
    background-color: #282828; /* Fundo da sidebar */
    padding: 20px;
    border-right: 1px solid #444;
}

.sidebar ul {
    list-style-type: none;
    padding: 0;
}

.sidebar li {
    padding: 10px 0;
    cursor: pointer;
    color: #ffffff; /* Texto da sidebar */
}

.sidebar li:hover {
    background-color: #444; /* Efeito hover */
}

.main-content {
    display: flex;
    flex-direction: column; /* Coloca os vídeos em coluna */
    flex-grow: 1; /* Para ocupar o espaço restante */
    padding: 20px;
    background-color: #181818; /* Fundo principal */
    align-items: center; /* Centraliza os itens horizontalmente */
}

.video-card {
    display: flex; /* Flexbox para alinhar iframe e informações */
    background-color: #222; /* Fundo dos cards */
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
    width: 100%;
    max-width: 800px; /* Limita a largura máxima */
    margin-bottom: 20px; /* Espaçamento entre os vídeos */
}

.video-card iframe {
    width: 320px; /* Largura fixa do iframe */
    height: 180px; /* Altura fixa do iframe */
    border: 1px solid rgba(0, 0, 0, 0.1);
    border-radius: 5px; /* Cantos arredondados */
}

.video-info {
    display: flex;
    flex-direction: column; /* Coloca as informações em coluna */
    margin-left: 15px; /* Espaçamento entre o iframe e as informações */
}

.video-info h3 {
    margin: 0 0 5px;
    font-size: 18px;
}

.channel {
    font-size: 14px;
    color: #cccccc; /* Canal em cinza claro */
    margin: 5px 0;
}

.description {
    font-size: 14px;
    color: #eeeeee; /* Descrição em cinza claro */
    margin: 5px 0;
}

.stats {
    font-size: 12px;
    color: #999; /* Estatísticas em cinza */
}

.footer {
    background-color: #282828;
    text-align: center;
    padding: 10px;
    border-top: 1px solid #444;
}

