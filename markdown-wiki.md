# Markdown Wiki

Esta é uma pequena wiki que aborda os principais recursos da linguagem Markdown.

<br />

**Sumário**
1. [Títulos](#títulos)
1. [Ferramentas de destaque de texto](#ferramentas-de-destaque-de-texto)
1. [Formatação de texto](#formatação-de-texto)
1. [Listas](#listas)
1. [Link interno e externo](#link-interno-e-externo)
1. [Imagem](#imagem)
1. [Citação](#citação)
1. [Tabela](#tabela)
1. [Código](#código)
1. [Texto colapsado](#texto-colapsado)
1. [Nota de rodapé](#nota-de-rodapé)
1. [Dicas e atalhos](#dicas-e-atalhos)

<br />

## Títulos

Podendo ir do 1 ao 6, os títulos são criados com o uso de cerquilha "#" seguido de espaço.

```md
# Exemplo de título correspondente ao <h1> do HTML.

### Exemplo de título correspondente ao <h3> do HTML.
```

<br />

## Ferramentas de destaque de texto

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

Para acrescentar um traçado horizontal, geralmente utilizado embaixo de títulos, basta utilizar três hífens seguidos "---". Lembrando que o Github, por exemplo, já exibe por padrão um traço horizontal abaixo de cada título.

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

Começando por links "internos", ou seja, hyperlinks que encaminham para uma parte do texto do próprio texto. Por exemplo, aqueles usados em sumários. Os links internos encaminham apenas títulos dentro do texto (os tópicos que são ressaltados com a # que equivale ao \<hx> no HTML).  
Deve-se deixar entre colchetes "[]" o texto que servirá de hyperlink (o *click aqui*), seguido do "título de referência" para o qual o link encaminhará. O título de referência deve estar entre parênteses "()", iniciado por uma cerquilha "#" e os espaços, quando houver, devem ser substituídos por hífens, as letras maiúsculas, quando houver, devem ser ignoradas e a acentuação deve ser mantida.

```md
[click aqui](#nome-do-título-para-onde-será-enchaminhado)
```

<br />

Para criar um link externo, os hyperlinks clássicos, basta realizar o mesmo processo da criação dos links internos sem acrescentar a cerquilha ao início, mas utilizando o link da página no lugar do nome do título.

```md
[click aqui](www.exemplodepaginaaleatória.com.br)
```

<br />

## Imagem

Para acrescentar uma imagem, deve utilizar o ponto de exclamação "!" seguido de um título para a imagem (que não ficará aparente) entre colchetes "[]". Em seguida, entre parênteses "()", deve-se inserir o nome exato do arquivo da imagem, incluindo a extensão, iniciando-se por uma barra "/". 

```md
![nome da imagem](/nome-do-arquivo.png)
```

<br />

É possível combinar um hyperlink com uma imagem. Em que ao se clickar na imagem, ela encaminhará para o link desejado.  
Para isso, basta combinar os dois recursos, criando primeiro a imagem e, em seguida, torna-la o "click aqui" do link.

```md
[![nome imagem](/arquivo.png)](www.exemplo.com.br)
```

<br />

## Citação

Muito comuns em fóruns e e-mails, é possível criar um visual de "citação" no *Markdown*. Para isso, basta utilizar o sinal de maior ">" no início de cada linha que se deseja apresentar como citação.
A quebra de linha se dá conforme apresentado anteriormente, para representar linhas em branco, entretanto, basta apenas utilizar o sinal de maior no início da linha e deixa-la em branco.  
Um modo de indicar o autor do texto citado é colocar seu nome entre as tags \<cite>\</cite>, começando por dois hífens, dentro ou fora da caixa de citação.

```md
> Exemplo de citação
>
> Terceira linha da citação
> -- <cite>Fulano</cite>
```

<br />

Assim como nos fóruns e e-mails, é possível utilizar citações de citações. Para cada nova citação, basta utilizar um sinal de maior na linha seguinte, seguido do número de sinais já utilizados.

```md
> Citação da citação
>> Primeira citação
```

<br />

## Tabela

É possível criar tabelas com o próprio *Markdown. Basta utilizar uma barra vertical "|" ao início da linha, e acrescentar mais uma barra vertical para cada nova coluna que se deseja acrescentar. A primeira linha corresponde ao título das colunas. Na segunda linha deve-se acrescentar dois pontos ":" seguido de um número de hífens (aqui se utiliza 5) para marcar o alinhamento horizontal dos textos nas colunas (à esquerda, centralizado, à direita).  
Para alinhar à esquerda os dois pontos devem estar no início da sequência de hífens. Para deixar centralizado se deve utilizar dois pontos no começo e no fim da sequência de hífens. Para alinhar à direita os dois pontos deve estar ao final da sequência de hífens.  
Após essa linha, pode-se formatar o número desejado de linhas com seus respectivos conteúdos, seguindo sempre o mesmo número de colunas.
Lembrando: deve haver uma barra vertical no início e ao fim da linha, e entre cada coluna. O alinhamento de cada coluna pode ser diferente, mas ele é válido para todas as linhas da coluna, incluindo o título.

```md
| Texto à esquerda | Texto centralizado | Texto à direita |
| :----- | :-----: | -----: |
| Linha 2 | Linha 2 | Linha 2 |
| Coluna 1 | Coluna 2 | Coluna 3 |
```

<br />

## Código

Em *Markdown* existe a possibilidade de se criar uma interface para representar as linhas de um código. De forma simples, para apenas uma única linha, basta colocar o código que se deseja representar entre acentos graves "`".  
Para uma representação mais elaborada, são utilizados três acentos graves seguidos, na primeira e última linha, entre essas duas linhas se insere o código que se deseja representar.  
Após os três acentos graves da primeira linha, pode-se inserir ou o nome ou a extensão do código que se está representando. Isso faz com que a formatação seja mais semelhante àquilo que se vê nos editores ou IDE's.  
*Foi utilizado um ponto antes dos três acentos graves no primeiro exemplo abaixo por motivos de conflito com o próprio código do Markdown. O correto é iniciar a linha apenas com os três acentos.*

```md
.```py
print('hello world')
.```
```

```md
`print('hello world')`
```

<br />

## Texto colapsado

Uma funcionalidade possível de incluir em textos com *Markdown* é o de colapsar/recolher a partir de um trecho de texto. Mais ou menos como uma funcionalidade do tipo "Saiba mais". Resultando em um texto oculto e um título vísivel iniciado por uma seta.  
Para cria-lo usa-se as tags \<details>\</details>, que devem englobar todo o bloco de texto, incluíndo o título. O título é criado a partir das tags \<summary>\</summary>. O texto em si deve vir após o título e antes da última tag de </details>.  
A formatação do texto a ser colapsado segue todas as regras padrões de formatação do *Markdown*. Se o texto for indentado, ocorre uma variação na forma de apresentação do texto.

```md
<details>

<summary>Título da seção</summary>

Texto a ser colapsado.  

</details>
```

```md
<details>

<summary>Título da seção</summary>

    Um outro estilo de apresentação de texto colapsado.

</details>
```

<br />

## Nota de rodapé

É possível inserir notas de rodapé com *Markdown, para isso é utilizado colchetes "[]" preenchido com um acento circunflexo seguido do número correspondente.  
*O VS Code não suporta esse recurso.*

```md
Uma nota de rodapé [^1]

*Imagine que a linha abaixo está no fim da página*.

<br />

[^1]: nota de rodapé
```

<br />

## Dicas e atalhos

Para visualizar o aspecto final do seu texto, utilize o preview do markdown. Ele pode ser acessado pelas teclas ctrl + shift + v.