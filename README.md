# Módulo 4 de NodeJS Rocket-Seat

Esse módulo é um estudo de Design Dirigido à Domínio. O DDD não diz respeito à implementação e ao código em si, mas sim às entidades e casos de uso que moldam a aplicação.

+ Domain Experts: Pessoas que entendem a fundo o problema que deve ser resolvido. São pessoas que lidam no dia a dia com esse problema.
  > É necessária a conversa

+ Linguagem ubíqua: Linguagem que pode ser entendida por todas as pessoas dialogando sobre o problema a ser resolvido.
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

## Conteúdo Programático do Módulo 4:

<details style="font-size: 16px">
<summary><strong style="font-size: 18px">1. Submod 1</strong></summary>

  ---

  + Aula 1
  + Aula 2

  ---
</details>

## Principais comandos:

### Aula "Entidades e Casos de Uso"

+ `npm init -y` : cria o package.json para iniciar o projeto NodeJS.
+ `npm i typescript @types/node -D` : instala o typescrit, o types/node e o tsx, responsável por converter .ts para .js. O tsup é a biblioteca que cria a versão de build.
+ `npx tsc --init`: executa o arquivo binário tsc dentro de ./node_modules/.bin/ para criar o arquivo tsconfig.json.
  > **_OBS1:_**  Mudar "target" para "es2020" dentro do tsconfig.json.

### Aula "Primeiro caso de uso"

+ `npm i vitest -D` : Instala a ferramenta de testes vitest como dependência de desenvolvimento.
+ `npx vitest run` : Roda os testes definidos nos arquivos com extensão .spec.ts.

## Autoria e Créditos:

+ Documentação criada com carinho e dedicação por [Júlio César Freitas](https://github.com/juliofreitasbm) a serviço do [CREA-GO](https://www.creago.org.br/).