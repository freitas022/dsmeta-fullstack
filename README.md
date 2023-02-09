# DSMeta Project

[![NPM](https://img.shields.io/npm/l/react)](https://github.com/devsuperior/sds1-wmazoni/blob/master/LICENSE)

# Sobre o projeto

DSMeta é uma aplicação full stack web construída durante a **Semana DevSuperior**, evento organizado pela [DevSuperior](https://devsuperior.com.br/cursos "Site da DevSuperior").

A aplicação web consiste em controlar uma lista de vendas com filtro de data, seus vendedores e notificar via SMS no seu dispositivo o total de vendas de cada um deles.

## Layout mobile

![Mobile 1](https://github.com/freitas022/dsmeta-layouts/blob/main/mobile.png?raw=true)

## Layout web 576px

![Web 1](https://github.com/freitas022/dsmeta-layouts/blob/main/web576.png?raw=true)

## Layout web 992px

![Web 2](https://github.com/freitas022/dsmeta-layouts/blob/main/web992.png?raw=true)

# Tecnologias utilizadas

## Back end

- API REST com Java e Spring Boot
- Banco de Dados com ORM
- JPA / Hibernate
- Maven
- Integração com SMS

## Front end

- HTML / CSS
- JS
- TypeScript
- ReactJS

## Implantação em produção

- Devido a retirada do plano gratuito do Heroku o aplicativo só funciona localmente.

# Configurando o projeto

```bash
# clonar repositório
git clone https://github.com/freitas022/simple-project-java-react.git
```

## Configurando o back-end antes de rodar o projeto

Pré-requisitos: STS / Eclipse / Twilio Account

Antes de configurar o projeto crie uma conta na [Twilio](https://www.twilio.com/try-twilio "Site da Twilio"), será necessário para enviar o SMS.

Faça o download do [SpringToolSuite](https://spring.io/tools "Spring site") e faça a importação do projeto usando o Maven e aguarde compilar das dependências.

```bash
# configurando variáveis de ambiente para enviar SMS com Twilio
- Clicar no pacote principal 
- Run As 
- Run Configurations
- Spring Boot App / {nome da aplicação} 
- Env 
- Add

# Adicionando variáveis de ambiente para não expor nossos dados 
Name = TWILIO_SID
Value = Colar a sua ID Account do Twilio;

Name = TWILIO_KEY
Value = Colar o seu AuthToken;

Name = TWILIO_PHONE_FROM
Value = Colar o seu número Twilio;

Name = TWILIO_PHONE_TO
Value = Colar o seu número de telefone para receber o SMS;

```

# Como executar o projeto

## Back-end
Pré-requisitos: Java 17

```bash

# entrar na pasta do projeto backend
cd backend

# executar o projeto
./mvnw spring-boot:run
 
# parar o projeto
ctrl + c
```

## Front-end
Pré-requisitos: npm / yarn

```bash
# entrar na pasta do projeto frontend
cd frontend

# instalar dependências
yarn install 

# executar o projeto
yarn run dev

# parar o projeto
ctrl + c
```

# Autor

Matheus Freitas da Silva

[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/matheus-freitas-0b27a8217/)