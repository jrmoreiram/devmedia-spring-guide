# Guia de Spring Framework

Bem-vindo ao meu repositório de projetos Java com Spring Framework! Este guia de referência foi criado para me ajudar a compreender e implementar aplicações utilizando o ecossistema Spring baseado em um curso de Spring que estou realizando pela plataforma [DevMedia](https://www.devmedia.com.br/).

<p align="center">
  <img src="https://spring.io/img/spring.svg" alt="Spring Logo" width="300" />
</p>

## 📋 Conteúdo

- [Introdução](https://www.devmedia.com.br/spring/introducao)
- [Aplicações Web MVC](https://www.devmedia.com.br/spring/aplicacoes-web-mvc)
- [Banco de Dados](https://www.devmedia.com.br/spring/banco-de-dados)
- [Autenticação em Aplicações Web MVC](https://www.devmedia.com.br/spring/autenticacao-em-aplicacoes-web-mvc)
- [Web Services RESTful](https://www.devmedia.com.br/spring/web-services-restful)
- [Relatórios](https://www.devmedia.com.br/spring/relatorios)
- [Boas Práticas](https://www.devmedia.com.br/spring/boas-praticas)

## 🚀 Introdução

O Spring Framework é um framework de código aberto para a plataforma Java que oferece suporte abrangente para o desenvolvimento de aplicações empresariais. Criado para abordar a complexidade do desenvolvimento de software corporativo, o Spring se baseia em princípios fundamentais como Inversão de Controle (IoC) e Injeção de Dependências (DI).

### Principais Componentes do Ecossistema Spring

- **Spring Boot**: Facilita a criação de aplicações stand-alone baseadas em Spring
- **Spring MVC**: Framework para desenvolvimento de aplicações web
- **Spring Data**: Simplifica o acesso a dados em diversos bancos
- **Spring Security**: Provê autenticação e autorização para aplicações
- **Spring Cloud**: Ferramentas para sistemas distribuídos

### Como Começar

Para iniciar um projeto Spring, recomendamos usar o [Spring Initializr](https://start.spring.io/), uma ferramenta web que gera a estrutura básica do projeto com as dependências selecionadas.

```bash
# Clone este repositório
git clone https://github.com/seu-usuario/spring-guide.git

# Entre no diretório
cd spring-guide

# Execute o projeto de exemplo (requer Maven instalado)
./mvnw spring-boot:run
```

## 💻 Aplicações Web MVC

O Spring MVC é um framework web robusto que implementa o padrão Model-View-Controller e facilita o desenvolvimento de aplicações web dinâmicas.

### Recursos Principais

- Controllers para manipular requisições HTTP
- Integração com engines de templates como Thymeleaf, FreeMarker, e JSP
- Validação de formulários e binding de dados
- Interceptadores para processamento de requisições
- Gerenciamento de exceções

## 🗄️ Banco de Dados

O Spring oferece excelente suporte para interação com bancos de dados através do Spring Data e outras tecnologias relacionadas.

### Spring Data JPA
O Spring Data JPA é uma parte do ecossistema Spring que simplifica a implementação da camada de persistência de aplicações Java. Ele fornece uma abstração sobre o JPA (Java Persistence API), reduzindo significativamente a quantidade de código necessário para interagir com bancos de dados.

Características principais:
- Implementa automaticamente métodos CRUD (Create, Read, Update, Delete)
- Permite criar consultas apenas declarando métodos em interfaces (query methods)
- Suporta consultas personalizadas com JPQL ou SQL nativo
- Facilita a paginação e ordenação de resultados
- Implementa o padrão de repositório

Em vez de escrever manualmente código para persistência, você só precisa definir interfaces que estendem os repositórios do Spring Data JPA, e a implementação é gerada automaticamente em tempo de execução.

### Recursos de Persistência

- ORM com Hibernate
- Consultas derivadas de métodos
- Transações declarativas
- Migrações de schema com Flyway ou Liquibase
- Suporte a múltiplos bancos de dados (MySQL, PostgreSQL, MongoDB, etc.)

Exemplos práticos estão disponíveis na pasta [/database-examples](/database-examples).

## 🔐 Autenticação em Aplicações Web MVC

O Spring Security fornece recursos abrangentes para autenticação e autorização em aplicações web.


### Recursos de Segurança

- Autenticação form-based, HTTP Basic, OAuth 2.0
- Autorização baseada em roles e permissões
- Proteção contra CSRF, XSS e outros ataques
- Integração com LDAP, JDBC, e outros provedores de autenticação
- Remember-me authentication

## 🌐 Web Services RESTful

O Spring oferece suporte excepcional para criação de APIs RESTful através do Spring Web e Spring Data REST.

### Recursos para APIs

- Serialização/desserialização automática JSON/XML
- Validação de requisições
- Documentação com Swagger/OpenAPI
- HATEOAS para APIs RESTful maduras
- Versionamento de API


## 📊 Relatórios

O Spring suporta várias maneiras de gerar relatórios em diferentes formatos.

### Integração com Bibliotecas de Relatórios

- JasperReports para relatórios PDF, Excel, HTML
- Apache POI para manipulação de planilhas Excel
- Exportação de dados para CSV
- Geração de gráficos com bibliotecas JavaScript

## 👍 Boas Práticas

Seguir boas práticas é essencial para manter seu código limpo, seguro e fácil de manter.

### Arquitetura em Camadas

```
src/main/java/com/exemplo/
  ├── controller/     # Controladores REST e MVC
  ├── service/        # Regras de negócio
  ├── repository/     # Acesso a dados
  ├── model/          # Entidades e DTOs
  ├── config/         # Configurações
  ├── exception/      # Exceções personalizadas
  └── util/           # Classes utilitárias
```

### Recomendações

- **Testes Automatizados**: Use JUnit, Mockito e MockMVC para garantir a qualidade do código
- **Documentação**: Documente APIs com Swagger/SpringDoc
- **Logs**: Implemente logging adequado com SLF4J e Logback
- **DTOs**: Use objetos de transferência de dados para separar representação externa da interna
- **Tratamento de Exceções**: Implemente handlers de exceção global
- **Segurança**: Siga as práticas de segurança OWASP
- **Containerização**: Use Docker para facilitar o deployment

## 🛠️ Recursos Úteis

- [Documentação Oficial do Spring](https://spring.io/docs)
- [Spring Boot Reference Documentation](https://docs.spring.io/spring-boot/docs/current/reference/html/)
- [Baeldung Spring Tutorials](https://www.baeldung.com/spring-tutorial)
- [Spring Guides](https://spring.io/guides)

## 📝 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

## 👥 Contribuições

Contribuições são bem-vindas!.