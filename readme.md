# TypeScript

## Introdução

**Typescript** é um superconjunto javascript, que adiciona anotações de tipagens e outros recursos tais como interfaces, classes e namescapes.

## Instalar e connfigurar o typescript

Para instalar e configurar o typescript, você deve realizar os seguintes passos:

- inicialize o npm no diretório do seu projecto executando o comando:

```bash
npm init
```

- instale o typescript como uma dependência do projecto executando o comando:

```bash
  npm install --save-dev typescript
```

-crie um arquivo **tsconfig.json** no diretório do seu projeto para especificar as opções do compilador para construir seu projeto. Por exemplo:

```json
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "strict": true,
    "outDir": "./dist",
    "rootDir": "./src"
  },

  "exclude": ["node_module"]
}
```

## Executando Javascript

Para executar o código typescript, você deve executar os seguintes passos:

- Escrever um código typescript em um **arquivo .ts**
- Compilar o código typescript usando o compilador (tsc)

```bash
tsc index.ts
```

- executar o código javascript usando um ambiente de desenvolvimento javascript (nodejs por exemplo);

### tsc

**tsc** é uma ferramenta de linha de comando para o compilador typescript. Ele compila o código typescript em código javascript, tornando-o compatível com os navegadores e qualquer outro ambiente de execução javascript.

### node-ts

É um mecanismo execução typscript e REPL node, com mapa de origem e suporte ESM nativo.
