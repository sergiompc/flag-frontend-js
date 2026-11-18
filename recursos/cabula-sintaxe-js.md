# Cábula · A sintaxe do JavaScript (sessão 1)

> Módulo 4 · JavaScript para Frontend. Uma página para ter aberta enquanto escrevem. Cresce na sessão 2 (decidir e repetir).

## Variáveis

```js
const preco = 49.9;       // por omissão: não volta a ser atribuída
let quantidade = 3;       // só quando o valor vai mudar
quantidade = 4;
// var: a forma antiga. Não usar
```

Nomes em camelCase (`precoUnitario`), sem espaços nem acentos.

## Tipos

| Tipo | Exemplo | `typeof` |
|---|---|---|
| string | `'Ana'`, `"Ana"`, `` `Ana` `` | `'string'` |
| number | `31`, `19.99`, `NaN` | `'number'` |
| boolean | `true`, `false` | `'boolean'` |
| undefined | `let x;` | `'undefined'` |
| null | `null` | `'object'` (um erro antigo da linguagem) |

## Números

```js
15 + 4      // 19        15 % 4     // 3 (o resto)
15 / 4      // 3.75      15 ** 4    // 50625 (potência)

pontos += 5;   pontos -= 3;   pontos *= 2;   pontos++;   pontos--;

(19.99 * 3).toFixed(2)    // '59.97' (uma string, com 2 casas decimais)
Math.round(4.6)           // 5      Math.floor(4.6)  // 4      Math.ceil(4.2)  // 5

Number('42')              // 42
Number('abc')             // NaN
'42' + 1                  // '421': com uma string, o + junta texto
```

## Strings

```js
const nome = 'Ana';
`Olá, ${nome}! Daqui a 10 anos: ${idade + 10}`     // template string: crases e ${ }

nome.length               // 3
nome.toUpperCase()        // 'ANA'
nome.toLowerCase()        // 'ana'
'  olá  '.trim()          // 'olá'
nome.includes('n')        // true
nome.replace('A', 'E')    // 'Ena'
nome.slice(0, 2)          // 'An'
nome[0]                   // 'A'
nome.at(-1)               // 'a' (a última letra)
```

Os métodos não mudam a string original: devolvem uma nova.

## Comparar

```js
>   <   >=   <=           // maior, menor…
===   !==                 // igual e diferente (valor E tipo): usar sempre
==    !=                  // convertem os tipos: não usar

&&   ||   !               // e, ou, não

const maiorDeIdade = idade >= 18;     // uma comparação guarda-se numa variável
```

## Truthy e falsy

**Falsy** (valem como `false`): `false`, `0`, `''`, `null`, `undefined`, `NaN`. **Tudo o resto é truthy**, incluindo `'0'`, `' '` e `-1`.

```js
Boolean('')        // false
Boolean('olá')     // true
```

## O template

```html
<section id="output"></section>

<script>
    let texto = '';

    // o vosso código vai aqui
    texto += `<p>…</p>`;

    /// escrever na página
    let output = document.getElementById('output');
    output.innerHTML = texto;
</script>
```

Página em branco? **F12 › Console**: o erro diz o ficheiro e a linha.
