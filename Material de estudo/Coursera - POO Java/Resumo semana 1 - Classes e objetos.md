---
title: Resumo semana 1 - Classes e objetos
tags:
  - "#poo"
  - java
date: 2024-12-23
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

[[Métodos vs Atributos]]

- **Conceitos:**
    - Atributos representam as características do objeto.
    - Métodos representam as ações realizadas pelo objeto.
    - Relação: Classe → Estado (Atributos) → Comportamento (Métodos).
- **Exemplo:**  
    Classe: Carro → Atributos: Potência, Velocidade → Métodos: Acelerar, Frear.
    
```java
    public class Carro {
	void acelerar() {
		velocidade += potencia;
	}
	void frear() {
		velocidade *= 0.5;
	}
}
```

- **Estrutura**
	- Retorno
		- `void` = não retorna nada.
		-  [[O que é void]]
	- Parâmetro
		- `()` = Pode ter ou não parâmetros.

- **Executando métodos:**

```java
civic.acelerar();
civic.frear();
```

---

### 🧩 3. Diferença entre Classe e Objeto  

| **Classe**     | **Objeto**              |
| -------------- | ----------------------- |
| Abstrato       | Concreto                |
| Tem atributos  | Tem valores específicos |
| Define métodos | Executa métodos         |

---

### 🧩 4. Criando Classes e Objetos 

- Classes:
```java
	public class Carro { 
		int potencia; 
		float velocidade; 
	}
```

- Objetos:
```java
	Carro fusca = new Carro();
```
- **Passos para criar um objeto:**
	1. Declare o tipo da variável (`Carro`).
	2. Use o operador `new` para instanciar.
---

### 🧩 5. Construtor

[[Construtores]]

- **O que é?**  
	Métodos especiais usados para inicializar objetos.
- **Exemplo:**
```java
public class Carro {
    int potencia;
    float velocidade;

    Carro(int potencia){
        this.potencia = potencia;
        velocidade = 0;
    }
}
```
- O construtor não tem retorno e tem o mesmo nome da classe.

---

### ✅ **Tarefas e Metas da Semana**

### 💡 **Observações e Insights**

- O uso de **"this"** é essencial para referenciar os elementos da classe internamente.
- Métodos como `acelerar()` e `frear()` alteram diretamente os atributos do objeto.

