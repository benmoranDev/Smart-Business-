Smart Business


Plataforma SaaS de gestão empresarial voltada para micro e pequenas empresas (MPEs), desenvolvida no contexto do curso de Engenharia de Computação.

## Descrição

O **Smart Business** é um sistema web de gestão empresarial que centraliza operações administrativas essenciais em um único ambiente digital. A proposta da plataforma é reduzir a complexidade da rotina de micro e pequenos negócios, oferecendo controle de clientes, produtos, vendas, estoque, financeiro e indicadores gerenciais em uma aplicação integrada.

O sistema foi pensado para apoiar empreendedores que ainda enfrentam dificuldades com processos manuais, falta de organização operacional e pouca visibilidade sobre o desempenho do negócio. Dessa forma, a plataforma busca melhorar a tomada de decisão, a produtividade e a sustentabilidade da empresa.

## Objetivo

Desenvolver uma plataforma SaaS que permita:

- Centralizar a gestão empresarial.
- Automatizar processos operacionais.
- Organizar informações de clientes, produtos, vendas e finanças.
- Fornecer indicadores para apoio à tomada de decisão.
- Reduzir a complexidade da gestão para pequenos negócios.

## Funcionalidades principais

- Cadastro e gestão de clientes.
- Cadastro e controle de produtos.
- Controle de estoque.
- Registro de vendas.
- Módulo de PDV (caixa).
- Controle financeiro com receitas e despesas.
- Dashboard com indicadores gerenciais.
- Histórico de vendas.
- Registro de forma de pagamento e troco.
- Alertas de estoque baixo.
- Precificação assistida.
- Gestão de usuários.
- Cadastro de empresa.

## Arquitetura

O sistema segue uma arquitetura em camadas, com separação clara entre apresentação, regras de negócio e persistência de dados.

### Camadas da aplicação

- **Frontend:** Thymeleaf, HTML5, CSS3, JavaScript, Bootstrap.
- **Backend:** Java + Spring Boot.
- **Persistência:** Spring Data JPA / Hibernate.
- **Banco de dados:** PostgreSQL.
- **Segurança:** Spring Security.
- **Build e gerenciamento de dependências:** Maven.

## Tecnologias utilizadas

### Backend

- Java
- Spring Boot
- Spring Web
- Spring Data JPA
- Spring Security
- Thymeleaf
- Thymeleaf Extras Spring Security
- Hibernate
- Bean Validation

### Frontend

- HTML5
- CSS3
- JavaScript
- Thymeleaf
- Bootstrap
- Bootstrap Icons

### Banco de dados

- PostgreSQL

### Ferramentas e infraestrutura

- Maven
- Git
- GitHub

## Dependências do projeto

Com base na estrutura atual da aplicação, o projeto utiliza ou está preparado para utilizar dependências como:

- `spring-boot-starter-web`
- `spring-boot-starter-thymeleaf`
- `spring-boot-starter-data-jpa`
- `spring-boot-starter-security`
- `thymeleaf-extras-springsecurity6`
- `postgresql`
- `spring-boot-starter-validation`
- `spring-boot-devtools` (em ambiente de desenvolvimento)
- `lombok` (caso esteja sendo usado nas entidades/DTOs)

> Ajuste esta lista conforme o seu `pom.xml`, caso existam dependências adicionais já incluídas no projeto.

O fluxo principal do Smart Business integra diferentes módulos da aplicação:

1. Uma venda é registrada no sistema.
2. Os itens vendidos são processados no módulo de vendas/PDV.
3. O estoque é atualizado conforme a quantidade vendida.
4. A forma de pagamento é registrada.
5. O valor recebido e o troco podem ser armazenados na venda.
6. As informações ficam disponíveis para histórico, acompanhamento e relatórios.

## Segurança

O sistema conta com recursos de segurança aplicados na camada web:

- Autenticação de usuários com Spring Security.
- Controle de acesso por perfil.
- Proteção de rotas e menus por autorização.
- Integração com Thymeleaf Extras para controle de exibição no frontend.
- Proteção contra CSRF em formulários.

## Público-alvo

- Microempreendedores individuais (MEI)
- Pequenos comércios
- Prestadores de serviço
- Restaurantes
- Negócios locais em geral

## Status do projeto

Em desenvolvimento. O sistema está evoluindo de forma incremental, com foco em módulos centrais como cadastro, vendas, PDV, estoque, financeiro e dashboard administrativo.

## Licença

Este projeto está licenciado sob a **MIT License**.

## Equipe

Projeto desenvolvido no contexto do curso de Engenharia de Computação.

Estrutura do projeto

/backend
/frontend
/docs
/docker

---

Status

Em desenvolvimento. MVP em construção conforme roadmap definido no projeto.

---

Licença

Este projeto está licenciado sob a MIT License.

---

Equipe

Projeto desenvolvido por equipe de Engenharia de Computação (UNIVESP).

---
