# Exercício 1.3 · A ficha de inscrição (desafio)

**Sessão 1 do módulo 4 · para quem acabar cedo, ou para casa**

Os dados de um formulário chegam sempre em texto, e muitas vezes mal escritos. O vosso programa limpa-os e verifica-os.

## O ponto de partida

Uma cópia do `0-template.html`, com o nome `ex-1.3-inscricao.html`. Comecem com estes dados, tal como estão:

```js
const nomeEscrito = '   mARIA joão  ';
const idadeEscrita = '17';
const emailEscrito = ' Maria.Joao@Exemplo.PT ';
const codigoPromocional = '';
```

## O que fazer

1. **Limpar:** o nome sem espaços à volta, em minúsculas e só com a primeira letra em maiúscula; a idade como número; o email sem espaços e em minúsculas.
2. **Verificar** (cada resultado é verdadeiro ou falso):
   - é maior de idade?
   - o email é válido? (para já, basta ter um `@` e um `.`)
   - tem código promocional? (uma string vazia conta como "não tem")
   - pode inscrever-se? (só se for maior de idade **e** o email for válido)
3. Mostrem a ficha na página, com a idade e o tipo dela (tem de ser `number`).

## Como deve ficar

```
Ficha de inscrição
Nome: Maria joão
Idade: 17 (number)
Email: maria.joao@exemplo.pt
Maior de idade: false
Email válido: true
Tem código promocional: false
Pode inscrever-se: false
```

Experimentem com outros dados: uma idade de `'25'`, um email sem `@`, um código `'NATAL10'`.

**Já conhecem o `if`?** Mostrem uma mensagem diferente conforme a pessoa pode ou não inscrever-se. Se não conhecem, é o tema de 6.ª feira.
