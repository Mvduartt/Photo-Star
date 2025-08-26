<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Photo Star - Sobre</title>
  <style>
    /* Reset básico */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      color: #333;
      line-height: 1.6;
    }

    header {
      background-color: #222;
      color: #fff;
      padding: 20px;
    }

    header h1 {
      font-size: 2rem;
      margin-bottom: 10px;
      text-align: center;
    }

    nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      gap: 20px;
      flex-wrap: wrap;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      padding: 8px 15px;
      border-radius: 5px;
      transition: background 0.3s;
    }

    nav a:hover {
      background-color: #444;
    }

    main {
      padding: 40px 20px;
      max-width: 900px;
      margin: 0 auto;
      text-align: center;
    }

    main img {
      max-width: 100%;
      height: auto;
      margin-top: 20px;
      border-radius: 10px;
    }

    footer {
      background-color: #222;
      color: #fff;
      text-align: center;
      padding: 15px;
      margin-top: 40px;
    }

    /* Botão flutuante */
    .badge-bottom-right {
      position: fixed;
      right: 12px;
      bottom: 16px;
      width: 45px;
      height: auto;
      z-index: 1000;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <header>
    <h1>Photo Star</h1>
    <nav>
      <ul>
        <li><a href="index.html">Informações</a></li>
        <li><a href="sobre.html">Sobre</a></li>
        <li><a href="contato.html">Contato</a></li>
        <li><a href="agendamento.html">Agendamento</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <h2>Sobre Nós</h2>
    <p>Agende um fotógrafo para eventos especiais como aniversários, casamentos, reuniões familiares e muito mais. Capturamos momentos únicos com profissionalismo e criatividade.</p>
    
    <img src="https://ichef.bbci.co.uk/ace/standard/1024/cpsprodpb/2C16/production/_90168211_neymar_getty.jpg" alt="Foto de exemplo" />
    
    <h2>Melhores Fotos</h2>
    <img src="https://i.pinimg.com/750x/99/5d/d0/995dd0b340d2c16f21d53d7de6b93711.jpg" alt="Exemplo de foto profissional" />
  </main>

  <footer>
    <p>&copy; 2025 Photo Star. Todos os direitos reservados.</p>
  </footer>

  <!-- Imagem flutuante -->
  <img class="badge-bottom-right" src="https://i.imgur.com/Qn6XUHN.png" alt="Ícone" />
</body>
</html>
