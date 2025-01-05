---
title: Métodos vs Atributoss
tags: 
date:
---

## 📝 Principais Características

| Aspecto       | Atributos                                  | Métodos                                             |
| ------------- | ------------------------------------------ | --------------------------------------------------- |
| Definição     | Representam o estado ou dados de um objeto | Representam o comportamento ou ação de um objeto.   |
| Função        | Armazenam informações sobre o objeto.      | Executam ações ou manipulam os atributos do objeto. |
| Visibilidade  | Podem ser privados (encapsulamento).       | Podem ser públicos ou privados.                     |
| Inicialização | Inicializados na criação do objeto.        | Definem as ações do objeto, não armazenam dados.    |

---

## 💻 Exemplo de Implementação

### Atributos

- **Classe:**
```java
public class Carro {
	int potencia;
	float velocidade;
	String cor;
}
```

- **Objeto:**
```java
civic.potencia = 150;
civic.velocidade = 140.5f;
civic.cor = "azul";
```

### Métodos

```java
public void pintar(String novaCor) {
	cor = novaCor;
}
```