# 	:woman_technologist: Project Docker Todo List

Esse projeto contém uma série de informações sobre o que eu aprendi aqui na Trybe ao longo  do curso de desenvolvimento web da Trybe. <br>
Foi o meu primeiro contato com os containers do Docker.

## :rocket:Começando
Esse projeto foi proposto pelo curso de desenvolvimento web da Trybe.
### Desenvolvimento
Esse proejto foi desenvolvido no bloco de back-end, usei containers do Docker e fiz um Dockerfile.
### Commits
Os commits foram feitos de acordo com os requisitos finalizados.
### Branch
Todo o projeto foi feita na branch 'juliana-oliveira-project-docker-todo-list', isso por conta da exigência do curso.
### Instalação
Antes de realizar o projeto, precisei instalar as dependências usando npm install.
### Testes
Os testes usando foram ESLint e Cypress, através dos **comandos**: <br>
* npm test
### Autores
Esse foi um projeto individual,que desenvolvido somente por Juliana Oliveira.
### Ferramentas usadas
Foi usado Visual Studio Code, além do Trello que auxiliou na organização das tarefas.
### Framework usado
Nenhum.
### Informações Importantes
Na pasta docker-commands foram criados arquivos commandx.dc. O x equivale o requisito que foi feito. Exemplo: command01.dc equivale ao requisito 1.

## :footprints:Requisitos
### Metodologia usada
No trabalho do desenvolvimento de software a gente sempre tem prazos, muitas vezes os prazos são apertados.<br>
Por outro lado, eu não quero criar algo que não entendo perfeitamente, como também fazer códigos rápidos pode levar a erros que podem demorar muito pra corrigir.<br>
Por isso, usei e sempre uso o método Baby Steps, que é uma estratégia de abordar o desafio passo à passo, defensivamente.<br>
Baby steps é um termo em inglês que quer dizer passos de bebê. Refere-se a fazer as coisas, quaisquer que sejam, devagar, com calma, passo a passo.
#### :footprints:Requisito 1
Crie um container em modo interativo, sem rodá-lo, nomeando-o como 01container e utilizando a imagem alpine na versão 3.12.
* O container não deve ser inicializado, somente criado;
* O container deve estar preparado para acesso interativo.
* Lembre-se que um parâmetro não é necessariamente aplicável a apenas um comando.
#### :footprints:Requisito 2
Inicie o container 01container.
#### :footprints:Requisito 3
Liste os containers filtrando pelo nome 01container.
#### :footprints:Requisito 4
Execute o comando cat /etc/os-release no container 01container sem se acoplar a ele.
#### :footprints:Requisito 5
Remova o container 01container.
#### :footprints:Requisito 6
Execute o comando cat /etc/os-release no container 01container sem se acoplar a ele.
#### :footprints:Requisito 7
Rode um novo container com a imagem nginx com a versão 1.21.3-alpine em segundo plano nomeando-o como 02images e mapeando sua porta padrão de acesso para porta 3000 do sistema hospedeiro.
* Que é possível ter acesso ao container pelo endereço localhost:3000.
#### :footprints:Requisito 8
Pare o container 02images que está em andamento.
#### :footprints:Requisito 9
Gere uma build a partir do Dockerfile do back-end do todo-app nomeando a imagem para todobackend.
* Se existe um arquivo Dockerfile em ./docker/todo-app/back-end/:
* O Dockerfile deve rodar uma imagem node utilizando a versão 14;
* Recomenda-se o uso da variante -alpine, pois ela é otimizada para desempenho;
* Lembre-se de consultar o README do todo-app para validar os requisitos da aplicação.
* Deve estar com a porta 3001 exposta;
* Deve adicionar o arquivo node_modules.tar.gz a imagem;
* Deve copiar todos os arquivos da pasta back-end para a imagem;
* Ao iniciar a imagem deve rodar o comando npm start.
* Se ao buildar o Dockerfile o nome da imagem gerada é igual a todobackend.
#### :footprints:Requisito 10
Gere uma build a partir do Dockerfile do front-end do todo-app nomeando a imagem para todofrontend.
* Se existe um arquivo Dockerfile em ./docker/todo-app/front-end/:
* O Dockerfile pode rodar uma imagem node utilizando a versão 14;
* Recomenda-se o uso da variante -alpine, pois ela é otimizada para desempenho;
* Lembre-se de consultar o README do todo-app para validar os requisitos da aplicação.
* Deve estar com a porta 3000 exposta;
* Deve adicionar o arquivo node_modules.tar.gz a imagem, de maneira que ele seja extraído dentro do container;
* Deve copiar todos os arquivos da pasta front-end para a imagem;
* Ao iniciar a imagem deve rodar o comando npm start;
* Se ao buildar o Dockerfile o nome da imagem gerada é igual a todofrontend.
#### :footprints:Requisito 11
Gere uma build a partir do Dockerfile dos testes do todo-app nomeando a imagem para todotests.
* O comando ADD do Dockerfile, também pode ser utilizado para descompactar arquivos dentro do container.
* Se existe um arquivo Dockerfile em ./docker/todo-app/tests/:
* O Dockerfile deve rodar a imagem mjgargani/puppeteer:trybe1.0 para que os testes funcionem;
* Deve adicionar o arquivo node_modules.tar.gz a imagem;
* Deve copiar todos os arquivos da pasta tests para a imagem;
* Ao iniciar a imagem deve rodar o comando npm test;
* Se ao buildar o Dockerfile o nome da imagem gerada é igual a todotests.

