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

- **Otimização do código**: Com a divisão das responsabilidades o código ficará menos bagunçado e mais legível.

---

## 💻 Exemplo de Implementação

[Link do código]([bllakk/LibertyWalk-Java](https://github.com/bllakk/LibertyWalk-Java))

- Classe `Motor`
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
```java
public class Endereco {
private String rua; 
private String cidade; 
	public Endereco(String rua, String cidade) {
		this.rua = rua;
		this.cidade = cidade; 
	} 
	public String getRua() {
		return rua; 
	} 
	public String getCidade() {
		return cidade; 
	} 
}
```

- Classe `Main`:
```java
public class Main { public static void main(String[] args) {
	Pessoa pessoa = new Pessoa("João", 30);
	Endereco endereco = new Endereco("Rua das Flores", "São Paulo"); 
	Cadastro cadastro = new Cadastro(pessoa, endereco); 
	cadastro.mostrarCadastro(); 
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