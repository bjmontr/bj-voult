---
title: Colaboração, Dependência e Classes Cliente e Servidora
tags:
  - java
  - poo
date: 2025-01-13
---

## 📝 Principais Características

- **Colaboração**:
	- **Tipos de colaboração**:
		- **Associação**: Uma classe pode ter uma referência a outra. Isso indica que as classes estão colaborando, mas de maneira mais flexível, sem forte dependência.
		  
		- **Composição**:
			Uma forma mais forte de associação onde uma classe é parte integrante de outra. Se a classe "pai", for destruída, seus objetos "filhos" também são destruídos.
			
		- **Herança**:
			Uma classe pode herdar comportamentos de outra. Isso permite reutilização de código e colaboração entre as classes de uma hierarquia.
			
		- **Agregação**: 
			Semelhante à composição, mas com uma relação mais fraca. A classe "mãe" depende diretamente da existência da classe "filha", ou seja, objetos podem existir independentemente.
			
		- **Use de interfaces**: 
			Classes podem colaborar por meio de interfaces, onde uma classe complementa uma interface e outras dependem dessa interface para interagir com a classe. Isso permite abstração e flexibilidade na colaboração.
- Exemplo:
```java
class Motor {
    public void ligar() {
        System.out.println("Motor ligado.");
    }
}

class Carro {
    private Motor motor;
    
    public Carro() {
        this.motor = new Motor();
    }
    
    public void ligarCarro() {
        motor.ligar();  // Colaboração entre Carro e Motor
        System.out.println("Carro ligado.");
    }
}

public class Main {
    public static void main(String[] args) {
        Carro carro = new Carro();
        carro.ligarCarro();  // O Carro colabora com o Motor
    }
}
```
A classe Carro colabora com a classe ``Motor`` ao chamar o método ``ligar()`` do Motor dentro do método ``ligarCarro()`` da classe ``Carro``. Isso é um exemplo de associação e delegação de responsabilidades entre as classes,

- **{{Dependência}}**:
	- Tipos de dependência:
		- Dependência de método:
			Uma classe pode depender de outra ao utilizar os métodos desta classe. Ou seja, a classe "A" pode chamar métodos da classe "B" em seus próprios métodos.
```java
class Motor{
	public void ligar(){
		System.out.println("Motor ligado.");
	}
}

class Carro {
	private Motor motor;
	
	public Carro(Motor motor){
		this.motor = motor;
	}
	
	public void ligarCarro(){
		motor.ligar();
		System.out.println("Motor ligado.");
	}
}
```

---

## 🧩 Vantagens e Desvantagens

- **Vantagens:**
- **Desvantagens:**

---

## 💻 Exemplo de Implementação

---

## ⚡ Melhores Práticas
