# ATIVIDADE
"Crie um aplicativo simples capaz de consumir um serviço e proporcionar algum benefício no cenário das cidades inteligentes. O app deve conter, no mínimo, duas e, no máximo, cinco telas.

A ideia principal é que apenas consuma um serviço já existente, não se preocupe em criar um back-end, apenas crie o back-end se for do seu interesse e queira produzir algum serviço específico para atender seu projeto, no mais, existem muitos serviços gratuitos na internet que podem ser úteis em cidades inteligentes, desde informações sobre clima, geolocalização, endereços de entrega, entre outros.

Lembre-se: para esta entrega, você deverá criar um app utilizando o conteúdo da fase, ou seja, um app nativo em Android ou iOS, você decide baseado no tipo de equipamento que possua."

## Pré-requisitos

- API 27 - Android Oreo (8)
- IDE: Android Studio Iguana
## Tecnologias Utilizadas

### Backend
- **Kotlin:** Linguagem principal utilizada para o desenvolvimento do backend.
- **Brasil API:** Utilizada para acessar dados específicos do Brasil, como informações de veículos através da API FIPE - https://brasilapi.com.br/docs#tag/FIPE/paths/~1fipe~1preco~1v1~1{codigoFipe}/get
- **SQLite:** Banco de dados utilizado para armazenamento local.

### Frontend
- **JetpackCompose:** Utilizado para a criação da interface do usuário (UI).

### Bibliotecas e Ferramentas
- **Retrofit e GSON:** Utilizados para fazer requisições em APIs e desserializar os dados retornados.
- **JSOUP:** Utilizado para fazer webscraping (Parser HTML).
- **ROOM:** ORM utilizado para manipulação do SGBD SQLite.
- **LiveData:** Utilizado para observar e reagir a mudanças nos dados, de acordo com a arquitetura MVVM.
- **Remember:** Utilizado para observar e reagir a mudanças nos dados, State Hoisting
  
## Hands On
https://github.com/pedroferrarezzo/FIPETracker---FIAP/assets/124400471/47af4c16-d670-4aa1-89fc-e28452221d92

## Descrição

O FIPETracker é um aplicativo desenvolvido na linguagem de programação nativa para sistemas operacionais Android - Kotlin, utilizando bibliotecas como ROOM, Retroft, GSON, JSOUP e LiveData. 
Este sistema visa facilitar o encontro de dados sobre os veículos de interesse dos clientes para fins diversos, como negociações entre vendedores e compradores, ou até mesmo pesquisas ligadas a esse mercado.

## Funcionalidades Principais

- **Consulta de veículos com base em um código FIPE:** Pesquise dados de veículos rapidamente;
- **Visualização de dados objetiva:** Após a consulta, obtenha dados assertivos como: preço, ano, tipo de combustível e mês referência;
- **Filtro de dados:** Visualize dados do veículo por ano de lançamento;
- **Imagens:** Após a consulta, imagens do veículo e da marca serão exibidas por meio de um webscrapping na página do Google Images, para melhor análise;
- **Salve para ver depois:** Requisições para API demandam conexão externa, é possível salvar a consulta no banco de dados SQLite para posterior visualização sem a necessidade de internet.
