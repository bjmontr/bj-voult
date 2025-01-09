---
title: Relacionamento entre classes
tags:
  - java
  - poo
date: 2025-01-08
---

## 🔍 Definição

Dividir a responsabilidade do código em várias classes diferentes.

---

## 📝 Principais Características

- **Associação**:
	- **Unilateral**: Uma classe conhece i pode acessar a outra, mas não o contrário.
	- **Bilateral**: Ambas as classes se conhecem e podem acessar uma à outra;
- **Agregação**: um tipo especial de associação, onde uma classe é compostas por outras, mas as partem podem existir independente da classe agregadora.
- **Composição**: 

---

## 💻 Exemplo de Implementação

[Link de projeto]([bllakk/LibertyWalk-Java](https://github.com/bllakk/LibertyWalk-Java))

- Classe `Motor`: 
	- Contém a definição da classe `Motor`, com um atributo `tipo` e um método para retornar esse tipo.
```java
// Motor.java
public class Motor {
    private String tipo;

    public Motor(String tipo) {
        this.tipo = tipo;
    }

    public String getTipo() {
        return tipo;
    }
}

```

- Classe `Roda`: 
	- Define a classe `Roda`, que tem um atributo `tamanho` e um método para retornar esse tamanho.
```java
// Roda.java
public class Roda {
    private String tamanho;

    public Roda(String tamanho) {
        this.tamanho = tamanho;
    }

    public String getTamanho() {
        return tamanho;
    }
}

```

- Classe `Carro`: 
	- A classe `Carro` tem um relacionamento de associação com a classe `Motor` e um relacionamento de composição com a classe `Roda`, representando o carro com motor e rodas.
```java
// Carro.java
public class Carro {
    private Motor motor;  // Associação: Carro tem um Motor
    private Roda[] rodas; // Composição: Carro tem várias Rodas

    public Carro(Motor motor, Roda[] rodas) {
        this.motor = motor;
        this.rodas = rodas;
    }

    public void exibirDetalhes() {
        System.out.println("Carro com motor tipo: " + motor.getTipo());
        System.out.print("Rodas: ");
        for (Roda roda : rodas) {
            System.out.print(roda.getTamanho() + " ");
        }
        System.out.println();
    }
}

```

- Classe `Main`:
	- Classe responsável pela execução do programa. Cria instâncias de `Motor` e `Roda`, e então cria um `Carro` usando essas instâncias, exibindo os detalhes do carro.
```java
// Main.java
public class Main {
    public static void main(String[] args) {
        Motor motor = new Motor("V8");  // Exemplo de motor
        Roda[] rodas = {
            new Roda("18 polegadas"),
            new Roda("18 polegadas"),
            new Roda("18 polegadas"),
            new Roda("18 polegadas")
        };  // Exemplo de rodas

        Carro carro = new Carro(motor, rodas);
        carro.exibirDetalhes();
    }
}

```
---

## ⚡ Melhores Práticas

---

## 📚 Referências 

- **Principais temas usados**:
	- [[Construtores]]
	- [[Métodos vs Atributos]]