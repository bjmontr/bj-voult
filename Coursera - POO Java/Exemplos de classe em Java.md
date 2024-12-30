#### Criação de uma classe 

```java
public class Carro {
	int potencia;
	float velocidade;
	String cor;
}
```

#### Criação de um objeto

```java
Carro civic = new Carro();

civic.potencia = 150;
civic.velocidade = 140.5f;
civic.cor = "azul";
```

#### Inserindo métodos

```java
public class Carro {
	int potencia;
	float velocidade;
	String cor;

	void acelerar() {
		velocidade += potencia;
	}
	void frear() {
		velocidade *= 0.5;
	}
}
```

[[O que é void]] -> Lembre-se o do porque usar void.
[[Métodos vs Atributos]] -> Diferença entre método e atributos.