# Logbook for JavaScript
Logbook for Programming Languages ​​and Paradigms

## Índice

1. [Introdução](#introdução)
2. [Método de Implementação](#método-de-implementação)
3. [Precedência e Associatividade de Operadores](#precedência-e-associatividade-de-operadores)
4. [Tipos, valores e variáveis](#tipos-valores-e-variáveis)

## Introdução

Introdução ao JavaScript e suas Aplicações:

JavaScript é uma das linguagens de programação mais populares e versáteis do mundo da tecnologia. Criada em 1995 por Brendan Eich, inicialmente para melhorar a experiência de interação dos usuários com páginas web, o JavaScript tornou-se uma linguagem essencial para o desenvolvimento front-end e back-end.

JavaScript é uma linguagem de programação interpretada, ou seja, é executada diretamente no navegador do usuário, permitindo que desenvolvedores criem páginas web interativas, dinâmicas e reativas. Inicialmente, sua aplicação principal era a manipulação de elementos HTML, permitindo que os desenvolvedores criassem páginas web mais ricas em funcionalidades.

Com o passar do tempo, o JavaScript evoluiu significativamente, sendo adotado também no desenvolvimento de aplicações server-side (back-end), com a popularização do Node.js. Dessa forma, desenvolvedores podem utilizar a mesma linguagem tanto no front-end quanto no back-end, o que resulta em maior eficiência e coesão no desenvolvimento de aplicações web completas.

As aplicações do JavaScript são diversas, incluindo:

1. __Desenvolvimento Web Front-end:__ JavaScript é essencial para criar interatividade e dinamismo em páginas web. Ele é usado para criar efeitos visuais, animações, formulários interativos, manipulação do DOM (Document Object Model), e muito mais.

2. __Desenvolvimento Web Back-end:__ Com o Node.js, o JavaScript pode ser utilizado no lado do servidor para criar aplicações escaláveis e de alto desempenho. É possível criar APIs, manipular arquivos, realizar operações de banco de dados e outras tarefas do servidor.

3. __Aplicações Web Full-Stack:__ Com a combinação do desenvolvimento front-end e back-end em JavaScript, é possível criar aplicações web completas com um único conjunto de habilidades.

4. __Desenvolvimento de Jogos:__ O JavaScript é usado em conjunto com bibliotecas e frameworks, como o Phaser e o Three.js, para criar jogos 2D e 3D diretamente no navegador.

5. __Aplicações Móveis:__ Com o uso de tecnologias como React Native e Ionic, é possível desenvolver aplicativos móveis para iOS e Android usando JavaScript.

6. __Internet das Coisas (IoT):__ JavaScript pode ser usado em plataformas como o Johnny-Five para programar dispositivos e sensores em projetos de IoT.

7. __Chatbots e Automatização:__ Com o uso de bibliotecas de processamento de linguagem natural (NLP) e ferramentas como o Botpress, é possível criar chatbots interativos.

8. __Visualização de Dados:__ Bibliotecas como D3.js permitem criar gráficos interativos e visualizações de dados complexas.

Em resumo, JavaScript é uma linguagem de programação versátil e poderosa, utilizada em praticamente todas as áreas do desenvolvimento web e de aplicações. Sua popularidade e adoção generalizada garantem que o JavaScript continue sendo uma das principais linguagens de programação no mundo da tecnologia.

## Método de Implementação

JavaScript é uma linguagem de programação interpretada, não uma linguagem compilada. Isso significa que, em vez de ser compilado em código de máquina antes da execução, o código JavaScript é lido e executado linha por linha por um interpretador no navegador ou no ambiente em que está sendo executado.

O processo de execução do JavaScript ocorre da seguinte maneira:

1. __Análise léxica e sintática:__ O código JavaScript é lido e dividido em elementos léxicos, como palavras-chave, operadores, identificadores, etc. Em seguida, esses elementos são analisados para formar uma estrutura de árvore de sintaxe abstrata (AST).

2. __Compilação Just-in-Time (JIT):__ O interpretador JavaScript, presente no navegador ou no ambiente de execução, compila o código de árvore de sintaxe abstrata (AST) em código de byte, que é uma representação intermediária.

3. __Execução:__ O código de byte gerado é interpretado e executado pelo mecanismo JavaScript do navegador ou do ambiente de execução.

A interpretação do JavaScript traz algumas vantagens, como a portabilidade do código, pois não há necessidade de recompilação para diferentes plataformas, e facilita a depuração, pois os erros podem ser identificados linha por linha.

No entanto, a interpretação pode ser mais lenta em comparação com linguagens compiladas, especialmente para operações intensivas em processamento. Para melhorar o desempenho, os navegadores modernos também usam otimização JIT, que transforma trechos de código frequentemente usados em código nativo otimizado para a plataforma em questão, acelerando sua execução.

## Precedência e Associatividade de Operadores

pagina 61. 

Em JavaScript, os operadores têm uma precedência e associatividade específica, o que determina a ordem em que as operações são realizadas em uma expressão com múltiplos operadores. É importante entender a precedência e associatividade dos operadores para garantir que as expressões sejam avaliadas corretamente.

Precedência:
A precedência de um operador determina a ordem em que ele é avaliado em relação a outros operadores na expressão. Operadores com maior precedência são avaliados primeiro. Caso operadores tenham a mesma precedência, a associatividade é usada para determinar a ordem de avaliação.

Aqui estão alguns exemplos de operadores JavaScript listados em ordem decrescente de precedência (ou seja, os operadores com maior precedência aparecem primeiro):

Precedência mais alta:

Parenteses (): Avaliados primeiro para definir a ordem de avaliação.
Acesso a propriedades de objetos . e acesso a elementos de array [].
Operadores aritméticos:

> **: Exponenciação.
*, /, %: Multiplicação, divisão e resto da divisão.
+, -: Adição e subtração.

>Operadores de comparação:
 '>', <, >=, <=: Maior que, menor que, maior ou igual a, menor ou igual a.
==, !=, ===, !==: Igualdade e desigualdade.
in, instanceof: Operadores especiais de comparação.

>Operadores lógicos:
&&: E lógico.
||: OU lógico.
!: Negação lógica.
Operador ternário:

? :: Operador ternário condicional.
Associatividade:
A associatividade determina a direção em que os operadores são agrupados quando têm a mesma precedência. Em JavaScript, a maioria dos operadores é associativa da esquerda para a direita, o que significa que as operações são realizadas da esquerda para a direita. No entanto, o operador de exponenciação ** é associativo da direita para a esquerda, o que significa que as operações são realizadas da direita para a esquerda.

É importante lembrar que, se você estiver usando diferentes operadores na mesma expressão, é fundamental conhecer a precedência e associatividade para garantir que a expressão seja avaliada corretamente. Caso seja necessário alterar a ordem de avaliação, é possível usar parênteses para agrupar as operações conforme desejado.

## Tipos, valores e variáveis
pagina 28 - 52

Os tipos de JavaScript podem ser divididos em duas categorias: __tipos primitivos__ e __tipos de objeto__. E podem ser divididos em __tipos com métodos__ e __tipos sem métodos__. Também podem ser classificados como __tipos mutáveis__ e __tipos imutáveis__.

Qualquer valor em JavaScript que não seja número, string, booleano, null ou undefined é um objeto. 


__Tipo mutável:__ Objetos e arrays: um programa JavaScript pode alterar os valores de propriedades do objeto e de elementos de arrays.

__Tipo Imutáveis:__ números, booleanos, null e undefined são imutáveis – nem mesmo faria sentido falar sobre alterar o valor de um número.

As variáveis em JavaScript são __não tipadas__: você pode atribuir um valor de qualquer tipo a uma variável e, posteriormente, atribuir um valor de tipo diferente para a mesma variável. As variáveis são declaradas com a palavra-chave var. 

JavaScript utiliza __escopo léxico__. As variáveis declaradas fora de uma função são variáveis globais e são visíveis por toda parte em um programa JavaScript. As variáveis declaradas dentro de uma função têm escopo de função e são visíveis apenas para o código que aparece dentro dessa função. 

A declaração e o escopo de variáveis são abordados na Seção 3.9 e na Seção 3.10.


1. Number;
2. String;
3. Boolean:
4. Undefined: Representa uma variável que foi declarada, mas ainda não possui valor atribuído.
5. Null: Representa um valor nulo, ou seja, a variável está vazia ou não possui valor.
6. Object: Representa um objeto, que pode conter várias propriedades e métodos.
7. Array: Representa uma lista ordenada de elementos.
8. Function: Representa um bloco de código reutilizável que pode ser chamado por meio de um nome ou uma variável.


### 1 - Number: 
Representa números inteiros ou de ponto flutuante. Por exemplo: 10, 3.14.

JavaScript não faz distinção entre valores inteiros e valores em ponto flutuante, permite representar exatamente todos os inteiros entre −9007199254740992 (−2^53) e 9007199254740992 (2^53).

### 2 - String
Representa uma sequência de caracteres ordenada imutável de valores de 16 bits. É delimitada por aspas simples ou duplas. Por exemplo: 'Olá, mundo!', "JavaScript".

Sequências de escape em strings literais usa o caractere de barra invertida (\) que possui  um propósito especial nas strings em JavaScript. Combinado com o caractere que vem a seguir, ele representa um caractere que não pode ser representado de outra forma dentro da string. Por exemplo:

| Sequência | Caractere representado       |
|-----------|-----------------------------|
| \0        | O caractere NUL (\u0000)     |
| \b        | Retrocesso (\u0008)          |
| \t        | Tabulação horizontal (\u0009)|
| \n        | Nova linha (\u000A)          |
| \v        | Tabulação vertical (\u000B)  |
| \f        | Avanço de página (\u000C)    |
| \r        | Retorno de carro (\u000D)    |
| \"        | Aspas duplas (\u0022)        |
| \'        | Apóstrofo ou aspas simples (\u0027)|
| \\        | Barra invertida (\u005C)     |
| \xXX      | O caractere Latin-1 especificado pelos dois dígitos hexadecimais XX |
| \uXXXX    | O caractere Unicode especificado pelos quatro dígitos hexadecimais XXXX |

### 3 - booleana:
Um valor booleano representa verdadeiro ou falso, ligado ou desligado, sim ou não. Só existem dois valores possíveis desse tipo. As palavras reservadas true e false são avaliadas nesses dois valores. Geralmente, os valores booleanos resultam de comparações feitas nos programas JavaScript.

### 4 - null e undefined

### literal numérico. 
(Página 31). 

Quando um número aparece diretamente em um programa JavaScript, ele é chamado de literal numérico. JavaScript aceita literais numéricos em vários formatos, conforme descrito nas seções a seguir. Note que qualquer literal numérico pode ser precedido por um sinal de subtração (-) para tornar o número negativo. Tecnicamente, contudo, - é o operador de negação unário (consulte o Capítulo 4) e não faz parte da sintaxe de literal numérico.

1. literais inteiros

Em um programa JavaScript, um inteiro de base 10 é escrito como uma sequência de dígitos. Por exemplo:

0 3 10000000 

Além dos literais inteiros de base 10, JavaScript reconhece valores hexadecimais (base 16). Um literal hexadecimal começa com “0x” ou “0X”, seguido por uma sequência de dígitos hexadecimais. Um dígito hexadecimal é um dos algarismos de 0 a 9 ou as letras a (ou A) até f (ou F), as quais representam valores de 10 a 15. Aqui estão exemplos de literais inteiros hexadecimais:

0xff // 15*16 + 15 = 255 (base 10)

0xCAFE911

Embora o padrão ECMAScript não ofereça suporte para isso, algumas implementações de JavaScript permitem especificar literais inteiros no formato octal (base 8). Um literal em octal começa com o dígito 0 e é seguido por uma sequência de dígitos, cada um entre 0 e 7. Por exemplo:

0377 // 3*64 + 7*8 + 7 = 255 (base 10)

Como algumas implementações aceitam literais em octal e algumas não, você nunca deve escrever um literal inteiro com um zero à esquerda; nesse caso, não dá para saber se uma implementação vai interpretá-la como um valor octal ou decimal. No modo restrito de ECMAScript 5 (Seção 5.7.3), os literais em octal são proibidos explicitamente.

2. literais em ponto flutuantes

Os literais em ponto flutuante podem ter um ponto decimal; eles usam a sintaxe tradicional dos números reais. Um valor real é representado como a parte inteira do número, seguida de um ponto decimal e a parte fracionária do número.

Os literais em ponto flutuante também podem ser representados usando-se notação exponencial: um número real seguido da letra e (ou E), seguido por um sinal de adição ou subtração opcional, seguido por um expoente inteiro. Essa notação representa o número real multiplicado por 10, elevado à potência do expoente.

Mais sucintamente, a sintaxe é:

[dígitos][.dígitos][(E|e)[(+|-)]dígitos]

    Por exemplo: 
    3.14 
    2345.789 
    .333333333333333333
    6.02e23 // 6.02 × 10^23
    1.4738223E-32 // 1.4738223 × 10−32

(Página 31). 


### 3.1.3 Aritmética em JavaScript - (Página 32). 

Além desses operadores aritméticos básicos, JavaScript aceita operações matemáticas mais complexas por meio de um conjunto de funções e constantes definidas como propriedades do objeto Math:

    Math.pow(2,53) // => 9007199254740992: 2 elevado à potência 53
    Math.round(.6) // => 1.0: arredonda para o inteiro mais próximo
    Math.ceil(.6) // => 1.0: arredonda para cima para um inteiro
    Math.floor(.6) // => 0.0: arredonda para baixo para um inteiro
    Math.abs(-5) // => 5: valor absoluto
    Math.max(x,y,z) // Retorna o maior argumento
    Math.min(x,y,z) // Retorna o menor argumento
    Math.random() // Número pseudoaleatório x, onde 0 <= x < 1.0
    Math.PI // π: circunferência de um círculo / diâmetro
    Math.E // e: A base do logaritmo natural
    Math.sqrt(3) // A raiz quadrada de 3
    Math.pow(3, 1/3) // A raiz cúbica de 3
    Math.sin(0) // Trigonometria: também Math.cos, Math.atan, etc.
    Math.log(10) // Logaritmo natural de 10
    Math.log(100)/Math.LN10 // Logaritmo de base 10 de 100
    Math.log(512)/Math.LN2 // Logaritmo de base 2 de 512
    Math.exp(3) // Math.E ao cubo

A aritmética em JavaScript não gera erros em casos de estouro, estouro negativo ou divisão por zero. Quando o resultado de uma operação numérica é maior do que o maior número representável (estouro), o resultado é um valor infinito especial, que JavaScript indica como __Infinity__. Da mesma forma, quando um valor negativo se torna maior do que o maior número negativo representável, o resultado é infinito negativo, indicado como __-Infinity__. Os valores infinitos se comportam conforme o esperado: somá-los, subtraí-los, multiplicá-los ou dividi-los por qualquer coisa resulta em um valor infinito (possivelmente com o sinal invertido).

1. __Estouro Negativo:__ Ocorre quando o resultado de uma operação numérica é mais próximo de zero do que o menor número representável. Nesse caso, JavaScript retorna 0 ou "zero negativo", que é quase indistinguível do zero normal.
2. __Divisão por Zero:__ Em JavaScript, a divisão por zero não gera um erro, mas retorna infinito ou infinito negativo. A única exceção é a divisão de zero por zero, que retorna o valor especial "NaN" (Not-a-Number).
3. __NaN (Not-a-Number):__ É um valor especial que surge em várias situações, como dividir infinito por infinito, extrair a raiz quadrada de um número negativo ou usar operadores aritméticos com operandos não numéricos que não podem ser convertidos em números.

(Página 32). 


Diário de Bordo - Tipos, Valores e Variáveis em JavaScript
Introdução
Neste capítulo, vamos explorar os fundamentos dos tipos de dados, valores e variáveis em JavaScript. Entender esses conceitos é essencial para a programação eficiente e para evitar erros comuns ao trabalhar com a linguagem.

Tipos de Dados em JavaScript
JavaScript possui diversos tipos de dados que são utilizados para representar diferentes tipos de informações. Os principais tipos de dados em JavaScript são:

Number: Representa números inteiros ou de ponto flutuante. Por exemplo: 10, 3.14.

String: Representa uma sequência de caracteres. É delimitada por aspas simples ou duplas. Por exemplo: 'Olá, mundo!', "JavaScript".

Boolean: Representa um valor lógico verdadeiro (true) ou falso (false).

Undefined: Representa uma variável que foi declarada, mas ainda não possui valor atribuído.

Null: Representa um valor nulo, ou seja, a variável está vazia ou não possui valor.

Object: Representa um objeto, que pode conter várias propriedades e métodos.

Array: Representa uma lista ordenada de elementos.

Function: Representa um bloco de código reutilizável que pode ser chamado por meio de um nome ou uma variável.

### Declaração de Variáveis

Para armazenar valores em JavaScript, é necessário declarar variáveis. As variáveis podem ser declaradas usando as palavras-chave let, const ou var (este último é menos recomendado em aplicações modernas). Por exemplo:
 
> let idade = 25; // Variável do tipo number

> const nome = 'Ana'; // Variável do tipo string, com valor constante (imutável)

> let ativo = true; // Variável do tipo boolean

### Conversão de Tipos (Type Coercion)

JavaScript é uma linguagem de tipagem dinâmica e fraca, o que significa que as conversões de tipos podem ocorrer automaticamente em algumas situações. Por exemplo:

> let numero = 42;

> let texto = "O número é: " + numero; // Conversão automática para string

> console.log(texto); // Saída: "O número é: 42"

Operações com Diferentes Tipos de Dados
Ao realizar operações com diferentes tipos de dados, JavaScript pode apresentar resultados inesperados devido à tipagem fraca. Por isso, é importante estar atento ao realizar comparações e operações aritméticas.

### Conclusão
Neste capítulo, aprendemos sobre os tipos de dados em JavaScript, como declarar variáveis e como ocorre a conversão de tipos. Compreender esses conceitos é fundamental para escrever código eficiente e evitar erros comuns. Em capítulos futuros, exploraremos mais a fundo cada tipo de dado e suas particularidades, bem como técnicas avançadas para lidar com variáveis em JavaScript.


## Objeto
JavaScript é uma linguagem orientada a objetos. Isso significa que, em vez de ter funções definidas globalmente para operar em valores de vários tipos, os próprios tipos definem métodos para trabalhar com valores. Para classificar os elementos de um array a, por exemplo, não passamos a para uma função sort(). Em vez disso, chamamos o método sort() de a: a.sort(); // A versão orientada a objetos de sort(a). A definição de método é abordada no Capítulo 9. Tecnicamente, em JavaScript apenas os objetos possuem métodos. Mas números, strings e valores booleanos se comportam como se tivessem métodos (a Seção 3.6 explica como isso funciona). Em JavaScript, null e undefined são os únicos valores em que métodos não podem ser chamados.

(Página 29). 


JavaScript define outro tipo especial de objeto, conhecido como função. Uma função é um objeto que tem código executável associado. Uma função pode ser chamada para executar esse código executável e retornar um valor calculado. Assim como os arrays, as funções se comportam de maneira diferente dos outros tipos de objetos, sendo que JavaScript define uma sintaxe especial para trabalhar com elas. O mais importante a respeito das funções em JavaScript é que elas são valores reais e os programas em JavaScript podem tratá-las como objetos normais. As funções são abordadas no Capítulo 8.

(Página 29). 
Um objeto normal em JavaScript é um conjunto não ordenado de valores nomeados. A linguagem também define um tipo especial de objeto, conhecido como __array__, que representa um conjunto ordenado de valores numerados. 

Um objeto (isto é, um membro do tipo objeto) é um conjunto de propriedades, em que cada propriedade tem um nome e um valor (ou um valor primitivo, como um número ou string, ou um objeto).


(Página 28). objeto 112 - 135 
O interpretador JavaScript realiza a coleta de lixo automática para gerenciamento de memória. Isso significa que um programa pode criar objetos conforme for necessário e o programador nunca precisa se preocupar com a destruição ou desalocação desses objetos. Quando um objeto não pode mais ser acessado – quando um programa não tem mais maneira alguma de se referir a ele –, o interpretador sabe que ele nunca mais pode ser utilizado e recupera automaticamente o espaço de memória que ele estava ocupando.

As funções que são escritas para serem usadas (com o operador new) para inicializar um objeto criado recentemente são conhecidas como construtoras. Cada construtora define uma classe de objetos – o conjunto de objetos inicializados por essa construtora. As classes podem ser consideradas como subtipos do tipo de objeto. Além das classes Array e Function, JavaScript básica define outras três classes úteis. A classe Date define objetos que representam datas. A classe RegExp define objetos que representam expressões regulares (uma poderosa ferramenta de comparação de padrões, descrita no Capítulo 10). E a classe Error define objetos que representam erros de sintaxe e de execução que podem ocorrer em um programa JavaScript.

JavaScript básico inclui uma construtora Date() para criar objetos que representam datas e horas. Esses objetos Date têm métodos que fornecem uma API para cálculos simples de data. Os objetos Date não são um tipo fundamental como os números. Esta seção apresenta um estudo rápido sobre o trabalho com datas. Detalhes completos podem ser encontrados na seção de referência:

(Página 34). 

## ARRAY 


A linguagem JavaScript contém sintaxe especial para trabalhar com arrays, sendo que os arrays têm um comportamento especial que os diferencia dos objetos normais. Os arrays são o tema do Capítulo 7.