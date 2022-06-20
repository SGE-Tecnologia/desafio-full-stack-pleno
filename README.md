# Desafio Fullstack Pleno
Seja bem-vindo! Este desafio foi projetado para avaliar a sua capacidade técnica como candidato à vaga de Desenvolvedor Fullstack Pleno.

## Proposta
Você deverá desenvolver uma aplicação de monitoramento de preços do mercado de energia. Para isso, separaremos a proposta desse desafio em duas etapas:

Crie o seu projeto como um repositório público do github e nos envie o link.

### Back-end
Desenvolva uma API utilizando Java com Spring Boot que deve conter as seguintes rotas:
- `/register` - [POST] - esta rota deve cadastrar um usuário;
- `/login` - [POST] - esta rota deve autenticar um usuário;
- `/coletar-precos` - [POST] (requer autenticação) - esta rota deve iniciar uma coleta dos preços de energia disponíveis em uma fonte externa:
- - O endereço https://www.ccee.org.br/precos/painel-precos disponibiliza o download de uma planilha com dados históricos no final da página;
- - Essa rota deve iniciar uma rotina que irá se conectar nessa página e realizar o download da planilha de "Preço Médio Mensal" dos últimos 12 meses e salvar os dados em um banco de dados;
- `/precos-mensais` - [GET] (requer autenticação) - esta rota deve listar os preços médios de energia mensal por região dos últimos 12 meses que foram coletados pela rota enterior;

### Front-end
Desenvolva uma aplicação web utilizando o React.js e esta deve atender as seguintes histórias:
 - Eu como usuário desejo me cadastrar;
 - Eu como usuário desejo realizar login;
 - Eu como usuário autenticado desejo visualizar um gráfico com os preços de energia dos últimos 12 meses;
 - Eu como usuário autenticado desejo iniciar uma coleta dos preços de energia mais recentes ao clicar em um botão;

## Diferenciais
Consideraremos como diferenciais os seguintes pontos:
- Deploy realizado em qualquer ambiente em nuvem;
- Criação de testes unitários;
- Criação de testes de integração.

**Observações:**
- Sua aplicação web DEVE se comunicar com sua API;
- Você pode utilizar o banco de dados de sua preferência (relacional ou não relacional).
