# HS-Tech - Sprint 1

## Descricao

Este projeto tem como objetivo a criacao de um dashboard que visa representar os dados dos pacientes.

## Equipe
* Erick Yuki Emori
* Vinicius R. Tavares

## Organizacao dos diretorios

    ├── Dashboard/          (diretório contendo o dashboard principal e suas paginas)
    |   ├── pages/
    |   ├── ├── 1_Principal.py        (pagina inicial do dahsboard, representando os graficos)
    |   |   ├── 2_Filtro.py           (pagina que possui o filtro com os dados de todos os pacientes)
    |   |   └── 3_User.py             (pagina que possui os dados de um usuario especifico)
    |   └── Contatos.py        (pagina inicial do dahsboard, contendo os contatos dos residentes)
    ├── docker_params/      (diretorio que possui arquivos necessarios para o docker)
    |   └── requirements.txt    (arquivo que possui requerimentos para o python)
    ├──  notebooks/         (notebooks com algumas funcoes que foram testadas individualmente antes de serem aplicadas no dashboard, nao e necessario para 
    └──  Dockerfile (documento utilizado para criar o docker)

## Como utilizar
### Criando a imagem docker
#### 1. Instale o docker na maquina atual
##### https://docs.docker.com/engine/install/ubuntu/

#### 2. Crie a imagem baseado no documento Dockerfile
##### rode o comando na pasta root desse projeto "docker build -t hs-tech-dashboard:latest -f Dockerfile ."

#### 3. Execute a imagem
##### rode o comando "docker run -p 8501:8501 hs-tech-dashboard:latest"

#### 4. Abra o dashboard
##### Acesse o seguinte site: "http://localhost:8501/"
