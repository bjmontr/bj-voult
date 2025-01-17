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
		// Testando se o carro e a garagem estão sendo cadastrados no banco
	}
	@afterEach
	public void apagarRegistro(){
		// Apagando os registros criados
	}
	
	@afterAll
	public void fechandoBanco(){
		// Fechando o banco
	}
}
```

- **Nomenclaturas**:
	- **BeforeAll**:
		Executado **uma única vez** antes de todos os testes da classe. Geralmente usado para configurações que precisam ser realizadas apenas uma vez, como abrir conexões com banco de dados ou inicializar recursos globais. Deve ser aplicado em métodos estáticos.
		
	- **BeforeEach**:
		Executado **antes de cada teste** na classe. Usado para configurar o estado inicial necessário para o teste, como instanciar objetos ou limpar variáveis.
		
	- **Test**:
		Marca um método como um **teste unitário**. É onde você implementa a lógica para verificar o comportamento esperado do código, usando asserções (como `Assertions.assertTrue()` ou `assertEquals()`).
		
	- **AfterBefore**:
		Executado **após cada teste** na classe. Usado para realizar ações de limpeza, como remover registros temporários ou resetar estados alterados durante o teste.
		
	- **AfterAll**:
		Executado **uma única vez** após todos os testes da classe. Geralmente usado para liberar recursos globais, como fechar conexões de banco de dados ou encerrar serviços mockados. Deve ser aplicado em métodos estáticos.
---

## ⚡ Melhores Práticas

1. **Organização e isolamento**
	- **Independência dos testes**: 
		- Cada teste deve ser independente dos outros. Um teste nunca deve depender do sucesso ou falha de outro teste.
		- Use ``@BeforeEach`` para garantir que os objetos e estados sejam criados novamente antes de cada teste.
		 
2. **Uso correto das anotações**
	- ``@BeforeAll`` e ``@AfterAll``: 
		- Use para configurar e liberar recursos que são caros para inicializar como conexões de banco de dados.
	- ``@BeforeEach`` e ``@AfterEach``:
		- Use para configurar ou limpar recursos que devem ser reiniciados antes e após **cada teste individual**, como instanciar objetos ou remover registros criados.
		 
3. **Simplicidade nos testes**:
	- **Testar um único comportamento por método**:
		- Cada método anotado com @Test deve validar apenas uma funcionalidade específica. Isso facilita a identificação de problemas quando o teste falha.
		 
4. **Manutenção de dados de teste**
	- **Limpe os dados após cada teste**:
		- Isso evita que dados residuais prejudiquem outros testes. (@AfterEach)
		 
5. **Assertivas significativas**
	- **Use assertivas específicas e claras**:
		- Use `assertEquals`, `assertTrue`, `assertThrows`, etc.
			- **Exemplo ruim:** `assertTrue(resultado == esperado)`.
			- **Exemplo bom:** `assertEquals(esperado, resultado)`.