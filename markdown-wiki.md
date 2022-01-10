# Markdown Wiki

[click aqui para ser encaminhado](#testando-uma-frase-com-maiúsculas-e-acentos-lírico)

<br />

[teste hyperlink](#testando-link-1-2-3)

Esta é uma pequena wiki que aborda os principais recursos da linguagem Markdown.

<br />

**Sumário**
1. Títulos
1. Ferramentas de destaque de texto
1. Formatação de texto
1. Listas
1. Link interno e externo
1. Imagem
1. Citação
1. Texto oculto "Saiba mais"
1. Checklist
1. Código
1. Dicas e atalhos

<br />

## Títulos
---

Indo do 1 ao 6, os títulos são criados com o uso de cerquilha "#" seguido de espaço.

```md
# Exemplo de título correspondente ao <h1> do HTML.

### Exemplo de título correspondente ao <h3> do HTML.
```

<br />

## Ferramentas de destaque de texto
---

Há duas formas de se marcar uma palavra ou trecho em itálico e também duas formas de se marcar uma palavra ou trecho em negrito.

Para itálico basta utilizar um asterisco "*" no início e no fim da palavra ou do trecho, sem espaços. Ou, então, underline "_" também no início e fim da palavra ou do trecho, sem espaços.

Para negrito se utiliza dois asteriscos "**" no início e no fim da palavra ou do trecho, sem espaços. Ou, então, dois underlines "__" também no início e fim da palavra ou do trecho, sem espaços.

```md
*itálico*
_também itálico_

**negrito**
__também negrito__
```

<br />

É possível utilizar um efeito de palavra ou trecho riscado, utilizando dois tils "~~", no ínicio ou fim da palavra ou trecho, sem espaços.

```md
~~Texto riscado~~
```

<br />

## Formatação de texto
---

Para acrescentar um traçado horizontal, geralmente utilizado embaixo de títulos, basta utilizar três hífens seguidos "---".

```md
## Exemplo da utilização de traçado horizontal.
---
```

<br />

Para acrescentar linhas em branco entre parágrafos basta utilizar \<br /> para cada linha que se deseja inserir.

```
Exemplo de linha em branco entre dois parágrafos.

<br />

Segundo parágrafo...
```

<br />

Para inserir uma quebra de linha, há dois modos distintos: o primeiro deles é utilizar dois espaços no fim da linha que se deseja inserir a quebra. Nesse primeiro modo, é necessário que as linhas que se deseja estar separadas também estejam em linhas diferentes.

```md
Separando linhas *dois espaços*  
utilizando dois espaços ao final da primeira linha.
```

<br />

Um outro modo de inserir uma quebra de linha é utilizar \<br> no lugar onde se deseja que haja quebra de linha. Nesse modo as linhas que se deseja estar separadas podem ser escritas em uma mesma linha, ou em linhas distintas.

```md
Inserindo uma quebra de linha <br> *nova linha*.

Inserindo uma quebra de linha <br> 
*nova linha*.
```

<br />

## Listas
---

Há três tipos de listas possíveis de serem criados. Listas não numeradas, listas numeradas e checklists.

<br />

Começando pela lista não númerada, há dois modos de cria-las. O primeiro é utilizando hífens "-" para a marcação de cada item, seguido de espaço. O segundo modo é utilizando asterisco "*" ao invés de hífens.

```md
- item 1
- item 2

* item 1
* item 2
```

<br />

Listas numeradas são criadas iniciando a linha a partir do numeral correspondente ao item, seguido de um ponto final "." e um espaço. O *Markdown*, entretanto, facilita essa tarefa por possibilitar a crianção de uma lista numerada utilizando apenas o numeral 1 seguido de ponto, ficando a cargo da linguagem enumerar os itens na devida ordem.

```md
1. item 1
2. item 2
3. item 3

1. item 1
1. item 2
1. item 3
```

<br />

Por fim, é possível criar também uma lista do tipo checklist. Basta utilizar um hífen, à exemplo das listas não numeradas, e abrir e fechar colchetes "[ ]", separando-os por um espaço. Para dar "check" em um item da lista, basta substituir o espaço entre colchetes pela letra x.  
*Checklists não são suportadas pelo VS Code.*

```md
- [x] item marcado
- [ ] item não marcado
```

<br />

## Link interno e externo
---

Começando por links "internos", ou seja, hyperlinks que encaminham para uma parte do texto do próprio texto. Por exemplo, aqueles usados em sumários.  
Deve-se deixar entre colchetes "[]" o texto que servirá de hyperlink, seguido do "texto de referência" para o qual o link encaminhará. O texto de referência deve estar entre colchetes "()", iniciado por uma cerquilha "#" e os espaços, quando houver, devem ser substituídos por hífens.

```md
[click aqui para ser encaminhado](#texto-para-onde-será-enchaminhado)
```

<br />

testando uma frase Com Maiúsculas e acentos lírico.

testando link 1 2 3