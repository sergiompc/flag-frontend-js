# Exercício 1.1 · O cartão de apresentação

**Sessão 1 do módulo 4 · sozinhos · cerca de 12 minutos**

Vão escrever um programa que mostra, na página, o cartão de apresentação de uma pessoa (vocês ou uma pessoa inventada).

## O ponto de partida

Uma cópia do `0-template.html`, com o nome `ex-1.1-cartao.html`, na vossa pasta `flag-frontend/04-javascript/s01/`. O `styles.css` tem de estar na mesma pasta.

## O que fazer

1. Guardem em variáveis: o nome, o apelido, a cidade, o ano de nascimento, o ano atual, a profissão e se a pessoa está a aprender JavaScript (verdadeiro ou falso). Escolham bem entre `const` e `let`.
2. Calculem a idade a partir dos dois anos.
3. Construam o nome completo e as iniciais (a primeira letra do nome e a do apelido).
4. Mostrem o cartão na página, com uma template string:
   - o nome completo em maiúsculas, com as iniciais entre parênteses;
   - a idade e a cidade;
   - a profissão;
   - quantos caracteres tem o nome completo;
   - se está a aprender JavaScript;
   - a idade que terá daqui a 10 anos.

## Como deve ficar

```
RUI COSTA (RC)
32 anos, de Lisboa
Profissão: designer
O nome completo tem 9 caracteres.
A aprender JavaScript: true
Daqui a 10 anos terá 42 anos.
```

Nada aparece? Abram a consola do browser (F12 › Console): o erro diz a linha.
