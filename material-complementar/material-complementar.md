# O básico de JavaScript

## Olá, mundo

Começaremos com o tradicional `Olá, mundo!`.

Digite a linha de código abaixo no Code Editor:

```javascript
print('Olá, mundo!');
```

Clique em Run ou utilize as teclas Ctrl + Enter para executar o código.

Observe que o texto `Olá, mundo!` será mostrado - ou “printado” - no Console, no painel à direita. O comando `print()` tem essa função: mostrar algo no Console.

Pode ser um texto, o conteúdo de uma variável, as propriedades de uma imagem ou o resultado de uma análise mais complexa. O importante é entender que o `print()` não adiciona informações no mapa.

Na linguagem JavaScript, as instruções são chamadas de declarações, e são delimitadas por um ponto e vírgula `;`.

## Comentários

Podemos utilizar barras duplas `//` para criar comentários no script, ou para “ignorar” a execução de determinada linha sem que haja a necessidade de deletá-la.

Os comentários também podem ser utilizados no processo de depuração do código, ou _debug_.

```javascript
// print('Olá, mundo!');
```

Além das barras duplas, podemos criar comentários utilizando a notação `/* */`, veja no código abaixo:

```javascript
// Comentário utilizando barras duplas

/*
  Comentário utilizando a notação asterisco-barra.
  Geralmente esta notação é utilizada em comentários com mais de uma linha.
*/
```

Os comentários também possibilitam que você mantenha seu código bem documentado:

```javascript
print('Olá, mundo!'); // Mostra o texto 'Olá, mundo!' no console
```

## Tipos básicos de dados JavaScript

### Strings

Strings são cadeias de caracteres delimitadas por um par de aspas simples `''` ou duplas `""`. Por exemplo:

```javascript
var var1 = 'Olá, eu sou uma string!';
print(var); 

var var2 = "Olá, eu também sou uma string!";
print(var2);
```

Evite misturar os tipos de aspas. Escolha um dos tipos e escreva seu código.

### Variáveis

Imagine que as variáveis são “caixas” nas quais podemos armazenar alguma informação. 
No exemplo acima, temos duas “caixas” - as variáveis `var1` e `var2` - onde armazenamos duas strings: 
`'Olá, eu sou uma string!'` e `"Olá, eu também sou uma string!"`, respectivamente.

### Números

Os números podem ser inteiros ou números reais:

```javascript
var numeroInteiro = 42;
print('Número inteiro: ', numeroInteiro); 

var numeroReal = 4.2;
print('Número real: ', numeroReal);
```

### Listas

Podemos criar listas utilizando colchetes `[]`:

```javascript
var listaDeNumeros = [1,2,3,4,5];
print('Lista de números: ', listaDeNumeros);

var listaDeString = ['a', 'b', 'c', 'd', 'e'];
print('Lista de string: ', listaDeString);
```

### Dicionários

Na linguagem JavaScript, dicionários são dados do tipo chave:valor. Podemos criar um dicionário utilizando chaves `{}`:

```javascript
var dicionario = {
  nome: 'João',
  idade: 25
};

print('Meu dicionário: ', dicionario);

// Selecionando uma key (chave) específica utilizando colchetes
print('Meu nome é: ', dicionario['nome']);
print('Minha idade é: ', dicionario['idade']);

// Selecionando uma key (chave) específica utilizando a notação
// de ponto (dot notation)
print('Meu nome é: ', dicionario.nome); // Meu nome é: João
```

### Funções

Uma função é um agrupamento de declarações que podem ser utilizadas para realizar uma tarefa específica. 
Na API JavaScript do GEE, as funções podem ser criadas das seguintes maneiras:

```javascript
var minhaFunção = function(parâmetro1, parâmetro2){
  declaração;
  declaração;
  return declaração;
};

// Ou...
function minhaFunção (parâmetro1, parâmetro2){
  declaração;
  declaração;
  return declaração;
}
```

Uma função é definida pelo termo `function`, e pode ou não conter parâmetros. Esses, quando houverem, vão dentro dos parênteses `()`.
O conjunto de declarações vai dentro dos colchetes `{}`.
O termo `return` diz respeito ao resultado que teremos ao executar a função.

Por exemplo, vamos criar uma função que retorne a soma de dois números, `n1` e `n2`. O nome da função será `adicione`:

```javascript
// Criando a função
var adicione = function(n1, n2){
  return n1 + n2;
};

// Chamando a função
var soma = adicione(1, 2);

// Inspecionando o resultado
print('Resultado: ', soma); // Resultado: 3
```
