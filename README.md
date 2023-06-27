# Email and password validator

O projeto consiste em um formulário de registro que valida o email e a senha inseridos pelo usuário. Ele utiliza HTML, CSS e JavaScript para criar a interface do usuário e implementar a lógica de validação.

O código fornecido consiste em um formulário de registro que solicita o nome, email e senha do usuário com restrições. Vamos analisar cada parte do código em mais detalhes:

### HTML (index.html)
Este trecho de código HTML cria a estrutura básica do formulário de registro. Aqui estão os principais elementos utilizados:

- `<section>`: Define uma seção do documento.
- `<h1>`: Título principal exibido na página.
- `<form>`: Cria um formulário que agrupa os elementos do registro.
- `<label>`: Rótulo para os campos do formulário.
- `<input>`: Caixa de entrada para inserção de texto.
- `<span>`: Elemento para exibir mensagens de erro.

### CSS (index.css)
O arquivo CSS contém estilos para tornar o formulário visualmente agradável. Aqui estão algumas das regras de estilo aplicadas:

- Definição da fonte, margens e alinhamento do texto.
- Estilização da seção do formulário com cores de fundo, bordas arredondadas e sombras.
- Estilização dos elementos do formulário, como espaçamentos, bordas e tamanho de fonte.
- Definição de estilos para exibição de mensagens de erro.
- Estilização do botão de registro com cor de fundo e efeito de hover.

### JavaScript (index.js)
O código JavaScript adiciona interatividade ao formulário, validando o email e a senha inseridos pelo usuário. Aqui está uma explicação detalhada das principais partes do código:

- `validateEmail(email)`: Esta função recebe um email como parâmetro e verifica se ele corresponde ao padrão de um endereço de email válido. Caso contrário, ela cria um objeto de erro personalizado contendo uma mensagem de erro e o campo de entrada relacionado.

- `validatePassword(password)`: Essa função recebe uma senha como parâmetro e verifica se ela atende a determinados critérios de validação. Ela verifica se a senha tem pelo menos 8 caracteres, contém pelo menos uma letra maiúscula, uma letra minúscula, um número e um caractere especial. Caso a senha não atenda a esses critérios, a função lança um objeto de erro personalizado contendo uma mensagem de erro e o campo de entrada relacionado.

- `resetFormStyles()`: Essa função remove as classes CSS "success" e "error" dos elementos de entrada do formulário e limpa as mensagens de erro exibidas.

- `userInputs`: Um objeto que armazena as referências para os elementos de entrada do formulário (nome, email e senha).

- `form.addEventListener('submit', (ev) => {...})`: Esse trecho de código adiciona um ouvinte de eventos ao formulário para capturar o evento de envio (submit). Quando o formulário é enviado, ele executa o código dentro da função de callback.

Dentro da função de callback, os estilos do formulário são redefinidos chamando `resetFormStyles()`. Em seguida, são realizadas as seguintes etapas de validação:

1. O campo do nome é marcado como "success" (sucesso) para fins de estilização.

2. A função `validateEmail()` é chamada com
