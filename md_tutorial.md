
# Guia básico de Markdown em português

Entenda primeiramente, que existem [regras](https://github.com/DavidAnson/markdownlint/blob/v0.23.1/doc/Rules.md) que na verdade são *boas práticas* na linguagem **Markdown**.

Isso pode te assustar um pouco é claro, mas saiba que ela continua funcionando mesmo que você cometa alguns erros.

## 1. Headers

* Para começar saiba que utilizar caracteres # criam _headers_ e seus níveis se dão de acordo com o número de # que você coloca no arquivo.
* Ao criar *headers* deve-se seguir a ordem de headers utilizados não podendo pular do **nível 1 (#)** para o **nível 2 (##)** como diz a regra [md001](https://github.com/DavidAnson/markdownlint/blob/v0.23.1/doc/Rules.md#md001)

* Também podemos criar _headers_ utilizando **"=========" para nível 1**, e **"---------" para nível 2**, _headers_ de nível 3 continuam utilizando **###**.

## 2. Listas

---

* Existem basicamente 2 tipos de listas possíveis, *_Ordenada_* e *_Não-Ordenada_*. As listas ordenadas são utilizadas com os caracteres **"1. (ou número ponto espaço")** e listas não ordenadas são criadas a partir dos caracteres **"- ","+ ","\* "(ou traço espaço,mais espaço,asterísco espaço)**

### Listas não-ordenadas

---

* A regra [md004](https://github.com/DavidAnson/markdownlint/blob/v0.23.1/doc/Rules.md#md004) , explica que listas não ordenadas não devem mesclar símbolos diferentes para a mesma lista.
  * Isso vale também para os subníveis.
  * As regras [md005](https://github.com/DavidAnson/markdownlint/blob/v0.23.1/doc/Rules.md#md005), e  [md007](https://github.com/DavidAnson/markdownlint/blob/v0.23.1/doc/Rules.md#md004) relacionam a identação da lista, determinando a diferença de espaços para cada subnível como 2 espaços e a quantidade em um mesmo subnível não pode ser diferente.

## CheckLists

---

 Um exemplo de lista não ordenada são as checklists, elas são utilizadas para destacar tópicos com *checkbox*.

- [ ] Caixa sem seleção

- [ ] Caixa selecionada

### Listas ordenadas

---

1. esse é um exemplo de lista ordenada
1. Nessa lista eu utilizei o inicio de todos os itens como *"1. "*.

    1. Sub-lista ordenada.
    2. Aqui eu enumero a lista como 1.2.3.... em cada item da lista.

1. Utilizar 1->3-> 2 como índice de uma lista ordenada fere a regra [md029](https://github.com/DavidAnson/markdownlint/blob/v0.23.1/doc/Rules.md#md029).

## 3. Links, imagens e coisinhas a mais

---

* Para criar links se deve utilizar a sintaxe:
>
>        (texto do link)+[endereço do link].
>
ou:
>
>        "(texto do link)"+[ref]
>
>        "[ref]":image.jpg "Texto opcional"

* Para criar links com referências a imagens deve ser utilizada a sintaxe:
>
>       "![Alternate text]"+"(image.jpg)"
>
ou:
>
>        "![Alternate text]"+"[ref]"
>
>       "[ref]":image.jpg "Texto opcional"
> <img src="kaminari.jpg" width= "200" description="Imagem contendo o personagem de boku no hero Academy Kaminari sorrindo">

* Para criar um texto com fundo escuro basta utilizar TAB+TAB

>        O texto fica assim.

---

## 4. Códigos

Para adicionar códigos basta adicionar *crase*.

        `var fruta="banana" //linha de código`
`var fruta="banana" //linha de código`

```js
fruta="banana";
```

>       ```js
>       fruta="banana";
>       ```

## 5. TABELAS

1. Coloque os nomes das colunas da tabela e os separe utilizando o caractére " **|** ".

        Exemplo:
        Invocador | Posição | Winrate

1. Na próxima linha utilize os caractéres delimitadores para cada coluna, sendo necessária somente uma vez.
   1. "**---|**" : Para alinhamento padrão.
   2. "**:---**" : Para alinhamento à esquerda (padrão).
   3. "**:---:**" : Para alinhamento centralizado.
   4. "**---:**" : Para alinhamento à direita.

1. Agora basta adicionar os itens da tabela separando-os por "**|**" e sua tabela está criada.

---

### Exemplo 1: Alinhamento à esquerda ou padrão

Invocador | Posição | Winrate
---|---|---
Pijack | top |10%
Jukes | top | 50%

---

### Exemplo 2: Alinhamento à direita

Invocador | Posição | Winrate
---:|---:|---:
Pijack | lane do topo |10%
propositalmente | lane do topo | 50%

---

### Exemplo 3: Alinhamento centralizado

Invocador | Posição | Winrate
:---:|:---:|:---:
Pijack | lane do topo |10%
propositalmente | lane do topo | 50%

---
