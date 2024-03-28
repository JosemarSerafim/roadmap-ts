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

## Tipagem em typescript

O javascript tem 3 primitivas comumente muito utilizadas: **string**, **number** e **boolean**. E cada uma tem a sua correspondência em typescript.

## Tipos Primitivos

### boolean

É um tipo de dados primitivo typescript que representa um valor booleano, ou seja, verdadeiro ou falso.

```typescript
let isTrue: boolean = true;
let isFalse: boolean = false;
```

### number

é um tipo de dado primitivo do typescript que representam valores numéricos. Inclui valores inteiros e de pontos flutuantes.

```typescript
let intValue: number = 23;
let floatValue: number = 3.14;
```

### string

É um tipo de dado primitivo em typescript que representa dados textuais.

```typescript
let name: string = "Josemar Serafim";
```

### void

Repreenta o valor de retorno de funções que não retornam um valor.

```typescript
function teste(){
  return;
}
```

### undefined e null

Valores usado para identificar valores ausentes ou não inicializados.

```typescript
function doSomething(value: string | null){
  if(value == null) {
    //dosomething
  } else {
    console.log("value: ", value.toUpperCase());
    
  }
}
```

## Tipos Objectos

### Interface

É o modo de declarar o comportamento de uma classe,

```typescript
interface Person {
  name: string;
  age: number
}

function greet(person: Person){
  return "Hello " + person.name
}
```
