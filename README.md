# Logbook for JavaScript
Logbook for Programming Languages ​​and Paradigms

## Índice

1. [Introdução](#introdução)
2. [Método de Implementação](#método-de-implementação)
3. [Precedência e Associatividade de Operadores](#precedência-e-associatividade-de-operadores)

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

2. __Compilação Just-in-Time (JIT):__ O interpretador JavaScript, presente no navegador ou no ambiente de execução, compila o código AST em código de byte, que é uma representação intermediária.

3. __Execução:__ O código de byte gerado é interpretado e executado pelo mecanismo JavaScript do navegador ou do ambiente de execução.

A interpretação do JavaScript traz algumas vantagens, como a portabilidade do código, pois não há necessidade de recompilação para diferentes plataformas, e facilita a depuração, pois os erros podem ser identificados linha por linha.

No entanto, a interpretação pode ser mais lenta em comparação com linguagens compiladas, especialmente para operações intensivas em processamento. Para melhorar o desempenho, os navegadores modernos também usam otimização JIT, que transforma trechos de código frequentemente usados em código nativo otimizado para a plataforma em questão, acelerando sua execução.

Em resumo, JavaScript é uma linguagem interpretada, o que significa que o código é executado diretamente sem uma etapa explícita de compilação em código de máquina.

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

**: Exponenciação.
*, /, %: Multiplicação, divisão e resto da divisão.
+, -: Adição e subtração.
Operadores de comparação:

>, <, >=, <=: Maior que, menor que, maior ou igual a, menor ou igual a.
==, !=, ===, !==: Igualdade e desigualdade.
in, instanceof: Operadores especiais de comparação.
Operadores lógicos:

&&: E lógico.
||: OU lógico.
!: Negação lógica.
Operador ternário:

? :: Operador ternário condicional.
Associatividade:
A associatividade determina a direção em que os operadores são agrupados quando têm a mesma precedência. Em JavaScript, a maioria dos operadores é associativa da esquerda para a direita, o que significa que as operações são realizadas da esquerda para a direita. No entanto, o operador de exponenciação ** é associativo da direita para a esquerda, o que significa que as operações são realizadas da direita para a esquerda.

É importante lembrar que, se você estiver usando diferentes operadores na mesma expressão, é fundamental conhecer a precedência e associatividade para garantir que a expressão seja avaliada corretamente. Caso seja necessário alterar a ordem de avaliação, é possível usar parênteses para agrupar as operações conforme desejado.
