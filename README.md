## Santander Dev Week
Java RESTful API criada para a Santander Dev Week.

# Santander Dev Week 2023 Java API

RESTful API da Santander Dev Week 2023 construída em Java 17 com Spring Boot 3.

## 🚀 Principais Tecnologias

- ☕ Java 17  
Utilizamos a versão LTS do Java para aproveitar recursos modernos, melhor desempenho e maior estabilidade no desenvolvimento da aplicação.

- 🌱 Spring Boot 3  
Framework utilizado para acelerar o desenvolvimento da API REST, utilizando autoconfiguração e boas práticas do ecossistema Spring.

- 🗄️ Spring Data JPA  
Responsável pela camada de persistência de dados, facilitando a integração com bancos de dados relacionais através de repositories e ORM.

- 📄 OpenAPI (Swagger)  
Ferramenta utilizada para documentação da API, permitindo visualizar e testar os endpoints de forma simples e organizada.

- ☁️ Railway  
Plataforma utilizada para deploy e hospedagem da aplicação, oferecendo integração simples com banco de dados e CI/CD.

## 🎨 Link do Figma

O Figma foi utilizado para a abstração do domínio desta API, auxiliando na análise, modelagem e prototipação da solução.

🔗 https://www.figma.com/design/0ZsjwjsYlYd3timxqMWlbj/SANTANDER---Projeto-Web-Mobile?node-id=1421-432&t=rfK5zfMMwVihKA94-0
## Diagrama De Classes

``` mermaid
classDiagram

class User {
  -String name
  -Account account
  -Feature[] features
  -Card card
  -News[] news
}

class Account {
  -String number
  -String agency
  -Number balance
  -Number limit
}

class Feature {
  -String icon
  -String description
}

class Card {
  -String number
  -Number limit
}

class News {
  -String icon
  -String description
}

User "1" *-- "1" Account
User "1" *-- "N" Feature
User "1" *-- "1" Card
User "1" *-- "N" News
```
## 📄 Documentação da API (Swagger)

A documentação da API foi gerada utilizando OpenAPI (Swagger), permitindo visualizar e testar todos os endpoints da aplicação.

🔗 https://std-2026-api-prd.up.railway.app/swagger-ui/index.html

Esta API está hospedada no Railway e pode ficar indisponível futuramente. Como o projeto é open-source, você pode cloná-lo, modificar e executar localmente sem problemas.

---

## 🌐 URL de Produção

🔗 https://std-2026-api-prd.up.railway.app/users/1
