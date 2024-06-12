
### Descrição dos Arquivos

- **index.html**: Página inicial que dá as boas-vindas aos usuários e contém diversos elementos para explorar as possibilidades da responsividade, incluindo um dashboard explicativo.
- **css/styles.css**: Arquivo de estilos CSS que aplica uma aparência moderna e responsiva ao site.
- **images/background.jpg**: Imagem de fundo utilizada na página.

## Explicação do Código

### index.html

- **Cabeçalho e Rodapé**: Utilizamos classes Bootstrap para estilização e classes personalizadas para cores e espaçamento.
- **Navegação**: Navbar responsiva que colapsa em dispositivos menores.
- **Conteúdo Principal**: Dividido em duas colunas utilizando o grid do Bootstrap. A coluna esquerda contém um card e uma tabela responsiva, enquanto a coluna direita contém um formulário.
- **Bootstrap**: Incluímos o CDN do Bootstrap para facilitar a criação de um layout responsivo.
- **JavaScript**: Importamos o jQuery, Popper.js e o script JavaScript do Bootstrap para funcionalidades interativas.

### styles.css

- **Estilos Customizados**: Adicionamos estilos adicionais para o cabeçalho, rodapé e conteúdo principal para melhorar a aparência e a responsividade da página.

## Conclusão

Este projeto é um exemplo prático de como criar uma página web responsiva utilizando HTML, CSS e Bootstrap. Estude o código, experimente fazer modificações e observe como cada mudança afeta a responsividade e a aparência da página. Isso ajudará a entender melhor como construir interfaces web modernas e funcionais.

## Recursos Adicionais

Para ajudar você a entender melhor o Bootstrap e o sistema de colunas, recomendo os seguintes recursos:

1. **Documentação Oficial do Bootstrap**:
   - O site oficial do Bootstrap oferece uma documentação completa e bem detalhada sobre como usar o framework. A seção sobre o sistema de grid é especialmente útil para entender o sistema de colunas.
   - [Documentação do Bootstrap](https://getbootstrap.com/docs/4.5/getting-started/introduction/)
   - [Sistema de Grid do Bootstrap](https://getbootstrap.com/docs/4.5/layout/grid/)

2. **W3Schools**:
   - W3Schools oferece tutoriais interativos e exemplos práticos sobre como usar o Bootstrap, incluindo uma seção dedicada ao sistema de grid.
   - [W3Schools Bootstrap Grid System](https://www.w3schools.com/bootstrap4/bootstrap_grid_basic.asp)

3. **MDN Web Docs**:
   - Embora não seja específico do Bootstrap, o MDN Web Docs oferece uma excelente base sobre CSS Flexbox e Grid Layout, que são fundamentais para entender como funciona a responsividade e o sistema de layout em frameworks como o Bootstrap.
   - [MDN Web Docs sobre CSS Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)
   - [MDN Web Docs sobre CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)

Explore esses recursos, pratique e bons estudos!

---
**Professor Ederson**

## Código-Fonte do Projeto

### index.html

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Responsiva com Bootstrap</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" type="text/css" href="css/styles.css">
</head>
<body>
    <!-- Cabeçalho -->
    <header class="bg-primary text-white text-center py-5">
        <h1>Bem-vindo ao Projeto Responsivo</h1>
        <p>Explore os elementos e veja como se comportam em diferentes tamanhos de tela</p>
    </header>

    <!-- Navegação -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
                <li class="nav-item active">
                    <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Features</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Pricing</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
                </li>
            </ul>
        </div>
    </nav>

    <!-- Conteúdo Principal -->
    <main class="container my-5">
        <div class="row">
            <!-- Coluna da Esquerda -->
            <div class="col-lg-8">
                <!-- Cards -->
                <div class="card mb-4">
                    <div class="card-header">Card Header</div>
                    <div class="card-body">
                        <h5 class="card-title">Card Title</5>
                        <p class="card-text">Este é um exemplo de card. Você pode usá-lo para mostrar informações importantes.</p>
                        <a href="#" class="btn btn-primary">Go somewhere</a>
                    </div>
                </div>
                <!-- Tabela -->
                <h2>Tabela Responsiva</h2>
                <div class="table-responsive">
                    <table class="table">
                        <thead>
                            <tr>
                                <th>#</th>
                                <th>Nome</th>
                                <th>Idade</th>
                                <th>Email</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>1</td>
                                <td>João</td>
                                <td>25</td>
                                <td>joao@example.com</td>
                            </tr>
                            <tr>
                                <td>2</td>
                                <td>Maria</td>
                                <td>30</td>
                                <td>maria@example.com</td>
                            </tr>
                            <tr>
                                <td>3</td>
                                <td>Pedro</td>
                                <td>35</td>
                                <td>pedro@example.com</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
            <!-- Coluna da Direita -->
            <div class="col-lg-4">
                <!-- Formulário -->
                <h2>Formulário</h2>
                <form>
                    <div class="form-group">
                        <label for="name">Nome</label>
                        <input type="text" class="form-control" id="name" placeholder="Digite seu nome">
                    </div>
                    <div class="form-group">
                        <label for="age">Idade</label>
                        <input type="number" class="form-control" id="age" placeholder="Digite sua idade">
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" class="form-control" id="email" placeholder="Digite seu email">
                    </div>
                    <button type="submit" class="btn btn-primary">Enviar</button>
                </form>
            </div>
        </div>
    </main>

    <!-- Rodapé -->
    <footer class="bg-dark text-white text-center py-3">
        <p>&copy; 2024 Projeto Responsivo. Todos os direitos reservados.</p>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.2/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
