

1. O que é o Node.js?

Node.js é um ambiente de execução (runtime) que permite rodar JavaScript fora do navegador, principalmente no servidor.

Ele não é uma linguagem de programação, porque utiliza a linguagem JavaScript, que já existe.
Ele é considerado um ambiente de execução porque fornece recursos para executar o código JavaScript no sistema operacional, como:

Acesso a arquivos

Criação de servidores

Manipulação de processos

Comunicação em rede

2. Diferença entre Node.js e JavaScript no navegador

Duas diferenças importantes:

1️⃣ Ambiente de execução

No navegador: roda dentro do browser (Chrome, Firefox etc.).

No Node.js: roda no servidor ou no computador.

2️⃣ Acesso ao sistema

No navegador: não pode acessar arquivos do sistema por segurança.

No Node.js: pode acessar arquivos, banco de dados, criar servidores etc.

3. O que é o V8 Engine?

O V8 é o motor JavaScript criado pelo Google (usado no Chrome).

Ele é responsável por:

Interpretar e compilar o código JavaScript

Transformar JavaScript em código de máquina

No Node.js, o V8 permite que o JavaScript seja executado fora do navegador com alto desempenho.

4. O que é E/S não bloqueador?

E/S significa Entrada e Saída (Input/Output), como:

Leitura de arquivos

Requisições HTTP

Acesso a banco de dados

No Node.js, essas operações são não bloqueadoras, ou seja:
O programa não fica parado esperando a operação terminar.

Isso melhora o desempenho porque:

O servidor pode atender outras requisições enquanto espera a resposta

Permite lidar com muitas conexões ao mesmo tempo

5. O que é o Event Loop?

O Event Loop é o mecanismo que permite ao Node.js executar operações assíncronas.

Funcionamento resumido:

O código é executado.

Operações demoradas (como leitura de arquivo) são enviadas para o sistema.

Quando terminam, entram em uma fila.

O Event Loop verifica essa fila e executa as funções de retorno (callbacks).

Ele permite que o Node.js funcione de forma assíncrona usando apenas uma thread principal.

6. O que são módulos no Node.js?

Módulos são blocos de código reutilizáveis.

Tipos:

🔹 Módulos internos (core modules)
Já vêm com o Node.js.
Ex: fs, http, path.

🔹 Módulos externos
Instalados via npm.
Ex: express, axios.

🔹 Módulos criados pelo desenvolvedor
Arquivos criados dentro do próprio projeto.
Ex: utils.js, database.js.

7. Para que serve o arquivo package.json?

O package.json guarda as informações do projeto.

Ele pode conter:

Nome e versão do projeto

Lista de dependências

Scripts (ex: "start": "node index.js")

Autor

Licença

8. O que é o npm?

npm significa Node Package Manager.

Funções:

Instalar bibliotecas (npm install)

Gerenciar dependências

Atualizar pacotes

Executar scripts do projeto

Ele facilita o desenvolvimento ao permitir reutilizar códigos prontos da comunidade.

9. O que é uma API REST e como o Node.js pode ser usado?

Uma API REST é uma interface que permite comunicação entre sistemas usando HTTP.

Ela utiliza métodos como:

GET

POST

PUT

DELETE

No Node.js, podemos usar frameworks como Express para:

Criar rotas

Receber requisições

Enviar respostas em JSON

Conectar com banco de dados

10. Duas vantagens e duas desvantagens do Node.js

✅ Vantagens:

Alto desempenho em aplicações com muitas conexões simultâneas.

Usa JavaScript no front-end e back-end (mesma linguagem).

❌ Desvantagens:

Não é ideal para tarefas muito pesadas de processamento (CPU intensivo).

Pode ficar complexo lidar com muitas operações assíncronas (callbacks).
