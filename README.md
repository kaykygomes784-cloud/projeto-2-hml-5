# projeto-2-hml-5
index.html

<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Organização</title>
  <link rel="stylesheet" href="styles/style.css">
</head>
<body>
  <header>
    <nav class="nav-menu">
      <ul>
        <li><a href="index.html">Início</a></li>
        <li><a href="projetos.html">Projetos Sociais</a></li>
        <li><a href="cadastro.html">Cadastro</a></li>
      </ul>
      <button class="menu-hamburguer">
        <span></span>
        <span></span>
        <span></span>
      </button>
    </nav>
  </header>
  <main>
    <h1>Organização</h1>
    <p>Bem-vindo à nossa organização!</p>
    <address>
      Contato: <a href="mailto:contato@organizacao.com">contato@organizacao.com</a>
    </address>
    <img src="imagens/logo.png" alt="Logo da Organização">
  </main>
  <footer>
    <p>&copy; 2023 Organização</p>
  </footer>
  <script src="scripts/script.js"></script>
</body>
</html>


projetos.html

<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Projetos Sociais</title>
  <link rel="stylesheet" href="styles/style.css">
</head>
<body>
  <header>
    <nav class="nav-menu">
      <ul>
        <li><a href="index.html">Início</a></li>
        <li><a href="projetos.html">Projetos Sociais</a></li>
        <li><a href="cadastro.html">Cadastro</a></li>
      </ul>
      <button class="menu-hamburguer">
        <span></span>
        <span></span>
        <span></span>
      </button>
    </nav>
  </header>
  <main>
    <h1>Projetos Sociais</h1>
    <p>Conheça nossos projetos sociais!</p>
    <section class="grid-container">
      <div class="card">
        <h2>Voluntariado</h2>
        <p>Participe do nosso voluntariado!</p>
        <img src="imagens/voluntariado.jpg" alt="Voluntariado">
      </div>
      <div class="card">
        <h2>Doação</h2>
        <p>Faça uma doação para nossa causa!</p>
        <img src="imagens/doacao.jpg" alt="Doação">
      </div>
    </section>
  </main>
  <footer>
    <p>&copy; 2023 Organização</p>
  </footer>
  <script src="scripts/script.js"></script>
</body>
</html>


cadastro.html

<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cadastro</title>
  <link rel="stylesheet" href="styles/style.css">
</head>
<body>
  <header>
    <nav class="nav-menu">
      <ul>
        <li><a href="index.html">Início</a></li>
        <li><a href="projetos.html">Projetos Sociais</a></li>
        <li><a href="cadastro.html">Cadastro</a></li>
      </ul>
      <button class="menu-hamburguer">
        <span></span>
        <span></span>
        <span></span>
      </button>
    </nav>
  </header>
  <main>
    <h1>Cadastro</h1>
    <form>
      <fieldset>
        <legend>Informações Pessoais</legend>
        <label for="nome">Nome Completo:</label>
        <input type="text" id="nome" name="nome" required>
        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required>
        <label for="cpf">CPF:</label>
        <input type="text" id="cpf" name="cpf" pattern="\d{3}\.\d{3}\.\d{3}-\d{2}" required>
        <label for="telefone">Telefone:</label>
        <input type="tel" id="telefone" name="telefone" pattern="\(\d{2}\) \d{4,5}-\d{4}" required>
        <label for="nascimento">Data de Nascimento:</label>
        <input type="date" id="nascimento" name="nascimento" required>
      </fieldset>
      <fieldset>
        <legend>Endereço</legend>
        <label for="endereco">Endereço:</label>
        <input type="text" id="endereco" name="endereco" required>
        <label for="cep">CEP:</label>
        <input type="text" id="cep" name="cep" pattern="\d{5}-\d{3}" required>
        <label for="cidade">Cidade:</label>
        <input type="text" id="cidade" name="cidade" required>
        <label for="estado">Estado:</label>
        <select id="estado" name="estado" required>
          <option value="">Selecione</option>
          <option value="AC">Acre</option>
          <option value="AL">Alagoas</option>
          <!-- Adicione mais opções aqui -->
        </select>
      </fieldset>
      <button type="submit">Cadastrar</button>
    </form>
  </main>
  <footer>
    <p>&copy; 2023 Organização</p>
  </footer>
  <script src="scripts/script.js"></script>
</body>
</html>


styles/style.css

:root {
  --cor-primaria: #3498db;
  --cor-secundaria: #f1c40f;
  --cor-neutra: #f9f9f9;
  --cor-acinzentada: #ccc;
  --cor-escura: #333;
  --tamanho-fonte-titulo: 36px;
  --tamanho-fonte-texto: 18px;
  --espacamento-xs: 8px;
  --espacamento-sm: 16px;
  --espacamento-md: 24px;
  --espacamento-lg: 32px;
  --espacamento-xl: 48px;
  --espacamento-xxl: 64px;
}

.grid-container {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: var(--espacamento-sm);
}

.card {
  background-color: #fff;
  border: 1px solid var(--cor-acinzentada);
  padding: var(--espacamento-md);
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.button {
  background-color: var(--cor-primaria);
  color: #fff;
  padding: var(--espacamento-sm) var(--espacamento-md);
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.button:hover {
  background-color: var(--cor-secundaria);
}

.nav-menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: var(--espacamento-sm);
  background-color: var(--cor-primaria);
  color: #fff;
}

.nav-menu ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}

.nav-menu li {
  margin-right: var(--espacamento-sm);
}

.nav-menu a {
  color: #fff;
  text-decoration: none;
}

.menu-hamburguer {
  display: none;
}

@media (max-width: 768px) {
  .nav-menu ul {
    display: none;
  }
  .menu-hamburguer {
    display: block;
  }
  .nav-menu.active ul {
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    background-color: var(--cor-primaria);
    padding: var(--espacamento-sm);
  }
}


scripts/script.js

document.querySelector('.menu-hamburguer').addEventListener('click', () => {
  document.querySelector('.nav-menu').classList.toggle('active');
});
