## MoniBank

MoniBank é um projeto de serviços bancários online, permitindo aos usuários criar uma conta corrente. Abaixo está uma descrição detalhada da estrutura do código e instruções para configurar e executar o projeto.

### Estrutura do Projeto

- **index.html**: Página inicial do site.
- **styles/**: Pasta que contém os arquivos CSS para estilização do site.
  - **styles.css**: Arquivo principal de estilos.
  - **formulario/**: Pasta que contém estilos específicos para o formulário.
    - **styles.css**: Estilos específicos para a página de formulário.
- **img/**: Pasta que contém as imagens usadas no site.
- **js/**: Pasta que contém os arquivos JavaScript.
  - **script.js**: Script principal para validação e manipulação do formulário.
  - **camera.js**: Script que permite tirar uma foto para o cadastro.
  - **valida-cpf.js**: Script que permite validar o CPF do cadastro.
  - **valida-idade.js**: Script que permite validar a idade do usuário.

### Estrutura do HTML

- **Cabeçalho (header)**:
  - Contém o logotipo e a barra de navegação com links para "Sobre", "Serviços", campo de busca, e botões para "Abrir conta" e "Acessar conta".
- **Seção de Banner**:
  - Um título promovendo a abertura de conta.
- **Main (container)**:
  - **Breadcrumb**: Indica a localização da página atual.
  - **Seção de Formulário**:
    - Um formulário para criar uma conta corrente, com campos para nome, email, RG, CPF, data de nascimento e termos de serviço.
- **Rodapé (footer)**:
  - Contém informações sobre a empresa, serviços oferecidos, contatos e links para redes sociais.

### Validação do Formulário

O formulário usa JavaScript para validar os campos antes de enviar os dados. Há verificações para garantir que os campos não estejam vazios e que os dados inseridos estejam no formato correto.

### JavaScript

- **script.js**:
  - Adiciona eventos de validação aos campos do formulário.
  - Impede o envio do formulário se os dados estiverem incorretos.
  - Armazena os dados no `localStorage` e redireciona para a próxima página após a submissão bem-sucedida.
  - Valida CPF e data de nascimento através de funções customizadas `ehUmCPF` e `ehMaiorDeIdade`.

### Como Executar o Projeto

1. **Clonar o Repositório**:
   ```bash
   git clone https://github.com/seu-usuario/monibank.git
   ```
2. **Navegar para o Diretório**:
   ```bash
   cd monibank
   ```
3. **Abrir o Arquivo HTML**:
   - Abra o arquivo `index.html` em seu navegador preferido para visualizar a página inicial do MoniBank.
   - Navegue para a página de abrir conta para ver o formulário e testar a validação dos campos.

### Dependências Externas

- **Google Fonts**:
  - Fontes usadas: Inter e Montserrat.
- **Reset CSS**:
  - Para resetar estilos padrão do navegador.
