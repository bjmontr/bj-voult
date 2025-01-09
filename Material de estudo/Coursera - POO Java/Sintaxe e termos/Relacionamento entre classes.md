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

```java
public class Pessoa {
	private String nome;
	private int idade; 
 // Construtor
	 public Pessoa(String nome, int idade) {
		this.nome = nome; this.idade = idade; 
	} 
	// Métodos getters 
public String getNome() {
	 return nome; } 
	 public int getIdade() { 
	 return idade; 
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