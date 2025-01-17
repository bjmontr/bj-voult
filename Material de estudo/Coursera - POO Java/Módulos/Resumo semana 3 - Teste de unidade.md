---
title: Resumo semana 3 - Teste de unidade
tags:
  - java
  - poo
date: 2025-01-09
---

## 📖 Tópicos Estudados  

### 🧩 1. Importância de testes automatizados

[[Teste unitário]]

- **Importância**:
	Vamos supor que tenhamos a classe A, logo iremos testar a classe A, em seguida foi criado a classe B, teremos que testar a classe B e em seguida testar a classe A, pois talvez a classe B tenha influenciado no código da classe A.

- **Tipos de testes**:
	- **Unidade**:
		- Testa uma única classe ou um único método.
		
	- **Integração**:
		- Testa a colaboração de um grupo de classes.
		
	- **Funcional**:
		- Testa o software como um todo de acordo com os requisitos.
		
- **Antes e depois dos testes**:
	Para tornar nossos testes mais limpos e organizados, podemos utilizar métodos como `@BeforeAll`, `@BeforeEach`, `@AfterEach` e `@AfterAll`. Esses métodos ajudam a estruturar melhor o código, configurando o ambiente de teste de forma eficiente e garantindo uma limpeza adequada após a execução. Com isso, os testes se tornam mais legíveis, reutilizáveis e fáceis de manter.
	
	- **Exemplo**:
		Vamos realizar um teste de um CRUD com um banco.
		
		1. `@beforeAll`: Abrir uma conexão com o banco.
		2. `@beforeEach`: Adicionar dados padrão, como um usuário ou produto.
		3. `@test`: Adicionar, buscar e remover itens no banco. 
		4. `@afterEach`: Apagar os registros criados 
		5. `@afterAll`: Fechar a conexão com o banco.

---
### 🧩 2. UML - Classe, Associação e Multiplicidade

[[UML]]
[[Visibilidade]]
[[Classe, Associação e Multiplicidade]]

- **Classe**:
	- **Definição**:
		Representa uma entidade do sistema, como um objeto no mundo real ou conceito abstrato.
		
- **Associação**:
	- **Definição**:
		Representa um relacionamento entre duas ou mais classes.
		
- **Multiplicidade**
	- **Definição**:
		Define o número de objetos de uma classe que podem estar associados a um objeto de outra classe.

---
### 🧩 3. UML - # Colaboração, Dependência e Classes Cliente e Servidora

[[Colaboração, Dependência e Classes Cliente e Servidora]]

- Colaboração:
	- Definição:
		É interação entre diferentes classes para alcançar um objetivo comum. Isso envolve o uso de métodos e atributos de uma classe por outras, onde uma classe pode delegar parte do seu comportamento ou lógica para outra, a fim de realizar uma tarefa específica.
		
- Dependência:
	- Definição:
		É uma relação em que uma classe utiliza outra para realizar suas funções ou operações. Quando uma classe depende de outra, isso significa que ela precisa de um ou mais objetos da outra classe para executar seu comportamento ou lógica.
		
- Classe cliente e classe servidora:
	- Definição:
		É a relação funcional entre duas classes. Essa terminologia é usada para descrever como as classes interagem umas com as outras, geralmente em contextos onde uma classe utiliza os serviços ou funcionalidades por outras.
---
### ✅ **Tarefas e Metas da Semana**

- [ ] Tarefa 1
- [ ] Tarefa 2
- [ ] Tarefa 3
- [ ] Tarefa 4

### 💡 **Observações e Insights**

- {{Observação}}
- {{Observação}}

