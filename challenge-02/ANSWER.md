# Resolução Desafio da semana #2

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function sum(x, y) {
  return x + y;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var sum = sum(5, 3);

// Qual o valor atualizado dessa variável?
8

// Declare uma nova variável, sem valor.
var value;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function addValue(x) {
  value = x;
  return "O valor da variável agora é " + value;
}

// Invoque a função criada acima.
addValue(10);

// Qual o retorno da função? (Use comentários de bloco).
'O valor da variável agora é 10'

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function multiplyAndAdd2(x, y, z) {
  if (x == null || y == null || z == null) {
     return "Preencha todos os valores corretamente!";
  }
  
  return x * y * z + 2;
}

// Invoque a função criada acima, passando só dois números como argumento.
multiplyAndAdd2(3, 4);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
Como o terceiro argumento não foi passado como parâmetro cai na condição do 'if' então o resultado foi 
"Preencha todos os valores corretamente!"

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
multiplyAndAdd2(3, 4, 5);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
62

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function whatever(x, y, z) {
	if (x ! = null) {
		if ( y != null ) {
			if ( z!= null) {
				return (x + y) / z;
			} 
			return x + y;
		}
		return x;
	}
	return null;
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
whatever(); // retorno null
whatever(3); // retorno 3
whatever(3, 4); // retorno 7
whatever(3, 4, 5); // retorno 1,4

```
