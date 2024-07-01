# Módulo 4 de NodeJS Rocket-Seat

Esse módulo é um estudo de Design Dirigido à Domínio. O DDD não diz respeito à implementação e ao código em si, mas sim às entidades e casos de uso que moldam a aplicação. Ele trata de converter os problemas do mundo real para uma linguagem de domínio.
  > DDD é com conceito desconexo de Arquitetura de Software, pois na Arquitetura de Software já é trabalhada a parte ferramental, de linguagem de programação, da estrutura do projeto, etc.

+ Domínio: Área de entendimento, área de conhecimento que engloba os processos e comportamentos essenciais para o negócio.

+ Domain Experts: Pessoas que entendem a fundo o problema que deve ser resolvido. São pessoas que lidam no dia a dia com esse problema.
  > Conversar é uma das melhores formas de entender quais são os problemas dos experts.

+ Linguagem ubíqua: Linguagem universal que pode ser entendida por todas as pessoas dialogando sobre o problema a ser resolvido.
  > Nomenclaturas utilizadas pelos desenvolvedores nem sempre são as mesmas utilizadas pelos Domain Experts. Exemplo: usuário (cliente, fornecedor, atendente, barman)

+ Agregados

+ Value Objects

+ Eventos de domínio

+ Subdomínios (Bounded Contexts)

+ Entidades

+ Casos de uso

___
### Palavras chave:
>Domain-driven Design (DDD), Domain Experts, Linguagem ubíqua

### Glossário sobre DDD:

>Pode ser acessado através [dessa página](https://efficient-sloth-d85.notion.site/Gloss-rio-DDD-3a81b4df36d348a299ccbc53f38a1665) no Notion.

## Conteúdo Programático do Módulo 4:

<details style="font-size: 16px">
<summary><strong style="font-size: 18px">1. Fundamentos do DDD</strong></summary>

  ---

  + Design de software e DDD
  + Entidades e casos de uso
  + Primeiro caso de uso
  + Mapeando relacionamentos
  + Value Object de slug
  + Classe base de entidades
  + Classe base de entidades
  + ID das entidades
  + Mapeando propriedades
  + Abstraindo criação de entidades
  + Getters & Setters das entidades
  + Path aliases e Vitest globals

  ---
</details>

<details style="font-size: 16px">
<summary><strong style="font-size: 18px">2. Fórum com DDD & Clean Architecture</strong></summary>

  ---

  + Configuração do ESLint
  + Fundamentos de Clean Architecture
  + Refatorando as pastas
  + Caso de uso: Criar pergunta
  + Refatorando os teste unitários
  + Caso de uso: Buscar pergunta pelo slug
  + Factories de testes
  + Gerando dados fictícios
  + Caso de uso: Deletar pergunta
  + Caso de uso: Deletar resposta
  + Caso de uso: Editar pergunta
  + Caso de uso: Editar resposta
  + Caso de uso: Escolher melhor resposta
  + Caso de uso: Listar perguntas recentes
  + Caso de uso: Listas respostas da pergunta
  + Entidades de comentários
  + Classe base de comentários
  + Caso de uso: Comentar na pergunta
  + Caso de uso: Comentar na resposta
  + Caso de uso: Deletar comentário da pergunta
  + Caso de uso: Deletar comentário da resposta
  + Caso de uso: Listar comentários da pergunta
  + Caso de uso: Listar comentários da resposta

  ---
</details>

<details style="font-size: 16px">
<summary><strong style="font-size: 18px">3. Functional Error Handling</strong></summary>

  ---

  + Problemas com Error Handling
  + Functional Error Handling
  + Testando classes de erro
  + Criando erros genéricos
  + Refatorando casos de uso
  + Refatorando testes unitários

  ---
</details>

<details style="font-size: 16px">
<summary><strong style="font-size: 18px">4. Aggregates & Watched Lists</strong></summary>

  ---

  + Aggregates & Watched Lists
  + Classe base de AggregateRoot
  + Entidades de anexo
  + Criando pergunta com anexos
  + Pattern: WatchedList
  + Editando pergunta com anexos
  + Teste de edição da pergunta
  + Excluindo anexos da pergunta
  + Anexos nas respostas

  ---
</details>

<details style="font-size: 16px">
<summary><strong style="font-size: 18px">5. Subdomínios & Domain Events</strong></summary>

  ---

  + Fundamentos de subdomínios
  + Entidade de notificação
  + Caso de uso: envio de notificação
  + Caso de uso: ler notificação
  + Fluxo de eventos de domínio
  + Estrutura de eventos de domínio
  + Testando eventos de domínio
  + Evento: Resposta criada
  + Ouvindo um evento de domínio
  + Enviando notificação no subscriber
  + Fluxo de melhor resposta

  ---
</details>

### Atalhos do VSCode:

>Clique para visualizar os [Atalhos do VSCode](https://silicon-chips-f58.notion.site/VsCode-Shortcuts-Atalhos-4ced0388660c4f1c93b410765c0a44cd) no Notion.

## Principais comandos:

### Aula "Entidades e Casos de Uso"

+ `npm init -y` : cria o package.json para iniciar o projeto NodeJS.
+ `npm i typescript @types/node -D` : instala o typescrit, o types/node e o tsx, responsável por converter .ts para .js. O tsup é a biblioteca que cria a versão de build.
+ `npx tsc --init`: executa o arquivo binário tsc dentro de ./node_modules/.bin/ para criar o arquivo tsconfig.json.
  > **_OBS1:_**  Mudar "target" para "es2020" dentro do tsconfig.json.

### Aula "Primeiro caso de uso"

+ `npm i vitest -D` : Instala a ferramenta de testes vitest como dependência de desenvolvimento.
+ `npx vitest run` : Roda os testes definidos nos arquivos com extensão .spec.ts.

### Aula "Dependências externas"

+ Scripts de teste para colocar no arquivo package.json:
  ```
  "scripts": {  
    "test": "vitest run",
    "test:watch": "vitest"
  },
  ```

### Aula "Getters & Setters das entidades"

+ `npm i dayjs` : Biblioteca para lidar com datas.

### Aula "Path aliases e Vitest globals"

+ `npm i vite-tsconfig-paths` : Permite utilizar os "@" nas importações.

### Aula "Configuração do ESLint"

+ `npm i eslint @rocketseat/eslint-config -D` : Instala o ESLint com a configuração da rocketseat.
+ Alteração nos scripts do package.json
  ```
  "scripts": {
    "test": "vitest run",
    "test:watch": "vitest",
    "lint": "eslint src --ext .ts",
    "lint:fix": "eslint src --ext .ts --fix"
  },
  ```
+ `npm i eslint-plugin-vitest-globals -D` : Plugin para permitir que o ESLint reconheça algumas funções do vitest declaradas globalmente.

### Aula "Refatorando as pastas"

+ Dica: Colocar a configuração `"explorer.compactFolders": false` no settings.json do VScode para melhorar a visualização das pastas.

### Aula "Gerando dados fictícios"

+ `npm i @faker-js/faker -D`: Biblioteca para gerar dados aleatórios.

## Autoria e Créditos:

+ Documentação criada com carinho e dedicação por [Júlio César Freitas](https://github.com/juliofreitasbm) a serviço do [CREA-GO](https://www.creago.org.br/).