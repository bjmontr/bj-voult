## Definição
*Sequencia de instruções que resolve determinado problema*

## Formas de Representação de Algoritmos

**Descrição narrativa**
	Forma de linguagem natural
		***Principal Desvantagem***
			1. Pouco usada na prática  porque dá margem para interpretações erradas.
**Fluxograma**
	Representação gráfica do algoritmo
		***Principal vantagem***
			1. Formas geométricas diferentes mostram ações distintas.
		***Objetivo***
			Facilitar o entendimento de uma ideia.
	**Principais Símbolos do fluxograma**

![[fluxograma.png]]


### **Descrição narrativa e fluxograma: Exemplo**

![[exemplo-fluxograma.png]]
**Pseudocódigo**
	Também conhecido como português estruturado ou portugol. Ponto intermediário entre o entendimento humano e de uma linguagem de programação.
		***Principal vantagem***
			Pode ser facilmente traduzido para uma linguagem de programação.
	***Exemplo:***
```
Algoritmo Média

Var N1, N2, Média : Real

Início
	Leia N1, N2
	Média <- ( N1 + N2 ) / 2
	Se Média >= 7 Entao
		Escreva "Aprovado"
	Senao
		Escreva "Reprovado"
Fim
```
