---
title: Resumo semana 2 - Aprofundamento de classes e CRC
tags:
  - java
  - poo
date: 2025-01-06
---
 
## 📖 Tópicos Estudados  

### 🧩 1. Relacionamento entre classes

[[Relacionamento entre classes]]

 - **Conceito**:
	 - Dividir o códigos em varias classes, é uma boa prática dividir a responsabilidade do código em varias classes para posteriormente ajudar na manutenção.
		
	 - **Exemplo**:
		 Uma pizzaria precisa calcular o valor de cada sabor de pizza, e precisa calcular o valor da entrega.
		 Para isso iriamos ter as seguintes classes:
		 - `class Pizza`: Calcular o preço baseado nos ingredientes da pizza.
		 - `class Entrega`: Calcula a entrega baseado no dia da semana e na distância.
		 - `class Carrinho`: Calcula o valor total da compra com as pizzas e a entrega.
	
	Com esse conceitos iremos ter um código mais fácil de ler, de fazer manutenções e mais leve.

---

### 🧩 2. Pensando em métodos orientados a objetos

- **Programação estruturada**: 
	- As funções recebem o parâmetro para retornar um valor com base no que recebeu.
	- Também pode ter variáveis globais que a função também pode acessar.
- **Programação orientada a objetos**:
	- Temos uma classe, com base nessa classe criamos objetos, passamos parâmetros e parametrizar objetos.
	- Não significa do os objetos da mesma classe irá funcionar da mesma forma.
	- Um objeto executa seus métodos com base nos parâmetros recebidos e em dados internos.

---

### ✅ **Tarefas e Metas da Semana**

- [x] Atividade ✅ 2025-01-09 [Link de projeto]([bllakk/LibertyWalk-Java](https://github.com/bllakk/LibertyWalk-Java))
