### Tipos de funções

- ##### Função Regular

Declarando:

```javascript
function calcula(numero){
	return numero*2
}
calcula(2) //retorna 4
```

A definiçao da funcao consiste no uso da palavra chave `function`, em seguida por:

 `Nome da função: calcula`
 `Lista de argumentos entre parênteses: (numero)`
 `Conteudo da função: {  }`
 

- ##### Função Anônima

Declarando:

```javascript
var calcula= function(numero){
	return numero * 2
};

var x = calcula(4) //x retorna o valor 8
```

Diferença entre a **Função Regular** e a **Função Anônima**:

- Função Anônima é declarada dentro de uma variável 


- ##### Arrow function

Declarando: 

```javascript
const mensagem = (nome) => {
	console.log(`Olá, ${nome}!`);
};
	mensagem("Marcelo");
```

