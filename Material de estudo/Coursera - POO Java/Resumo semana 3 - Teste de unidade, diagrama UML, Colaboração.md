---
title: Resumo semana 3 - Teste de unidade, diagrama UML, Colaboração
tags:
  - java
  - poo
date: 2025-01-09
---

## 📖 Tópicos Estudados  

[[Teste unitário]]
### 🧩 1. Importância de testes automatizados

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
---

### 🧩 2. Diagramas 

Diagramas permitem ter uma visão geral do software como um todo, e não apenas de uma pequena parte dele, além de que é possível explicar o software de uma forma mais simples.

- **Diagrama de classes**:
	- Como uma classe é representada

|  Nome   |
| --- |
|  Atributos   |
|  Operações ou métodos   |

- Visibilidade:
	- - -> Privado
	- '#' -> Protegido
	- + -> Público

- Exemplo:

| Carro                     |
| ------------------------- |
| -nome                     |
| '#'getNome<br>+trocarNome |

---

### 🧩 3. {{Tópico}}  


---

### 🧩 4. {{Tópico}}  


---

### 🧩 5. {{Tópico}}


---

### ✅ **Tarefas e Metas da Semana**

- [ ] Tarefa 1
- [ ] Tarefa 2
- [ ] Tarefa 3
- [ ] Tarefa 4

### 💡 **Observações e Insights**

- {{Observação}}
- {{Observação}}

