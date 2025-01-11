---
title: Teste unitário
tags:
  - poo
  - java
date: 2025-01-11
---

## 🔍 Definição

Conjunto de classes que servem para testar uma parte do código ou a aplicação inteira.

---

## 📝 Principais Características

- **Tipos de testes**:
	- **Unidade**: Testa uma única classe ou um único método.
	- **Integração**: Testa a colaboração de um grupo de classes.
	- **Funcional**: Testa o software como um todo de acordo com os requisitos.

---

## 🧩 Vantagens

- **Vantagens:**
	- **Eficiência e velocidade**:
		Testes automatizados podem ser executados rapidamente, economizando tempo em comparação com testes manuais.
    
	- **Reprodutibilidade**:
		Os testes podem ser executados repetidamente, garantindo consistência nos resultados.
		
	- **Cobertura de código ampliada**:
		Permitem testar várias combinações de cenários, aumentando a cobertura e detectando bugs sutis.
    
	- **Facilidade de integração contínua**:
		Automatizar testes facilita a integração contínua (CI), identificando problemas em estágios iniciais do desenvolvimento.
		
	- **Economia a longo prazo**:
		Apesar do custo inicial, a automação reduz custos operacionais a longo prazo, especialmente em projetos grandes.
---

## 💻 Exemplo de Implementação

- **Contexto**: Temos 2 classes, uma classe ``classe carro`` para criar o objeto carro, uma ``classe garagem`` para criar uma garagem, e consequentemente colocar nosso carro na garagem, e também temos um banco de dados imaginário (por enquanto).

==**NÃO TEREMOS MUITO CÓDIGO NAS CLASSES POIS O INTUITO É AS CLASSES DE TESTES!!**==

1. Classe Carro
```java
public class Carro {
	// Atributos e métodos da classe Carro
}
```

2. Classe Garagem
```java
public class Garagem {
	// Atributos e métodos da classe garagem
}
```

3. Classe de teste
```java
class Teste {
	@beforeAll
	public void abrirBanco(){
		// Abertura do banco de dados
	}
	
	@beforeEach 
	public void criarObjetos(){
		// Instanciando objetos que irão ser usados no teste
	}
	
	@test
	public void testeColocarCarroNaGaragem(){
		// Testando se o carro e a garagem estão sendo cadas
	}
	@
}
```
---

## ⚡ Melhores Práticas
