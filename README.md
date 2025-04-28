# ToDo! - Projeto Inicial para SSR MPA

Este projeto é um template inicial para uma aplicação ToDo, projetado para fins educacionais em ambientes de sala de aula. Ele demonstra o uso do padrão de design **MVC** (Model-View-Controller), renderização no lado do servidor (SSR) e o conceito de aplicação multi-página (MPA).

## Estrutura do Projeto

O projeto está organizado de acordo com o padrão MVC, com os seguintes componentes:

- **Model (Modelo)**: Gerencia a lógica de negócios e a interação com o banco de dados.
  - Localizado em `src/models/`.
  - Arquivos principais: `model.ts`, `database.ts`, `config.ts`.

- **View (Visão)**: Gerencia a interface do usuário.
  - Localizado em `views/`.
  - Utiliza templates Handlebars para renderizar as páginas.

- **Controller (Controlador)**: Atua como intermediário entre o modelo e a visão.
  - Localizado em `src/controllers/`.
  - Atualmente inclui um placeholder para lógica de ordenação em `sorting.ts`.

## Funcionalidades Atuais

Este projeto inicial inclui:

- Configuração básica do servidor usando Express.
- Servir arquivos estáticos do diretório `static/`.
- Integração com Handlebars para renderização no lado do servidor.
- Configuração de conexão com banco de dados usando a classe `Database`.

## Funcionalidades Ausentes

Este projeto é um ponto de partida e ainda não inclui as seguintes funcionalidades:

- Rotas para manipulação de operações ToDo.
- Lógica completa dos controladores.
- Visões totalmente implementadas.

## Estrutura de Arquivos

```plaintext
src/
├── server.ts              # Ponto de entrada da aplicação
├── controllers/           # Controladores (C no MVC)
│   └── sorting.ts         # Placeholder para lógica de ordenação
├── models/                # Modelos (M no MVC)
│   ├── model.ts           # Repositório de dados e lógica
│   ├── database.ts        # Conexão com o banco de dados
│   ├── config.ts          # Configurações
static/                    # Arquivos estáticos (CSS, imagens, etc.)
├── style.css              # Estilos personalizados
├── bootstrap.min.css      # Estilos do Bootstrap
views/                     # Visões (V no MVC)
├── base.html              # Template base HTML
package.json               # Configuração do projeto Node.js
tsconfig.json              # Configuração do TypeScript
README.md                  # Documentação do projeto
```

## Tecnologias Utilizadas

- **Node.js**: Ambiente de execução JavaScript.
- **Express**: Framework para servidores web.
- **Handlebars**: Motor de templates para renderização de visões.
- **TypeScript**: Superset tipado do JavaScript.

## Como Usar

1. Clone este repositório.
2. Execute `npm install` para instalar as dependências.
3. Inicie o servidor de desenvolvimento com `npm run dev`.
4. Acesse a aplicação em `http://localhost:3000`.

## Notas

Este projeto é destinado a fins educacionais e não é uma aplicação completa. Os alunos são esperados a implementar as funcionalidades ausentes como parte do processo de aprendizado.


