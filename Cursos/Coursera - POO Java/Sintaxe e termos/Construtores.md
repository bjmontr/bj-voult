---
title: Construtores
tags:
  - java
  - poo
date: 2024-12-31
---

## 🔍 Definição

É um bloco de código especial dentro da classe, que tem por função inicializar novos objetos. São chamados automaticamente quando um novo objeto é criado. facilitando a configuração inicial do objeto.

---

## 📝 Principais Características

| Caracteristicas |                                          |
| --------------- | ---------------------------------------- |
| Nome            | Deve ter o mesmo nome da classe.         |
| Retorno         | Não possui, nem mesmo o `void`.          |
| Acesso          | Pode ter qualquer modificador de acesso. |

- **Tipos de construtores**:
	- **Default**: Se a classe nao tiver um construtor explicitamente definido, o Java oferece um construtor padrão, que não faz nada além de chamar o construtor da superclasse.
	
	- **Parametrizado**: Permite que o desenvolvedor especifique um ou mais parâmetros, possibilitando a inicialização de objetos com diferentes estados.

---

## 🧩 Vantagens e Desvantagens

- **Vantagens:**
- **Desvantagens:**

---

## 💻 Exemplo de Implementação

```java
public class Carro {
	String marca;
	String modelo;
	// Construtor parametrizado
	public Carro(String marca, String modelo){
		this.marca = marca;
		this.modelo = modelo;
	}
}
```

---

## ⚡ Melhores Práticas

- **Importância:** 
	- Inicialização segura
	- Flexibilidade
	- Encapsulamento