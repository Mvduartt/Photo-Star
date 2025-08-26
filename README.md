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
      background-color: #f7f8fa;
      color: #333;
      line-height: 1.6;
    }

    header {
      background: linear-gradient(135deg, #111, #444);
      color: #fff;
      padding: 25px 15px;
      text-align: center;
      animation: fadeInDown 0.8s ease;
    }

    header h1 {
      font-size: 2rem;
      font-weight: 700;
    }

    nav ul {
      display: flex;
      justify-content: center;
      gap: 25px;
      list-style: none;
      margin-top: 15px;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 500;
      font-size: 1rem;
      transition: color 0.3s, transform 0.2s;
    }

    nav a:hover {
      color: #ff0000;
      transform: translateY(-2px);
    }

    main {
      max-width: 650px;
      margin: 50px auto;
      background: #fff;
      padding: 40px 30px;
      border-radius: 15px;
      box-shadow: 0 6px 25px rgba(0,0,0,0.08);
      animation: fadeIn 1s ease;
    }

    h2 {
      text-align: center;
      margin-bottom: 25px;
      color: #222;
      font-size: 1.8rem;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 18px;
    }

    input, textarea, select {
      padding: 14px;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 1rem;
      transition: border-color 0.3s, box-shadow 0.3s;
    }

    input:focus, textarea:focus, select:focus {
      border-color: #ff0505;
      box-shadow: 0 0 8px rgba(255, 203, 5, 0.4);
      outline: none;
    }

    button {
      padding: 14px;
      border: none;
      background: linear-gradient(135deg, #ff0505, #f31212);
      color: white;
      font-size: 1.1rem;
      font-weight: 600;
      border-radius: 8px;
      cursor: pointer;
      transition: transform 0.2s, box-shadow 0.3s;
    }

    button:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 15px rgba(0,0,0,0.15);
    }

    footer {
      background: #111;
      color: #fff;
      text-align: center;
      padding: 20px;
      margin-top: 50px;
      font-size: 0.9rem;
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
