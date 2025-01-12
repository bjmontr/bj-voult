---
title: Visibilidade
tags:
  - java
  - poo
date: 2025-01-12
---

## 🔍 Definição

Na representação de classes em UML, os símbolos `-`, `+` e `#` são usados para indicar a **visibilidade** de atributos e métodos, ou seja, o nível de acesso permitido a esses elementos dentro da classe.

---

## 📝 Principais Características

- `-` **Private**:
	- **Significado**: 
		O elemento só pode ser acessado dentro da própria classe.
		
	- **Uso comum**: 
		Usado para proteger informações sensíveis ou garantir o encapsulamento.
		
- `+` **Public**:
	- **Significado**:
		O elemento pode ser acessado por qualquer classe do sistema.
		
	- **Uso comum**:
		Atributos ou métodos que precisam estar disponíveis para outros objetos ou usuários do sistema.
		
- `#` **Protected**:
	- **Significado**:
		O elemento pode ser acessado pela própria classe e por suas subclasses, mas não por outras classes externas.
		
	- **Uso comum**:
		Garantir que atributos e métodos possam ser reutilizados por classes derivadas sem ficarem disponíveis para classes não relacionadas.

- Comparativo entre os níveis de visibilidade

| Símbolo | Nível de acesso | Acesso permitido para           |
| ------- | --------------- | ------------------------------- |
| `-`     | Privado         | Apenas dentro da própria classe |
| `+`     | Público         |                                 |

---

## 🧩 Vantagens e Desvantagens

- **Vantagens:**
	- Encapsulamento
	- Segurança
	- Organização

---

## 💻 Exemplo de Implementação

Imagine um sistema onde temos uma classe `ContaBancaria`:

```
class ContaBancaria {
	- saldo: double   // Privado: Não pode ser acessado diretamente fora da classe.
	# taxaOperacao: double   // Protegido: Pode ser usado por subclasses.
	+ ConsultarSaldo(): double   // Público: Pode ser chamado por qualquer classe.
}
```

