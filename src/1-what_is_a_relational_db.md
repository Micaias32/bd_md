# O que é um Banco de Dados Relacional (BDR)?

Já sabemos o que é um banco de dados, mas como que fazemos um? Qual o modo usado normalmente?

Bom, no mundo onde vivemos, temos vários modos de fazer um banco de dados, e o mais comum atualmente, é o Banco de Dados Relacional, onde vamos guardar os dados usando o relacionamento entre eles. Se está complicado, vamos usar um exemplo:

Suponhamos que temos uma pessoa chamada Miguel. Ele é um usuário do nosso sistema. Temos que guardar algumas informações dele. Num sistema de verdade teríamos que guardar muitas informações dele, mas, para esse exemplo, vamos utilizar somente o nome completo, nome de usuário, *email* e senha. Se colocássemos essas informações numa planilha ficaria mais ou menos assim:

| Nome            | Nome de Usuário | *Email*                   | Senha        |
| --------------- | --------------- | ------------------------- | ------------ |
| Miguel Oliveira | miguel_o        | "miguel123@fakeemail.com" | miguel123456 |

Neste exemplo, vemos que podemos tratar usuário Miguel como uma linha da tabela, já que por essa linha, podemos saber todos os dados dele, e para um banco de dados, Miguel é somente isso, dados com conexões entre eles. Se adicionássemos outro usuário, seria simples, já que é só adicionar mais uma linha:

| Nome            | Nome de Usuário | *Email*                   | Senha        |
| --------------- | --------------- | ------------------------- | ------------ |
| Miguel Oliveira | miguel_o        | "miguel123@fakeemail.com" | miguel123456 |
| Luiz Rocha      | luiz_rocha      | "luizrocha@fakeemail.com" | Jniowefm8482 |

Agora, se precisarmos das informações do usuário "luiz_rocha", procuramos a linha com esse nome de usuário, e vemos a informação que precisamos.

A parte mais legal é que não estamos distantes do banco em si, até porque usar uma tabela para modelar e mostrar como um BDR funciona é muito comum.

> Quando se fala em bancos de dados relacionais, usamos nomes mais **bonitinhos** para esses conceitos. Mantemos colunas (*columns*), mas ao invés de linhas, usamos tuplas (*tuples*) e chamamos a tabela de *table*, porque a maioria dos sistemas feitos para bancos de dados são em inglês, então é útil saber os nomes em inglês.