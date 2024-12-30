'## Identificando Classes e Objetos

A classe é algo abstrato -> ao contrário do objeto que é algo concreto -> "produto" Classe -> Cria/Instancia -> Objetos
É possível criar vários objetos diferentes seguindo o modelo da classe.

## Comportamento e Estado das classes

As características de cada objeto são chamadas de atributos da classe. Classes podem realizar ações, e podem mudar os valores dos atributos (características). As ações que um objeto pode realizar são chamadas de métodos.

Classe -> Estado (Atributos) -> Comportamento (Métodos).

### Diferença entre Classe e Objeto

Classe -> Abstrato -> Tem atributos -> Tem ações Objeto -> Concreto -> Tem valores -> Realiza ações

### Exemplo

Classe Carro -> Potência, Motor, Velocidade -> Acelerar, Frear. Objeto Civic -> Potência = 2.0, Velocidade = 150km/h -> Acelerar, Frear.

## Criando Classes

A informação que uma classe precisa saber é armazenada nos atributos -> variáveis.

```java
public class Carro {
	int potencia;
	float velocidade;
}
```

### Criando objetos

`Carro fusca = new Carro();`

Para criar um objeto: 1. Declare o tipo da variável (`Carro`) 2. Sempre use o operador `new`

### Acessando atributos

```java
fusca.potencia = 2;
float v = fusca.velocidade;
```

Os atributos (valores) podem ser acessados para escrita e leitura.

### Comportamento

Os métodos definem o comportamento da classe.

```java
public class Carro {
	void acelerar() {
		velocidade += potencia;
	}
	void frear() {
		velocidade *= 0.5;
	}
}
```

``` java
void acelerar() {
	velocidade += potencia;
}
```

Retorno -> `void` = não retorna nada.
Parâmetro -> `()` -> Pode ter ou não parâmetros.
Manipulação do estado da classe -> `velocidade += potencia;`

#### Executando métodos

```java 
fusca.acelerar();
fusca.frear();
```

O método será executado no objeto utilizado para a chamada.

