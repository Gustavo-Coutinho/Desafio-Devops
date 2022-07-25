## Desafio DevOps concluído!
Após cerca de 36 horas dedicadas a esse projeto, consegui concluir a entrega dentro de 5 dias. Apesar de ser uma aplicação simples, os procedimentos de elaboração de container, docker-compose e github actions precisam ser muito bem estudados. Sendo assim, acredito que esse projeto me ensinou um pouco de como uma empresa real (Frexco) trabalha com os conceitos de DevOps. 
## Como executar o projeto
Após clonar o repositório, abra em sua máquina um terminal no diretório web/ e execute o comando:

    docker compose up
> **_NOTA:_**  Você precisa ter instalado em sua máquina o [Docker](https://www.docker.com/products/docker-desktop/) e o [Docker-compose](https://docs.docker.com/compose/install/compose-plugin/#install-the-plugin-manually).
## Como testar a aplicação Django
Após executar o projeto, abra uma nova janela do terminal e execute o comando:

    docker exec -it frexco-app "python manage.py test"

## Visão geral dos requisitos
### :white_check_mark: 1. Aplicação deverá conter um arquivo Dockerfile para realizar a build (construção da aplicação)
### :white_check_mark: 2. O arquivo responsável por subir o container deverá ser o Docker-compose contendo as demais informações (Ex. porta, nome, imagem e etc...)
### :white_check_mark: 3. O container deverá rodar em uma porta diferente da 8000, pois a aplicação da API já vem pré-configurada para isso, e queremos que explore e entenda as configurações de porta do Docker
### :white_check_mark: 4. Implementar a Pipeline CI no Github actions
### :white_check_mark: 5. Implementar conexão com banco de dados PostgreSQL (Implementar uma nova instancia no docker e fazer a parte de comunicação com a API.
### :white_check_mark: 6. Utilização de NGINX para permitir o acesso através da porta 80 direcionando para a porta do container
### :white_check_mark: 7. Projeto bem documentado no GitHub (Arquivo Readme bem detalhado), incluindo instruções de como executar e testar o desafio
### :black_square_button: 8. (Extra) Criar um pipeline CD - O principal objetivo é ver como você organiza o arquivo de configuração "deploy.yml", responsável por esse papel
