---
title: "{{title}}" # Substituído pelo título da nota
date: {{date}} # Data de criação automática
tags: #exemplo, #estudo, #materia
---
# Semana {{número da semana}}

## 🗓 Resumo da Semana  
Adicione aqui um breve resumo dos tópicos estudados e o que foi mais importante.  

---

## 📖 Tópicos Estudados  

### 🧩 1. Identificando Classes e Objetos  
- **Conceito:**  
  Classe é algo abstrato, enquanto o objeto é concreto.  
  Exemplo: Classe "Produto" → Objeto "Produto específico".  
- **Observações:**  
  É possível criar vários objetos diferentes seguindo o modelo de uma classe.  

---

### 🧩 2. Comportamento e Estado das Classes  
- **Conceitos:**  
  - Atributos representam as características do objeto.  
  - Métodos representam as ações realizadas pelo objeto.  
  - Relação: Classe → Estado (Atributos) → Comportamento (Métodos).  
- **Exemplo:**  
  Classe: Carro → Atributos: Potência, Velocidade → Métodos: Acelerar, Frear.  

---

### 🧩 3. Diferença entre Classe e Objeto  
| Classe         | Objeto                   |
| -------------- | ------------------------ |
| Abstrato       | Concreto                 |
| Tem atributos  | Tem valores específicos  |
| Define métodos | Executa métodos          |

---

### 🧩 4. Criando Classes e Objetos  
- **Classes:**  
  ```java
  public class Carro {
      int potencia;
      float velocidade;
  }```

- **Objetos**: 
```java
	Carro fusca = new Carro(); 
```
- Passos para criar um objeto:
	1. Declare o tipo da variável (`Carro`).
	2. Use o operador `new` para instanciar.

---

### 🧩 5. Tópico

- **O que é?**
Métodos especiais usados para instanciar objetos.

- **Exemplo:**
```java
public class Carro {
	String marca;
	int ano;

	Carro(String marca, int ano){
		this.marca = marca;
		this.ano = ano;
	}
}
```

- O construtor não tem retorno e tem o mesmo nome da classe.

---

### ✅ **Tarefas e Metas da Semana**

- [ ] Tarefa 1
- [ ] Tarefa 2
- [ ] Tarefa 3
- [ ] Tarefa 4

### 💡 **Observações e Insights**

- {{Observação}}
- {{Observação}}

