---
title: Classe, Associação e Multiplicidade
tags:
  - java
  - poo
date: 2025-08-12
---
[[UML]]
## 📝 Principais Características

- **Classe**:
	- **Definição**:
		Representa uma entidade do sistema, como um objeto no mundo real ou um conceito abstrato.
		
	- **Estrutura**:
		- **Nome**: O nome da classe (obrigatório).
		  
		- **Atributos**: Propriedades ou características da classe.
		  
		- **Métodos**: Comportamentos ou operações que a classe pode realizar.
		  
	- Exemplo:
``` plaintext
---------------------
|    Produto         |
---------------------
| - id: int          |
| - nome: String     |
| - preco: double    |
---------------------
| + calcularDesconto()|
| + exibirDetalhes()  |
---------------------

```

- **Associação**:
	- **Definição**:
		Representa um relacionamento entre duas ou mais classes.
		
	- **Tipos de associação**:
		- **Unilateral**: Apenas uma classe conhece a outra.
		  
		- **Bidirecional**: Ambas as classes têm conhecimento mútuo.
		  
	- **Exemplo**: Um cliente faz pedidos.
```plaintext
Cliente  ---------  Pedido
```

- Multiplicidade
	- Definição:
		Define o número de objetos de uma classe que podem estar associados a um objeto de uma classe.
	- Notação:
		- `1`: Exatamente um
		- `0..1`: Zero ou um
		- `*`: Muitos (0 ou mais)
		- `1..*`: Um ou mais
		- `0..*`: Zero ou muitos
	- Exemplo: Um pedido contém vários produtos, mas cada produto pode estar associado a vários pedidos.
```plaintext
Pedido  1 -------- * Produto
```
---

## 🧩 Vantagens e Desvantagens

- **Vantagens:**
- **Desvantagens:**

---

## 💻 Exemplo de Implementação

---

## ⚡ Melhores Práticas
