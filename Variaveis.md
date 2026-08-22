# 📚 AULA 2 — Variáveis, Tipos de Dados, Entrada e Saída
> 📅 **Dia 2 — Semana 1 — Setembro** | ⏱️ ~30 min | Lógica de Programação

---

## 🎯 Objetivo da Aula
Entender o que é uma **variável**, quais são os **tipos de dados** mais comuns e como **receber dados do usuário e mostrar resultados** — a base de TODO programa!

---

## 🔹 PARTE 1 — O QUE É UMA VARIÁVEL?

### 📦 Conceito Simples
> **Variável = uma "caixinha" na memória do computador para guardar um valor.**
> O conteúdo pode **variar** → por isso o nome "variável" 🤯

### Analogia Perfeita 🏷️
Imagine uma gaveta etiquetada:
- Etiqueta: `idade` → nome da variável
- Dentro da gaveta: `22` → valor guardado
- Você pode trocar o valor quando quiser!

### Regras para criar nomes de variáveis:
✅ Pode: letras, números, `_` (underline)  
❌ Não pode: espaço, acento, começar com número, palavras reservadas (`if`, `else`, `int`)  
✅ Boa prática: usar nomes **claros** → `salario` e não `s`

```
✅ nomeCompleto | ✅ nota_1 | ❌ nome completo | ❌ 1nota
```

### Como declarar (criar) uma variável:
```portugol
// Forma: tipo + nome = valor
inteiro idade = 20
real altura = 1.75
caractere sexo = 'M'
logico aprovado = verdadeiro
```

---

## 🔹 PARTE 2 — TIPOS DE DADOS

Cada "caixinha" tem um **tipo** — diz ao computador o que vai guardar dentro.

| Tipo | O que guarda | Exemplo |
|---|---|---|
| **Inteiro** | Números sem vírgula | `0`, `25`, `-100`, `2026` |
| **Real** | Números com vírgula (decimais) | `1.75`, `9.5`, `3.14` |
| **Caractere / Texto** | Letras, símbolos, palavras | `'A'`, `"Maria"`, `"Rua X"` |
| **Lógico / Booleano** | Só 2 valores possíveis | `verdadeiro` ou `falso` |

### 💡 Detalhes importantes:
- **Texto** → sempre entre aspas `" "` ou `' '`
- **Lógico** → NÃO é `sim/não` nem `1/0` — é EXATAMENTE `verdadeiro` ou `falso`
- **Números** → SEM aspas! Se colocar `"25"` vira texto e não dá para calcular

---

## 🔹 PARTE 3 — ENTRADA E SAÍDA DE DADOS

### 📤 SAÍDA = Mostrar informação na tela
> O programa **envia** dados para o usuário

```portugol
escreva("Olá, mundo!")          // Mostra: Olá, mundo!
escreva("Idade: ", idade)        // Mostra: Idade: 20
```

### 📥 ENTRADA = Receber informação do usuário
> O usuário **digita** e o programa **guarda** na variável

```portugol
inteiro idade
escreva("Digite sua idade: ")
leia(idade)                       // O que o usuário digitar → vai para a variável idade
```

### ✅ Exemplo Completo — JUNTANDO TUDO
```portugol
// 1. Declarar variáveis
caractere nome
inteiro    idade
real       altura

// 2. ENTRADA — pedir dados
escreva("Digite seu nome: ")
leia(nome)

escreva("Digite sua idade: ")
leia(idade)

escreva("Digite sua altura em metros: ")
leia(altura)

// 3. SAÍDA — mostrar resultado
escreva("\n--- DADOS CADASTRADOS ---")
escreva("Nome: ", nome)
escreva("Idade: ", idade, " anos")
escreva("Altura: ", altura, " m")
```

---

## 🧠 RESUMÃO PARA NÃO ESQUECER

| Conceito | Explicação |
|---|---|
| Variável | Caixinha etiquetada para guardar valor |
| Inteiro | Número sem vírgula → `10`, `-5` |
| Real | Número com vírgula → `3.14`, `9.9` |
| Texto | Frase/palavra → entre aspas → `"Ana"` |
| Lógico | Só verdadeiro ou falso |
| `leia()` | Entrada → usuário digita |
| `escreva()` | Saída → programa mostra |

---

## ✍️ EXERCÍCIOS — HORA DE PRATICAR!

### Exercício 1 — Cadastro Simples
> Crie um programa que:
> - Peça o **nome**, a **cidade** e a **profissão** do usuário
> - Mostre tudo em uma frase: `"Ana, você é de São Paulo e trabalha como Programador."`

<details>
<summary>👀 Ver Resposta</summary>

```portugol
caractere nome, cidade, profissao

escreva("Digite seu nome: ")
leia(nome)
escreva("Digite sua cidade: ")
leia(cidade)
escreva("Digite sua profissão: ")
leia(profissao)

escreva(nome, ", você é de ", cidade, " e trabalha como ", profissao, ".")
```
</details>

---

### Exercício 2 — Dados Numéricos
> Crie um programa que peça:
> - **Ano de nascimento** (inteiro)
> - **Altura** (real)
> - Mostre na tela: `"Você nasceu em 2004 e tem 1.80m de altura."`

<details>
<summary>👀 Ver Resposta</summary>

```portugol
inteiro anoNasc
real altura

escreva("Digite seu ano de nascimento: ")
leia(anoNasc)
escreva("Digite sua altura: ")
leia(altura)

escreva("Você nasceu em ", anoNasc, " e tem ", altura, "m de altura.")
```
</details>

---

### Exercício 3 — Desafio 💪
> Crie um programa que peça **2 números inteiros** e mostre os dois na tela.
> Dica: use variáveis com nomes diferentes, exemplo: `num1` e `num2`

<details>
<summary>👀 Ver Resposta</summary>

```portugol
inteiro num1, num2

escreva("Digite o primeiro número: ")
leia(num1)
escreva("Digite o segundo número: ")
leia(num2)

escreva("Primeiro: ", num1)
escreva("Segundo: ", num2)
```
</details>

---

## ✅ FINALIZOU? MARCA NO APP! 📱
> Vai no app → **Dia 2** → marca o checkbox ✅

---

### 📌 Para refletir antes de dormir:
- Por que `"25"` (com aspas) não dá para somar?
- O que acontece se eu tentar guardar `"Maria"` em uma variável do tipo `inteiro`?

---

Quer que eu já monte a **próxima aula (Dia 3 — Operadores Aritméticos e Expressões)** ou tem dúvida de algo que viu aqui? 🚀
