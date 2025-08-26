<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Agendamento | Photo Star</title>

  <!-- Google Fonts: Poppins -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    /* Reset e fonte base */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background-color: #f0f2f5;
      color: #333;
    }

    header {
      background-color: #222;
      color: #fff;
      padding: 20px;
      text-align: center;
      animation: fadeInDown 0.8s ease;
    }

    nav ul {
      display: flex;
      justify-content: center;
      gap: 20px;
      list-style: none;
      margin-top: 10px;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #ccc;
    }

    main {
      max-width: 600px;
      margin: 40px auto;
      background: #fff;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.05);
      animation: fadeIn 1s ease;
    }

    h2 {
      text-align: center;
      margin-bottom: 20px;
      color: #222;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    input, textarea, select {
      padding: 12px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 1rem;
    }

    button {
      padding: 12px;
      border: none;
      background-color: #222;
      color: white;
      font-size: 1rem;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #444;
    }

    footer {
      background-color: #222;
      color: #fff;
      text-align: center;
      padding: 15px;
      margin-top: 40px;
    }

    /* Animações */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
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
    <h2>Agende sua Sessão</h2>
    <form action="https://formsubmit.co/seu-email@email.com" method="POST">
      <input type="text" name="nome" placeholder="Seu nome completo" required />
      <input type="email" name="email" placeholder="Seu e-mail" required />
      <input type="tel" name="telefone" placeholder="Telefone para contato" required />
      
      <select name="tipo_evento" required>
        <option value="">Selecione o tipo de evento</option>
        <option value="Aniversário">Aniversário</option>
        <option value="Casamento">Casamento</option>
        <option value="Sessão Fotográfica">Sessão Fotográfica</option>
        <option value="Outro">Outro</option>
      </select>

      <textarea name="mensagem" rows="4" placeholder="Detalhes do evento (data, local, etc.)" required></textarea>

      <button type="submit">Enviar Agendamento</button>
    </form>
  </main>

  <footer>
    <p>&copy; 2025 Photo Star. Todos os direitos reservados.</p>
  </footer>

</body>
</html>
