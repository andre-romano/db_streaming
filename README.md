# Sistema de Streaming de Video (usando PHP e MySQL)

Este sistema serve de exemplo para vocês se basearam para construir o sistema de vocês.

Cada pasta tem uma finalidade especifica nesse projeto:
- **[css](./css)**: Armazena arquivos de estilo CSS
- **[db](./db)**: Armazena arquivos de banco de dados .SQL e o modelo lógico do BrModelo
- **[img](./img)**: Armazena imagens 
- **[js](./js)**: Armazena scripts Javascript
- **[src](./src)**: Armazena scripts PHP (que serão usados para criar as telas do seu sistema)

As telas do seu sistema devem estar na raiz desta pasta (veja o exemplo de [consulta_video.php](./consulta_video.php))

Dentro de **./src** temos alguns arquivos interessantes:
- **[bootstrap_components.php](./src/bootstrap_components.php)**: Contem funções do PHP para criar componentes Bootstrap
  - Use as funções desse arquivo para facilitar na hora de criar suas telas
- **[db_connection_pdo.php](./src/db_connection_pdo.php)**: Faz a conexao com o banco de dados
  - Você deve modificar ela para colocar o nome do seu banco de dados na variavel `$db` deste arquivo
- **[db_disconnect_pdo.php](./src/db_disconnect_pdo.php)**: Desconecta o PHP do DB 
- **[nav_bar.php](./src/nav_bar.php)**: Barra de navegação do seu site (escrita em Bootstrap)
  - Voce deve modificar ela para incluir as telas do seu sistema (consultas, inserções, etc)

Quando voce acessa o seu sistema (usando `http://localhost/NOME_PASTA_DO_PROJETO`) a primeira tela que o usuário verá é o arquivo **[index.php](./index.php)**

**IMPORTANTE**: Antes de usar esse sistema, importe o arquivo do banco de dados (``.SQL``) que esta na pasta **[./db](./db/)** usando o PHPMyAdmin. Isso irá criar o banco de dados `streaming` dentro do MySQL.