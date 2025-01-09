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
	
- **Agregação**: Um tipo especial de associação, onde uma classe é compostas por outras, mas as partem podem existir independente da classe agregadora.

- **Composição**: É uma forma mais forte de agregação, onde as partes não podem existir sem o todo.

- **Herança**: Quando uma classe herda características e comportamentos de outra. A classe que herda é chamada de "subclasse", e a classe que é herdada é chamada de "superclasse".

- **Dependência** Quando uma classe usa outra para realizar suas funções, geralmente temporariamente, como no caso de um método que recebe um parâmetro de outra classe.

---

## 🧩 Vantagens e Desvantagens

- **Vantagens:**
	- **Reutilização de código**: você pode reutilizar o código de outras classes, evitando duplicação e facilitando a manutenção.
	  
	- **Facilidade de manutenção**: Relacionamentos bem definidos permitem que modificações em uma classe tenham impacto mínimo nas outras.
	  
	- **Encapsulamento**: Relacionamentos ajudam a definir limites claros entre as responsabilidades das classes, promovendo a separação de preocupações e melhorando a modularidade.
	  
	- **Facilidade em adicionar novas funcionalidades**: Usando herança e composição, você pode adicionar novas funcionalidades sem modificar as classes existentes.
	
- **Desvantagens:**
	- **Complexidade**: Relacionamentos entre classes podem aumentar a complexidade do código, tornando-o difícil de entender e manter, especialmente em sistemas grandes e mal projetados.
	  
	- **Acoplamento**: Se o relacionamento entre as classes for muito forte (como na composição), isso pode aumentar o acoplamento, tornando o sistema mais difícil de modificar e testar.
	  
	- **Herança excessiva**: O uso indevido da herança pode levar a hierarquias profundas e difíceis de entender, além de tornar a modificação de classes superclasses mais arriscada.
	  
	- **Desempenho**: O uso de certos tipos de relacionamentos, como a composição, pode causar um pequeno overhead de desempenho, dependendo de como os objetos são gerenciados.

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

- **Favor composição à herança**: Em muitos casos, a composição (ao invés da herança) pode ser uma solução mais flexível, pois evita a rigidez e o alto acoplamento da herança.
- Mantenha o baixo acoplamento:
- Use interfaces e classes abstratas
- Princípio de responsabilidade 

---

## 📚 Referências 

- **Principais temas usados**:
	- [[Construtores]]
	- [[Métodos vs Atributos]]