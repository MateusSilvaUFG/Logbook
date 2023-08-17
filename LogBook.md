# Logbook for JavaScript
Logbook for Programming Languages ​​and Paradigms

## Índice

## Índice

1. [Introdução](#introdução)
2. [Método de Implementação](#método-de-implementação)
3. [Precedência e Associatividade de Operadores](#precedência-e-associatividade-de-operadores)
4. [Tipos, valores e variáveis](#tipos-valores-e-variáveis)
   1. [Objeto](#objeto)
   2. [Herança](#herança)
   3. [ARRAY](#array)
   4. [Tipo Registro](#tipo-registro)
   5. [Tipo MAP](#tipo-map)
   6. [Tipo União](#tipo-união)
   7. [Modelo de Programação - DOM](#modelo-de-programação---dom)
   8. [Conversão de Tipos (Type Coercion)](#conversão-de-tipos-type-coercion)
   9. [Verificação de Tipo](#verificação-de-tipo)
   10. [Escopo](#escopo)
   11. [Endereço de Memória](#endereço-de-memória)
   12. [Amarração](#amarracao)
   13. [Tempo de Vida](#tempo-de-vida)
   14. [Variável Estática](#variável-estática)
   15. [Variável Pilha](#variável-pilha)
   16. [Variável Explícita de Heap x Variável Implícita de Heap](#variável-explícita-de-heap-x-variável-implícita-de-heap)
   17. [Literal Numérico](#literal-numérico)
   18. [Tratamento de Erro em JavaScript](#tratamento-de-erro-em-java-script)
5. [Expressões e Operadores](#expressões-e-operadores)
6. [Operadores](#operadores)


# Introdução
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

### Método de Implementação

JavaScript é uma linguagem de programação interpretada, não uma linguagem compilada. Isso significa que, em vez de ser compilado em código de máquina antes da execução, o código JavaScript é lido e executado linha por linha por um interpretador no navegador ou no ambiente em que está sendo executado.

O processo de execução do JavaScript ocorre da seguinte maneira:

1. __Análise léxica e sintática:__ O código JavaScript é lido e dividido em elementos léxicos, como palavras-chave, operadores, identificadores, etc. Em seguida, esses elementos são analisados para formar uma estrutura de árvore de sintaxe abstrata (AST).

2. __Compilação Just-in-Time (JIT):__ O interpretador JavaScript, presente no navegador ou no ambiente de execução, compila o código de árvore de sintaxe abstrata (AST) em código de byte, que é uma representação intermediária.

3. __Execução:__ O código de byte gerado é interpretado e executado pelo mecanismo JavaScript do navegador ou do ambiente de execução.

A interpretação do JavaScript traz algumas vantagens, como a portabilidade do código, pois não há necessidade de recompilação para diferentes plataformas, e facilita a depuração, pois os erros podem ser identificados linha por linha.

No entanto, a interpretação pode ser mais lenta em comparação com linguagens compiladas, especialmente para operações intensivas em processamento. Para melhorar o desempenho, os navegadores modernos também usam otimização JIT, que transforma trechos de código frequentemente usados em código nativo otimizado para a plataforma em questão, acelerando sua execução.

# Sintaxa Básica

JavaScript é uma linguagem de programação de alto nível amplamente utilizada para desenvolvimento web e outras aplicações interativas. A seguir, apresento a sintaxe e a semântica básica do JavaScript:

### Estruruta léxica

A *estrutura léxica* de uma linguagem de programação é o conjunto de regras elementares que especificam o modo de escrever programas nessa linguagem. É a sintaxe de nível mais baixo de uma linguagem; especifica detalhes de como são os nomes de variáveis, os caracteres delimitadores para comentários e como uma instrução do programa é separada da seguinte.

### Declaração de Variáveis (let , const e var):

Para armazenar valores em JavaScript, é necessário declarar variáveis. As variáveis podem ser declaradas usando as palavras-chave __let__, __const__ ou __var__ .

1. __let:__ Variáveis declaradas com let têm escopo de bloco. Isso significa que elas são acessíveis apenas dentro do bloco onde foram declaradas (por exemplo, dentro de um loop for, uma função ou um bloco condicional). Além disso, variáveis let podem ser reatribuídas com novos valores.

    let nome = "Alice";
    nome = "Bob"; // Permitido

2. __const:__ ariáveis declaradas com const também têm escopo de bloco, assim como o let. No entanto, variáveis const não podem ser reatribuídas após a inicialização. Elas são usadas para definir valores constantes que não devem ser alterados ao longo do tempo.

    const pi = 3.14159;
    pi = 3.14; // Erro: não é permitido reatribuir uma constante

3. __var:__ A declaração var tinha sido amplamente usada antes da introdução de let e const. Variáveis declaradas com var têm escopo de função ou escopo global, não de bloco. Isso pode levar a problemas de escopo inesperados em situações complexas. Além disso, variáveis var podem ser reatribuídas e atualizadas livremente.

    var contador = 1;
    if (true) {
      var contador = 2; // Mesma variável "contador" do escopo externo
    }
    console.log(contador); // Imprimirá 2

### identificadores

Em JavaScript, um identificador é um nome utilizado para identificar variáveis, funções, classes ou qualquer outro elemento nomeado dentro do código. Em outras palavras, é um nome que você escolhe para dar a uma entidade (variável, função, objeto, etc.) para poder referenciá-la e utilizá-la em seu programa.

Ao declarar variáveis em JavaScript, é importante seguir algumas regras para garantir que o código seja válido e compreensível. Aqui estão as principais regras para declarar nomes de variáveis em JavaScript:

1. __Sintaxe:__
* Os nomes de variáveis devem começar com uma letra (maiúscula ou minúscula), _ (underscore) ou $ (cifrão). Ele não pode começar com um dígito.
* Após o primeiro caractere, você pode usar letras, números, _ ou $.
* Não é permitido o uso de espaços em um identificador.

2. __Case-Sensitivity:__
* JavaScript é sensível a maiúsculas e minúsculas, o que significa que minhaVariavel e MinhaVariavel são consideradas diferentes.
* Palavras-chave, variáveis, nomes de função e outros identificadores da linguagem sempre devem ser digitados com a composição compatível de letras. A palavra-chave while, por exemplo, deve ser digitada como “while” e não como “While” ou “WHILE.” Da mesma forma, online, Online, OnLine e ONLINE, são quatro nomes de variável distintos.

3. __Palavras Reservadas:__
* Você não pode usar palavras reservadas do JavaScript como nomes de variáveis. Por exemplo, não é possível criar uma variável chamada function, if, else, for, entre outras.
* O identificador pode ser qualquer sequência de caracteres válidos que não seja uma palavra reservada (palavras que possuem significado específico na linguagem e não podem ser usadas como identificadores).

4. __Boas Práticas de Nomenclatura:__
* Use nomes significativos que descrevam o propósito da variável.
* Use camelCase para nomes de variáveis compostos, onde a primeira palavra começa com minúscula e as palavras subsequentes começam com maiúscula (por exemplo, nomeDoUsuario).
* Evite usar nomes muito curtos ou muito genéricos, pois isso pode dificultar a compreensão do código.
* Use nomes descritivos em vez de abreviações obscuras.

5. __Unicode:__
* JavaScript suporta caracteres Unicode em nomes de variáveis. Isso permite usar caracteres acentuados, símbolos e outros caracteres Unicode, mas não é recomendado para manter a legibilidade.
Exemplos válidos de declaração de variáveis:

Exemplos válidos de declaração de variáveis e sintaxe básica:

Exemplos de identificadores válidos em JavaScript:

      let nome;
      const idade;
      const _variavel;
      const $preco;
      let contador123;
      const minhaFuncao;

Exemplos de identificadores inválidos (que causariam erro de sintaxe):

      let 123abc; // Não pode começar com dígito
      let minha variavel; // Não pode conter espaços
      const break; // "break" é uma palavra reservada em JavaScript

1. Comentários:

### Comentários

JavaScript aceita dois estilos de comentários. 
* Qualquer texto entre // e o final de uma linha é tratado como comentário e é ignorado por JavaScript. 
* Qualquer texto entre os caracteres /* e */ também étratado como comentário; esses comentários podem abranger várias linhas, mas não podem ser aninhados. As linhas de código a seguir são todas comentários JavaScript válidos:

        // Este é um comentário de uma linha.
        /* Este também é um comentário */ // e aqui está outro comentário.
        /*
        * Este é ainda outro comentário.
        * Ele tem várias linhas.
        */

2. Variáveis e Atribuição:

        let nome = "Alice";
        const idade = 25;
        var contador = 0; // Escopo global (menos recomendado)

3. Tipos de Dados:

        let numero = 42;          // Número
        let texto = "Olá, mundo"; // String
        let booleano = true;      // Booleano (true/false)
        let nulo = null;          // Valor nulo
        let indefinido;           // Valor indefinido
        let objeto = { chave: "valor" }; // Objeto
        let array = [1, 2, 3];     // Array

4. Operadores Aritméticos:

        let soma = 5 + 3;
        let subtracao = 10 - 4;
        let multiplicacao = 6 * 2;
        let divisao = 12 / 3;
        let modulo = 7 % 3; // Resto da divisão

5. peradores de Comparação:

        let igualdade = 5 === "5"; // Igualdade estrita (valor e tipo)
        let desigualdade = 10 !== 5; // Diferente estrito
        let maior = 7 > 3;
        let menorOuIgual = 4 <= 4;

### Estruturas de Controle: 

* Condicional if:

      if (condicao) {
        // Código executado se a condição for verdadeira
      } else {
        // Código executado se a condição for falsa
      }
* Loop for:

        for (let i = 0; i < 5; i++) {
        // Código executado em cada iteração
      }

* Loop while:

      let contador = 0;

      while (contador < 5) {
        console.log("Contador: " + contador);
        contador++;
      }


### Funções:

      function saudacao(nome) {
        return "Olá, " + nome;
      }
      
      let mensagem = saudacao("Alice"); // Retorna "Olá, Alice"

### conjunto de caracteres

Os programas JavaScript são escritos com o conjunto de caracteres Unicode. Unicode é um superconjunto de ASCII e Latin-1 e suporta praticamente todos os idiomas escritos usados hoje no planeta.

### Sequências de escape Unicode

Alguns componentes de hardware e software de computador não conseguem exibir ou introduzir o conjunto completo de caracteres Unicode. Para ajudar os programadores que utilizam essa tecnologia mais antiga, JavaScript define sequências especiais de seis caracteres ASCII para representar qualquer código Unicode de 16 bits.

Esses escapes Unicode começam com os caracteres \u e são seguidos
por exatamente quatro dígitos hexadecimais (usando as letras A–F maiúsculas ou minúsculas). Os escapes Unicode podem aparecer em strings literais, expressões regulares literais e em identificadores
JavaScript (mas não em palavras-chave da linguagem). O escape Unicode para o caractere “é”, por exemplo, é \u00E9, e as duas strings JavaScript a seguir são idênticas:

      "café" === "caf\u00e9" // => true
  
Os escapes Unicode também podem aparecer em comentários, mas como os comentários são ignorados, eles são tratados como caracteres ASCII nesse contexto e não são interpretados como Unicode.

### Normalização

O Unicode permite mais de uma maneira de codificar o mesmo caractere. A string “é”, por exemplo, pode ser codificada como o caractere Unicode \u00E9 ou como um caractere ASCII “e” normal, seguido da marca de combinação de acento agudo \u0301.

Essas duas codificações podem parecer exatamente a mesma quando exibidas por um editor de textos, mas têm diferentes codificações binárias e são consideradas diferentes pelo computador. 

O padrão Unicode define a codificação preferida para todos os caracteres e especifica um procedimento de normalização para converter texto em uma forma canônica conveniente para comparações. JavaScript presume que o código-fonte que está interpretando já foi normalizado e não tenta normalizar identificadores, strings nem expressões regulare.

### Literais

Um literal é um valor de dados que aparece diretamente em um programa. Os valores seguintes são todos literais:

      12 // O número doze
      1.2 // O número um ponto dois
      "hello world" // Uma string de texto
      'Hi' // Outra string
      true // Um valor booleano
      false // O outro valor booleano
      /javascript/gi // Uma "expressão regular" literal (para comparação de padrões)
      null // Ausência de um objeto

### Pontos e vírgulas opcionais.

Muitos programadores JavaScript (e o código deste livro) utilizam pontos e vírgulas para marcar explicitamente os finais de instruções, mesmo onde eles não são obrigatórios. Outro estilo é omitir os pontos
e vírgulas quando possível, utilizando-os nas poucas situações que os encorajaram. Qualquer que seja o
estilo escolhido, existem alguns detalhes que você deve entender sobre os pontos e virgulas opções
em JavaScript.
Considere o código a seguir. Como as duas instruções aparecem em linhas separadas, o primeiro
ponto e virgula poderia ser omitido:

      a = 3;
      b = 4;
      Contudo, escrito como a seguir, o primeiro ponto e vírgula é obrigatório:
      a = 3; b = 4;

Observe que JavaScript não trata toda quebra de linha como ponto e vírgula: ela normalmente trata como
quebras de linha como pontos e vírgulas somente se não conseguir analisar o código sem os pontos e
vírgulas. Mais formalmente (e com as duas características, descritas a seguir), JavaScript trata uma quebra
de linha como ponto e virgula caso o próximo caractere que não seja espaço não possa ser interpretado como a continuação da instrução corrente. Considere o código a seguir:


      var a
      a
      =
      3
      console.log(a)

JavaScript interpreta esse código como segue:
var a; a = 3; console.log(a);

### Palavras reservadas

Em JavaScript, palavras reservadas (ou "keywords") são termos que têm um significado especial na linguagem e são usados para declarar estruturas de controle, tipos de dados, funções, entre outros elementos fundamentais da sintaxe do JavaScript. Essas palavras têm um propósito específico na linguagem e não podem ser usadas como nomes de variáveis, funções ou objetos, pois isso levaria a erros de sintaxe.

As palavras reservadas em JavaScript incluem:

    break      case       catch      class      const
    continue   debugger   default    delete     do
    else       export     extends    false      finally
    for        function   if         import     in
    instanceof new        null       return     super
    switch     this       throw      true       try
    typeof     var        void       while      with
    yield

      
# Semântica Básica:

JavaScript é uma linguagem de programação interpretada, o que significa que o código é executado diretamente pelo interpretador do navegador ou ambiente de execução. A semântica básica do JavaScript inclui:

* O fluxo de controle é determinado pelas estruturas de controle condicional (if/else) e de loop (for, while).
* As variáveis são tipadas dinamicamente, o que significa que você não precisa declarar explicitamente o tipo.
* Valores undefined e null são usados para representar valores ausentes ou não definidos.
* Os objetos são usados para agrupar valores relacionados em pares chave-valor.
* Funções permitem a reutilização de código e podem ser passadas como argumentos ou retornadas de outras funções.


As abordagens de semântica abordadas na aula de Linguagens e Paradigmas de Programação são (estática, dinâmica, operacional e denotacional), todas podem ser aplicadas à linguagem de programação JavaScript, mas algumas delas são mais relevantes ou comumente usadas do que outras.

Semântica Estática: Essa abordagem é muito aplicável em JavaScript, especialmente com o uso do TypeScript. O TypeScript é um superconjunto de JavaScript que adiciona verificações de tipo estático, o que ajuda a identificar erros de tipos antes mesmo da execução. Além disso, ferramentas de linting (como ESLint) também fornecem análise estática para identificar problemas de estilo e possíveis erros de código.

Semântica Dinâmica: Como JavaScript é uma linguagem de script que é executada em tempo de execução (no navegador, por exemplo), a semântica dinâmica é uma parte fundamental do seu comportamento. Isso inclui a execução de funções, gerenciamento de escopo, manipulação de eventos, interação com o DOM e assim por diante.

Logo, a semântica estática e dinâmica são as mais relevantes e amplamente aplicadas em JavaScript. A semântica operacional pode ser útil para entender detalhes de execução e comportamento, enquanto a semântica denotacional é menos comum, mas ainda pode ser explorada em um contexto mais acadêmico ou teórico.

# Precedência e Associatividade de Operadores

Em JavaScript, os operadores têm uma precedência e associatividade específica, o que determina a ordem em que as operações são realizadas em uma expressão com múltiplos operadores. É importante entender a precedência e associatividade dos operadores para garantir que as expressões sejam avaliadas corretamente.

### Precedência:

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

### Associatividade:

A associatividade determina a direção em que os operadores são agrupados quando têm a mesma precedência. Em JavaScript, a maioria dos operadores é associativa da esquerda para a direita, o que significa que as operações são realizadas da esquerda para a direita. No entanto, o operador de exponenciação ** é associativo da direita para a esquerda, o que significa que as operações são realizadas da direita para a esquerda.

É importante lembrar que, se você estiver usando diferentes operadores na mesma expressão, é fundamental conhecer a precedência e associatividade para garantir que a expressão seja avaliada corretamente. Caso seja necessário alterar a ordem de avaliação, é possível usar parênteses para agrupar as operações conforme desejado.

| Precedência | Operadores                    | Associatividade |
|-------------|------------------------------|-----------------|
| 19          | `()` (parênteses)             | -               |
| 18          | `.` (acesso a propriedades)   | Esquerda para Direita |
| 17          | `[]` (acesso a índices)       | Esquerda para Direita |
| 16          | `++`, `--` (pós-incremento/decremento) | - |
|             | `-` (unário), `+` (unário), `~` (bitwise NOT), `!` (lógico NOT) | - |
|             | `typeof`, `void`, `delete`   | -               |
|             | `await` (usado com `async` functions) | - |
| 15          | `**` (exponenciação)          | Direita para Esquerda |
| 14          | `*`, `/`, `%` (multiplicação, divisão, resto) | Esquerda para Direita |
| 13          | `+`, `-` (adição, subtração) | Esquerda para Direita |
| 12          | `<<`, `>>`, `>>>` (shifts)   | Esquerda para Direita |
| 11          | `<`, `<=`, `>`, `>=`, `in`, `instanceof` | - |
| 10          | `==`, `!=`, `===`, `!==` (igualdade) | - |
| 9           | `&` (bitwise AND)             | Esquerda para Direita |
| 8           | `^` (bitwise XOR)             | Esquerda para Direita |
| 7           | `|` (bitwise OR)              | Esquerda para Direita |
| 6           | `&&` (lógico AND)             | Esquerda para Direita |
| 5           | `||` (lógico OR)              | Esquerda para Direita |
| 4           | `? :` (operador ternário)     | Direita para Esquerda |
| 3           | `=`, `+=`, `-=`, `*=`, `/=`, `%=`, etc. (atribuição) | Direita para Esquerda |
| 2           | `,` (separador de expressões) | Esquerda para Direita |

A tabela acima é uma simplificação, e pode ser usado parênteses para controlar explicitamente a ordem das operações em expressões complexas.

Por exemplo:

      let resultado = 3 + 4 * 2; // Aqui, a multiplicação (precedência 14) ocorre antes da adição (precedência 13)

No entanto:

      let resultado = (3 + 4) * 2; // Aqui, os parênteses definem a ordem das operações

# Tipos de Dados

Os tipos de JavaScript podem ser divididos em duas categorias: __tipos primitivos__ e __tipos de objeto__. E podem ser divididos em __tipos com métodos__ e __tipos sem métodos__. 

Qualquer valor em JavaScript que não seja número, string, booleano, null ou undefined é um objeto. 

As variáveis em JavaScript são __não tipadas__: você pode atribuir um valor de qualquer tipo a uma variável e, posteriormente, atribuir um valor de tipo diferente para a mesma variável. As variáveis são declaradas com a palavra-chave var. 

JavaScript utiliza __escopo léxico__. As variáveis declaradas fora de uma função são variáveis globais e são visíveis por toda parte em um programa JavaScript. As variáveis declaradas dentro de uma função têm escopo de função e são visíveis apenas para o código que aparece dentro dessa função. 

1. Number;
2. String;
3. Boolean:
4. Undefined: 
5. Null: 
6. Object: 
7. Array: 
8. Function: 


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

### 3 - Booleana:
Um valor booleano representa verdadeiro ou falso, ligado ou desligado, sim ou não. Só existem dois valores possíveis desse tipo. As palavras reservadas __true__ e __false__ são avaliadas nesses dois valores. Geralmente, os valores booleanos resultam de comparações feitas nos programas JavaScript.

### null e undefined
__Undefined__ O valor undefined é usado para indicar que uma variável foi declarada, mas ainda não foi atribuída a nenhum valor, mas de forma implícita. Quando uma variável é declarada, mas não inicializada, seu valor padrão é undefined. Quando você tenta acessar uma variável que não foi inicializada ou não tem valor atribuído, ela retorna undefined.

    let idade; // Variável idade está declarada, mas ainda não possui valor, portanto, seu valor é undefined
    console.log(idade); // Saída: undefined


__Null__ É um tipo primitivo em JavaScript e representa explicitamente a ausência de valor. Ao contrário do undefined, null é um valor atribuível. Isso significa que você pode explicitamente definir uma variável para ter o valor null.

    let nome = null; // Variável nome tem valor null (ausência intencional de valor)

### 6 - Objeto

m JavaScript, um objeto é uma coleção de propriedades, onde cada propriedade tem um nome (chave) e um valor associado. Os objetos são uma estrutura de dados central na linguagem, e eles podem representar entidades do mundo real, conceitos abstratos ou até mesmo abstrações complexas.

Os objetos podem ser criados com objetos literais, com a palavra-chave new e (em ECMAScript 5) com a função __Object.create().__

#### Objetos literais

Um objeto literal é uma lista separada com vírgulas de pares nome:valor separados por dois-pontos, colocados entre chaves. Um nome de propriedade é um identificador JavaScript ou uma string literal (a string vazia é permitida).

Exemplos:

    var empty = {}; // Um objeto sem propriedades
    var point = { x:0, y:0 }; // Duas propriedades
    var point2 = { x:point.x, y:point.y+1 }; // Valores mais complexos
    var book = {
    "main title": "JavaScript", // Os nomes de propriedade incluem espaços,
    'sub-title': "The Definitive Guide", // e hifens; portanto, usam strings literais
    "for": "all audiences", // for é uma palavra reservada; portanto, usa
    // aspas
    author: { // O valor dessa propriedade é
    firstname: "David", // ele próprio um objeto. Note que
    surname: "Flanagan" // esses nomes de propriedade não têm aspas.
    }
    };

#### Criando objetos com new

O operador new cria e inicializa um novo objeto. A palavra-chave new deve ser seguida de uma chamada de função. Uma função usada dessa maneira é chamada de construtora e serve para inicializar um objeto recém-criado.

    var o = new Object(); // Cria um objeto vazio: o mesmo que {}.
    var a = new Array(); // Cria um array vazio: o mesmo que [].
    var d = new Date(); // Cria um objeto Date representando a hora atual
    var r = new RegExp("js"); // Cria um objeto RegExp para comparação de padrões.

#### Protótipos

Protótipos são um conceito fundamental em JavaScript que permite a herança e a reutilização de propriedades e métodos entre objetos. O sistema de protótipos é uma das características que diferencia JavaScript de muitas outras linguagens de programação.

Quando um objeto é criado em JavaScript, ele pode herdar propriedades e métodos de um protótipo. Cada objeto em JavaScript tem um protótipo associado a ele, que pode ser outro objeto ou null. Se uma propriedade ou método não for encontrado no objeto atual, o mecanismo de protótipos irá procurar essa propriedade ou método no protótipo.

__Sistema de protótipos em JavaScript:__

    let animal = {
      fazerSom: function() {
        console.log("Som genérico");
      }
    };

    let cachorro = Object.create(animal);
    cachorro.fazerSom(); // Saída: "Som genérico"

#### Consultando e configurando propriedades

Para obter o valor de uma propriedade, use os operadores ponto (.) ou colchete ([]), d O lado esquerdo deve ser uma expressão cujo valor é um objeto. 
* Se for usado o operador ponto, o lado direito deve ser um identificador simples que dê nome à propriedade.
* Se forem usados colchetes, o valor dentro deles deve ser uma expressão avaliada como uma string contendo o nome da propriedade desejada:

      var author = book.author; // Obtém a propriedade "author" de book.
      var name = author.surname // Obtém a propriedade "surname" de author.
      var title = book["main title"] // Obtém a propriedade "main title" de book.

Para criar ou configurar uma propriedade, use um ponto ou colchetes, como faria para consultar a propriedade, mas coloque-os no lado esquerdo de uma expressão de atribuição:

    book.edition = 6; // Cria uma propriedade "edition" de book.
    book["main title"] = "ECMAScript"; // Configura a propriedade "main title".

#### Herança 

Em JavaScript, a herança simples baseada em protótipos é implementada de forma natural. Cada objeto possui apenas um único protótipo, e as propriedades e métodos são buscados primeiro no objeto e depois na cadeia de protótipos. Isso evita problemas de ambiguidade e torna a herança mais simples e previsível.

1. __Herança Baseada em Protótipos:__ Essa é a forma nativa de herança em JavaScript, aproveitando o sistema de protótipos. Você pode criar um objeto e estabelecer um outro objeto como seu protótipo.

        let animal = {
          fazerSom: function() {
            console.log("Som genérico");
          }
        };

        let cachorro = Object.create(animal);
        cachorro.fazerSom(); // Saída: "Som genérico"

2. __class:__ O ES6 introduziu a sintaxe de classe em JavaScript, que é uma forma mais amigável de criar objetos com herança. As classes são uma abstração sobre a herança baseada em protótipos.

        class Animal {
          fazerSom() {
            console.log("Som genérico");
          }
        }

        class Cachorro extends Animal {
          constructor(nome) {
            super();
            this.nome = nome;
          }
        }

        let meuCachorro = new Cachorro("Rex");
        meuCachorro.fazerSom(); // Saída: "Som genérico"



### 7 - ARRAY 

Em JavaScript, um array é uma estrutura de dados que permite armazenar e acessar múltiplos valores em uma única variável. Os arrays são especialmente úteis quando você precisa lidar com uma coleção de elementos, como números, strings, objetos ou até mesmo outros arrays.

Aqui estão algumas características dos arrays em JavaScript:

1. __Criando um Array:__ Você pode criar um array utilizando a sintaxe de colchetes []. Dentro dos colchetes, você pode listar os elementos do array separados por vírgulas.

        let numeros = [1, 2, 3, 4, 5];
        let frutas = ["maçã", "banana", "laranja"];

2. __Acessando Elementos:__ Você pode acessar os elementos de um array utilizando um índice numérico, começando a contagem a partir de zero.

        console.log(numeros[0]); // Saída: 1
        console.log(frutas[1]); // Saída: "banana"

3. __Modificando Elementos:__ Você pode modificar os valores dos elementos de um array simplesmente atribuindo um novo valor ao índice correspondente.

        numeros[2] = 10;
        console.log(numeros); // Saída: [1, 2, 10, 4, 5]

4. __Propriedade length:__ O array possui uma propriedade chamada length que indica o número de elementos no array.

        console.log(frutas.length); // Saída: 3

5. __Métodos de Array:__ JavaScript oferece uma série de métodos embutidos para manipular arrays, como push, pop, shift, unshift, splice, concat, slice, forEach, entre outros.

        frutas.push("morango"); // Adiciona "morango" ao final do array
        frutas.pop(); // Remove o último elemento do array

6. __Arrays de Objetos:__ Você pode criar arrays que contenham objetos como elementos.

        let pessoas = [
          { nome: "Alice", idade: 30 },
          { nome: "Bob", idade: 25 }
        ];


### 8  - Function

Function: Representa um bloco de código reutilizável que pode ser chamado por meio de um nome ou uma variável.

    function saudacao(nome) {
      console.log(`Olá,eu sou o ${nome}!.`);
    }

    // Chamando a função
    saudacao("Mateus");


### Tipo Registro

Em JavaScript, você pode criar objetos que são coleções de pares chave-valor, onde as chaves são strings (ou símbolos) que representam os campos e os valores são os dados associados a esses campos. Essa é uma maneira eficaz de criar estruturas de dados semelhantes a registros. Aqui está um exemplo de como criar e usar um objeto em JavaScript:

    // Criando um objeto representando informações de uma pessoa
    var pessoa = {
    nome: "João",
    idade: 30,
    profissao: "Desenvolvedor"
    };

    // Acessando campos do objeto
    console.log(pessoa.nome);      // Saída: João
    console.log(pessoa.idade);     // Saída: 30
    console.log(pessoa.profissao); // Saída: Desenvolvedor

Além disso, a partir do ECMAScript 2015 (ES6), JavaScript também introduziu o tipo de dado "Map" que permite criar coleções de pares chave-valor, semelhantes a registros, com algumas funcionalidades adicionais em comparação com objetos.

Portanto, embora JavaScript não possua um tipo de dado específico chamado "Registro", a flexibilidade dos objetos e a introdução dos "Maps" permitem que você crie estruturas de dados semelhantes a registros para armazenar informações relacionadas.

### Tipo MAP

Em JavaScript, o tipo de dado "Map" é uma estrutura que permite armazenar coleções de pares chave-valor, onde tanto as chaves quanto os valores podem ser de qualquer tipo. O "Map" é uma alternativa mais flexível e poderosa aos objetos quando se trata de criar estruturas de dados complexas que requerem mapeamento de chaves para valores.

A principal diferença entre "Map" e objetos em JavaScript é que os "Map" permitem usar qualquer tipo de dado como chave, incluindo tipos de dados complexos como objetos e funções, enquanto os objetos permitem apenas usar strings e símbolos como chaves.

Exemplo de como criar e usar um "Map" em JavaScript:

    // Criando um Map
    var meuMap = new Map();

    // Adicionando elementos ao Map
    meuMap.set("chave1", "valor1");
    meuMap.set(123, "valor2");
    meuMap.set({ nome: "Alice" }, "valor3");

    // Acessando elementos no Map
    console.log(meuMap.get("chave1")); // Saída: valor1
    console.log(meuMap.get(123));      // Saída: valor2
    console.log(meuMap.get({ nome: "Alice" })); // Saída: valor3 (devido à referência de objeto)

    // Verificando a existência de uma chave no Map
    console.log(meuMap.has("chave1")); // Saída: true

    // Removendo um elemento do Map
    meuMap.delete(123);

    // Tamanho do Map
    console.log(meuMap.size); // Saída: 2

Ao usar "Map", você pode mapear praticamente qualquer tipo de dado a um valor correspondente e aproveitar métodos como set, get, has, delete, entre outros, para manipular a coleção. "Map" é especialmente útil quando você precisa armazenar pares chave-valor e a flexibilidade das chaves é importante.

###  Tipo União
O tipo união (também conhecido como união de tipos ou union type em inglês) é um conceito em programação de computadores que permite que uma variável, parâmetro ou propriedade possa conter valores de diferentes tipos

JavaScript não possui nativamente um tipo de dado chamado "União" (Union type) como é encontrado em algumas outras linguagens de programação, como TypeScript ou Kotlin. Um tipo de união permite que uma variável possa conter valores de diferentes tipos especificados.

No entanto, em JavaScript, as variáveis são tipadas dinamicamente, o que significa que uma mesma variável pode conter diferentes tipos de dados ao longo do tempo. Por exemplo, uma variável pode conter um número em um momento e, mais tarde, ser atribuída a uma string.

Embora JavaScript não tenha tipos de união incorporados como em outras linguagens, você pode simular comportamentos semelhantes usando lógica condicional e métodos de verificação de tipos. Por exemplo:

    let valor;

    if (condicao) {
    valor = 42;  // atribui um número
    } else {
    valor = "Olá"; // atribui uma string
    }

# modelo de programação - DOM 
O DOM (Document Object Model) em JavaScript é uma representação hierárquica dos elementos HTML (ou XML) de uma página da web. Ele permite que os scripts em JavaScript interajam com os elementos e o conteúdo de uma página, alterando dinamicamente a estrutura, o estilo e o comportamento do documento. O DOM é uma parte fundamental da programação web e é amplamente usado para criar interatividade e dinamismo nas páginas da web.

conceitos relacionados ao DOM em JavaScript:

__Árvore DOM:__ O DOM organiza os elementos HTML (como tags __div__, __p__, __h1__, etc.) em uma estrutura de árvore. Cada elemento é representado como um nó na árvore, com o nó raiz representando o documento inteiro. Os elementos podem ter filhos (elementos aninhados) e irmãos (elementos no mesmo nível hierárquico).

__Acesso e Manipulação:__ Com JavaScript, você pode acessar e manipular o DOM usando métodos e propriedades fornecidos pela API do DOM. Isso inclui alterar conteúdo, estilos, atributos e até mesmo adicionar ou remover elementos da página.

__Seleção de Elementos:__ Para interagir com elementos específicos, você pode usar métodos como getElementById, querySelector, querySelectorAll para selecionar elementos com base em seus identificadores, classes, nomes de tag e outros seletores CSS.

__Eventos:__ O DOM permite que você associe eventos a elementos, como cliques de mouse, pressionamentos de tecla e muito mais. Você pode usar os métodos addEventListener ou atributos de eventos HTML para lidar com eventos e executar ações específicas quando eles ocorrem.

__Alteração de Conteúdo:__ Você pode modificar o conteúdo de um elemento, como textos e HTML interno, usando propriedades como textContent e innerHTML.

__Estilos CSS:__ O DOM permite a manipulação de estilos CSS de elementos usando propriedades como style. Você pode alterar cores, tamanhos, margens e outros estilos diretamente por meio do JavaScript.

__Adição e Remoção de Elementos:__ Você pode criar novos elementos usando o método createElement e adicioná-los ao DOM com appendChild ou insertBefore. Também é possível remover elementos usando o método removeChild.

__Manipulação de Atributos:__  Você pode alterar ou obter valores de atributos de elementos usando métodos como getAttribute, setAttribute e removeAttribute.

__Navegação no DOM:__ Você pode navegar pelo DOM movendo-se entre os elementos pai, filhos e irmãos usando propriedades como parentNode, childNodes, nextSibling e previousSibling.

O DOM é uma parte essencial da programação JavaScript para a web e permite que os desenvolvedores criem páginas interativas e dinâmicas. Ao compreender e usar efetivamente o DOM, você pode criar experiências de usuário mais envolventes e funcionais.

### Conversão de Tipos (Type Coercion)

JavaScript é uma linguagem de tipagem dinâmica e fraca, o que significa que as conversões de tipos podem ocorrer automaticamente __(conversão implicita)__ em algumas situações. Por exemplo:

    x + "" // O mesmo que String(x)
    +x // O mesmo que Number(x). Você também poderá ver x-0
    !!x // O mesmo que Boolean(x). Observe o duplo !
 
    let numero = 42;
    let texto = "O número é: " + numero; // Conversão automática para string
    console.log(texto); // Saída: "O número é: 42"

Operações com Diferentes Tipos de Dados
Ao realizar operações com diferentes tipos de dados, JavaScript pode apresentar resultados inesperados devido à tipagem fraca. Por isso, é importante estar atento ao realizar comparações e operações aritméticas.

| Valor            | String         | Número | Booleano | Objeto              |
|------------------|----------------|--------|----------|---------------------|
| `undefined`      | "undefined"    | NaN    | false    | Lança TypeError     |
| `null`           | "null"         | 0      | false    | Lança TypeError     |
| `true`           | "true"         | 1      | true     | `new Boolean(true)`|
| `false`          | "false"        | 0      | false    | `new Boolean(false)`|
| "" (string vazia)| ""             | 0      | false    | `new String("")`    |
|"1.2" (não vazia,numéro)| | 1.2| true | new String ("1.2")|


A conversão explícita, também conhecida como coerção explícita ou __type casting__, em JavaScript é o processo de converter um valor de um tipo de dado para outro tipo de dado de forma deliberada e controlada pelo programador. Isso permite que você trate os dados de maneira específica, garantindo que eles estejam no formato correto antes de executar determinadas operações.

Existem várias maneiras de realizar a conversão explícita em JavaScript, incluindo:

1. Métodos de Conversão:

JavaScript fornece métodos para converter valores entre tipos de dados específicos. Por exemplo:

__Number():__ Converte um valor em um número.
__String():__ Converte um valor em uma string.
__Boolean():__ Converte um valor em um booleano.

Exemplo:

    let numeroString = "42";
    let numero = Number(numeroString); // Convertendo a string "42" para o número 42
    console.log(numero); // Saída: 42

### verificação de tipo 

A verificação de tipo em JavaScript é dinâmica, o que significa que os tipos de dados são associados aos valores em tempo de execução e podem ser alterados ao longo da vida do programa. Isso é diferente das linguagens de programação de tipagem estática, onde os tipos são definidos em tempo de compilação e não podem ser alterados facilmente durante a execução do programa.

Em JavaScript, você não precisa declarar explicitamente o tipo de uma variável ao criar. O tipo é inferido automaticamente com base no valor atribuído. Além disso, você pode alterar o tipo de uma variável simplesmente atribuindo um novo valor de um tipo diferente a ela.

Por exemplo:

    let valor = 42; // "valor" é inferido como um número
    console.log(typeof valor); // Saída: "number"

    valor = "Olá"; // "valor" agora é uma string
    console.log(typeof valor); // Saída: "string"

Essa natureza dinâmica da verificação de tipo em JavaScript oferece flexibilidade, mas também pode levar a erros se não for tratada com cuidado. É importante estar ciente de como os tipos podem mudar em diferentes partes do código e escrever verificações apropriadas para garantir o comportamento esperado.

### Escopo

O escopo de uma variável é a região do código-fonte de seu programa em que ela está definida. Uma variável global tem escopo global; ela está definida em toda parte de seu código JavaScript. Por outro lado, as variáveis declaradas dentro de uma função estão definidas somente dentro do corpo da função. Elas são variáveis locais e têm escopo local. Os parâmetros de função também contam como variáveis locais e estão definidos somente dentro do corpo da função.

Dentro do corpo de uma função, uma variável local tem precedência sobre uma variável global com o mesmo nome. Se você declara uma variável local ou um parâmetro de função com o mesmo nome de uma variável global, ela efetivamente oculta a variável global:

    var scope = "global"; // Declara uma variável global

    function checkscope() {
        var scope = "local"; // Declara uma variável local com o mesmo nome
        return scope; // Retorna o valor local, não o global
    }

    checkscope() // => "local"

Quando uma variável é declarada sem usar as palavras-chave var, let ou const, ela é automaticamente criada no escopo global (em navegadores, ela se torna uma propriedade do objeto global, que é window).

A declaração de uma variável usando var, let ou const dentro de uma função a restringe ao escopo dessa função, impedindo-a de afetar outras partes do código.
Variáveis com escopo local são úteis para evitar conflitos e poluição no escopo global. Elas são criadas quando a função é chamada e destruídas quando a função termina sua execução.

JavaScript usa __escopo estático__, também conhecido como escopo léxico ou escopo de compilação. Isso significa que o escopo das variáveis é determinado em tempo de compilação, com base na estrutura léxica (ordem física das palavras) do código fonte.

No __escopo estático__ em JavaScript, as variáveis são vinculadas aos blocos de código em que foram declaradas. Variáveis declaradas usando var são acessíveis apenas dentro da função em que foram declaradas ou no escopo global, se não estiverem dentro de uma função. Variáveis declaradas usando let ou const, em vez de var, têm escopo de bloco, o que significa que elas são acessíveis apenas dentro do bloco de código em que foram declaradas, incluindo blocos aninhados dentro desse bloco.

    function exemplo() {
    var x = 10; // Variável x está no escopo da função exemplo

    if (x > 5) {
        var y = 20; // Variável y está no escopo do bloco if
        console.log(x); // É possível acessar x aqui
        console.log(y); // É possível acessar y aqui
    }

    console.log(x); // É possível acessar x aqui
    // É possível acessar y aqui, pois var não tem escopo de bloco
    }

    exemplo();

    // console.log(x); // Isso causaria um erro, pois x não está disponível fora da função exemplo
    // console.log(y); // Isso também causaria um erro, pois y não está disponível fora do bloco if

Neste exemplo, a variável x está disponível dentro da função exemplo e dentro do bloco if, pois o bloco if está aninhado dentro da função. No entanto, a variável y só está disponível dentro do bloco if. Se tentarmos acessar x ou y fora de seus respectivos escopos, ocorrerá um erro.

O escopo estático em JavaScript é fundamental para entender como as variáveis são acessíveis em diferentes partes do código e garantir que elas sejam utilizadas corretamente. É recomendado utilizar let e const para declarar variáveis em blocos de código, pois eles oferecem um escopo mais previsível e seguro, evitando problemas de sobrescrita acidental e comportamentos inesperados.

### Endereço de memoria

Em JavaScript, não é possível acessar diretamente o endereço de memória de uma variável como é possível em algumas linguagens de programação de baixo nível. 
Não, JavaScript não possui ponteiros como em linguagens de programação de baixo nível, como C ou C++. Em JavaScript, a manipulação de memória é abstraída e gerenciada pelo próprio ambiente de execução (geralmente um navegador ou um ambiente de tempo de execução do JavaScript, como o Node.js).

Em vez de ponteiros, JavaScript usa referências a objetos e valores. Ao atribuir um valor a uma variável em JavaScript, essa variável contém uma referência ao valor, não o valor real. Isso torna o gerenciamento de memória mais seguro, pois não há acesso direto à memória bruta.

    let objeto1 = { nome: "João" }; // objeto1 contém uma referência a um objeto
    let objeto2 = objeto1; // objeto2 também contém uma referência ao mesmo objeto
    objeto1 = null; // objeto1 agora não aponta mais para o objeto
    console.log(objeto2.nome); // Ainda é possível acessar o objeto através de objeto2

### amarração 

Em JavaScript, a amarração de variáveis é dinâmica. Isso significa que o tipo de dado associado a uma variável pode mudar durante a execução do programa, conforme novos valores são atribuídos a ela.

Por ser uma linguagem de tipagem dinâmica, JavaScript permite que uma mesma variável assuma diferentes tipos de dados em momentos diferentes do programa. Isso é possível porque o tipo da variável é inferido a partir do valor que ela armazena em tempo de execução, e não é necessário declarar explicitamente o tipo de dado ao criar a variável.

Exemplo de tipagem dinâmica em JavaScript:

    let x = 10; // x é do tipo number
    console.log(typeof x); // Saída: "number"

    x = "Hello"; // Agora x é do tipo string
    console.log(typeof x); // Saída: "string"

    x = true; // Agora x é do tipo boolean
    console.log(typeof x); // Saída: "boolean"


### tempo de vida

 tempo de vida de uma variável em JavaScript refere-se ao período em que a variável existe na memória durante a execução do programa. Em outras palavras, é o intervalo de tempo entre a criação da variável e sua eventual remoção da memória (liberação de memória).

Em JavaScript, o tempo de vida de uma variável depende do escopo em que ela foi declarada e do tipo de declaração utilizada (var, let ou const).

Variáveis declaradas com var:
Têm escopo de função ou escopo global, caso sejam declaradas fora de uma função.
Existem durante toda a execução da função em que foram criadas ou durante toda a execução do programa, se declaradas fora de funções (escopo global).
São "hoisted" (içadas) para o topo do seu escopo de função ou global, o que significa que podem ser acessadas antes mesmo de serem declaradas, mas ainda não têm valor definido.
javascript
Copy code
    function exemplo() {
    if (true) {
        var x = 10; // x existe durante toda a execução da função exemplo
    }

    console.log(x); // Saída: 10 (x está disponível aqui, mesmo fora do bloco if)
    }

exemplo();

__Variáveis declaradas com let ou const:__
Têm escopo de bloco, ou seja, existem apenas dentro do bloco de código em que foram declaradas, incluindo blocos aninhados dentro desse bloco.
Existem apenas enquanto o bloco em que foram declaradas está ativo e são liberadas da memória quando o bloco é concluído.


    function exemplo() {
    if (true) {
        let y = 20; // y existe apenas dentro do bloco if
        const z = 30; // z também existe apenas dentro do bloco if
    }

    // console.log(y); // Isso causaria um erro, pois y não está disponível aqui
    // console.log(z); // Isso também causaria um erro, pois z não está disponível aqui
    }


Variáveis declaradas fora de funções têm escopo global e existem durante toda a execução do programa.

Variáveis globais têm um tempo de vida mais longo e são mantidas na memória até o final da execução do programa.


    let globalVar = "Sou global"; // Variável global, existe durante toda a execução do programa

    function exemplo() {
    console.log(globalVar); // Saída: "Sou global" (a variável globalVar pode ser acessada dentro da função)
    }

É importante lembrar que, após o tempo de vida de uma variável terminar (quando ela sai do escopo ou quando a execução do programa é concluída), a memória associada a essa variável é liberada automaticamente pelo garbage collector do JavaScript. Isso ajuda a evitar vazamento de memória e gerencia eficientemente os recursos do sistema.

### variavel estatica

Em JavaScript, não existe um conceito direto de "variável estática" como em algumas outras linguagens de programação. Nas linguagens que suportam variáveis estáticas, essas variáveis são geralmente associadas a uma classe ou escopo de função e mantêm seu valor entre chamadas subsequentes à função ou instâncias da classe, preservando seu estado ao longo do tempo.

Em JavaScript, a linguagem não oferece um mecanismo nativo para declarar variáveis estáticas. No entanto, é possível simular esse comportamento usando closures (funções internas) e escopo de função. Uma closure pode manter um valor que persiste entre chamadas da função externa, funcionando de forma semelhante a uma variável estática.

Exemplo de simulação de variável estática em JavaScript:

javascript
Copy code
    function contador() {
    let count = 0; // Variável local que funciona como "variável estática"

    function increment() {
        count++;
        console.log(count);
    }

    return increment;
    }

const contador1 = contador(); // Cria uma instância do contador
contador1(); // Saída: 1
contador1(); // Saída: 2
contador1(); // Saída: 3

const contador2 = contador(); // Cria outra instância do contador
contador2(); // Saída: 1 (inicia a contagem independente da outra instância)
contador2(); // Saída: 2
Neste exemplo, a função contador retorna uma closure, que é a função increment. A variável count dentro da função contador atua como uma "variável estática" porque mantém seu valor entre chamadas diferentes à função increment. Cada instância de contador criada por meio da função contador() tem seu próprio escopo e mantém uma cópia privada da variável count.

Lembrando que esse padrão é uma simulação de variável estática em JavaScript e pode não ser tão eficiente ou claro como em linguagens que suportam esse recurso diretamente. É importante entender como closures funcionam para evitar comportamentos inesperados ao criar variáveis com "persistência" em JavaScript.

### Variavel Pilha

Em JavaScript, as variáveis são alocadas de forma diferente em comparação com linguagens que têm uma área de memória dedicada para a pilha de execução, como C ou C++. Em JavaScript, a alocação de variáveis é feita no heap e não na pilha.

Quando você cria uma variável em JavaScript, ela é armazenada no heap e é acessível através de uma referência a essa variável. A referência é armazenada na pilha de execução, que rastreia o fluxo de execução do programa e controla o escopo das variáveis.

A pilha de execução em JavaScript é usada para armazenar informações sobre as chamadas de função e contextos de execução. Isso inclui os parâmetros das funções, variáveis locais e outros detalhes relacionados à execução do programa.

Vale ressaltar que os detalhes de alocação de memória em JavaScript são abstraídos e tratados pelo ambiente de tempo de execução (como navegadores ou o Node.js). Os desenvolvedores não precisam se preocupar diretamente com a alocação de memória ou a pilha de execução em JavaScript, pois a linguagem se encarrega desses detalhes de forma transparente.

Embora JavaScript não tenha uma pilha de execução explícita para alocar variáveis, você ainda precisa ter cuidado com o gerenciamento de memória e evitar vazamentos de memória ao criar objetos e referências. O mecanismo de coleta de lixo (garbage collector) do JavaScript é responsável por liberar a memória de objetos que não estão mais em uso, ajudando a evitar problemas de memória.


### Variável Explícita de Heap x Variável Implícita de Heap

Em JavaScript, não existem explicitamente "Variáveis Explícitas de Heap" ou "Variáveis Implícitas de Heap" como conceitos específicos da linguagem. A alocação e gerenciamento de memória em JavaScript são tratados automaticamente pelo ambiente de execução e pelo mecanismo de coleta de lixo (garbage collector).

Em vez disso, em JavaScript, todas as variáveis (sejam primitivas ou objetos) são armazenadas no heap e acessíveis por meio de referências. As variáveis primitivas (como números, strings, booleanos, null e undefined) são armazenadas diretamente na memória onde a variável é declarada. Por outro lado, as variáveis que armazenam objetos não contêm diretamente o objeto em si, mas sim uma referência (ou endereço de memória) ao objeto no heap.

Quando você cria um objeto em JavaScript, a alocação de memória para esse objeto ocorre no heap. Se você atribuir esse objeto a uma variável, a variável conterá uma referência a esse objeto no heap. Se você copiar ou atribuir essa variável a outra, apenas a referência será copiada, não o objeto em si. Isso é o que geralmente chamamos de "passagem por referência" em JavaScript.

Exemplo:


    let objeto1 = { nome: "João" }; // Cria um objeto no heap e armazena a referência em objeto1
    let objeto2 = objeto1; // objeto2 agora contém a mesma referência que objeto1

    objeto1.nome = "Maria"; // Altera o objeto1 (e também o objeto2, pois ambos apontam para o mesmo objeto)

    console.log(objeto2.nome); // Saída: "Maria", pois objeto2 é uma referência ao mesmo objeto que objeto1

Esse comportamento é diferente das variáveis primitivas, que armazenam diretamente o valor. Quando você copia ou atribui uma variável primitiva a outra, o valor é copiado, e as duas variáveis têm valores independentes.

  let a = 10;
  let b = a; // b recebe uma cópia do valor de a

  a = 20; // Altera o valor de a, mas não afeta b

console.log(b); // Saída: 10, pois b tem uma cópia do valor original de a
Portanto, em JavaScript, todas as variáveis, sejam primitivas ou objetos, são armazenadas no heap, mas o comportamento de cópia e atribuição difere entre os tipos de dados. O mecanismo de passagem por referência para objetos é importante para entender como as alterações em um objeto afetam outras variáveis que também fazem referência ao mesmo objeto.

### literal numérico

Quando um número aparece diretamente em um programa JavaScript, ele é chamado de literal numérico. JavaScript aceita literais numéricos em vários formatos, conforme descrito nas seções a seguir. Note que qualquer literal numérico pode ser precedido por um sinal de subtração (-) para tornar o número negativo. Tecnicamente, contudo, - é o operador de negação unário (consulte o Capítulo 4) e não faz parte da sintaxe de literal numérico.

1. literais inteiros

Em um programa JavaScript, um inteiro de base 10 é escrito como uma sequência de dígitos. Por exemplo:

    0 3 10000000 

Além dos literais inteiros de base 10, JavaScript reconhece valores hexadecimais (base 16). Um literal hexadecimal começa com “0x” ou “0X”, seguido por uma sequência de dígitos hexadecimais. Um dígito hexadecimal é um dos algarismos de 0 a 9 ou as letras a (ou A) até f (ou F), as quais representam valores de 10 a 15. Aqui estão exemplos de literais inteiros hexadecimais:

    0xff // 15*16 + 15 = 255 (base 10)

    0xCAFE911

Embora o padrão ECMAScript não ofereça suporte para isso, algumas implementações de JavaScript permitem especificar literais inteiros no formato octal (base 8). Um literal em octal começa com o dígito 0 e é seguido por uma sequência de dígitos, cada um entre 0 e 7. Por exemplo:

    0377 // 3*64 + 7*8 + 7 = 255 (base 10)

Como algumas implementações aceitam literais em octal e algumas não, você nunca deve escrever um literal inteiro com um zero à esquerda; nesse caso, não dá para saber se uma implementação vai interpretá-la como um valor octal ou decimal. No modo restrito de ECMAScript 5 (Seção 5.7.3), os literais em oc tal são proibidos explicitamente.

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

### Aritmética em JavaScript 

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

### tratamento de erro em java script

O tratamento de erros em JavaScript é uma prática importante para lidar com situações imprevistas que possam ocorrer durante a execução do código. Erros podem ser causados por erros de sintaxe, erros lógicos, exceções lançadas por funções ou problemas de rede, entre outros. Aqui estão algumas maneiras de lidar com erros em JavaScript:

__Bloco try...catch:__

O bloco try é usado para envolver o código que você acredita que pode gerar um erro. Se um erro ocorrer dentro do bloco try, ele é capturado pelo bloco catch, permitindo que você tome medidas para lidar com o erro.

      try {
        // Código que pode gerar um erro
      } catch (erro) {
        // Tratamento do erro
      }

__Lançamento de Exceções:__

Você pode usar a palavra-chave throw para lançar uma exceção em JavaScript. Isso permite que você crie e personalize seus próprios tipos de erros para situações específicas.

      function dividir(a, b) {
        if (b === 0) {
          throw new Error("Divisão por zero não é permitida.");
        }
        return a / b;
      }

__Bloco try...catch...finally:__

O bloco finally é opcional e é usado para conter código que será executado independentemente de ocorrer ou não um erro dentro do bloco try.

      try {
        // Código que pode gerar um erro
      } catch (erro) {
        // Tratamento do erro
      } finally {
        // Código executado sempre
      }

__Objeto Error:__

O JavaScript tem uma hierarquia de objetos de erro que podem ser usados para representar diferentes tipos de erros. Por exemplo, Error, SyntaxError, TypeError, entre outros.

      try {
        // Código que pode gerar um erro
      } catch (erro) {
        if (erro instanceof SyntaxError) {
          console.error("Erro de sintaxe:", erro.message);
        } else {
          console.error("Erro:", erro.message);
        }
      }

O tratamento de erros é crucial para tornar seus programas mais robustos e identificar problemas antes que eles causem impacto negativo no funcionamento do aplicativo. Certifique-se de identificar os pontos em seu código que podem gerar exceções e implementar tratamentos apropriados para lidar com elas.

# Expressões e operadores

Expressões em JavaScript são combinações de valores, variáveis e operadores que produzem um resultado. Elas podem ser tão simples quanto uma única variável ou tão complexas quanto uma fórmula matemática ou uma combinação de operações. As expressões são a base para a criação de lógica e cálculos em programas.

1. __Expressões Aritméticas:__ São expressões que envolvem operações matemáticas, como adição, subtração, multiplicação e divisão. Exemplos de expressões aritméticas:

        let soma = 5 + 3;       // Expressão de adição
        let multiplicacao = 4 * 6; // Expressão de multiplicação

2. __Expressões Relacionais:__ São expressões que comparam valores e retornam um valor booleano (true ou false). Elas são frequentemente usadas para avaliar condições. Exemplos de expressões relacionais:

        let maiorQue = 10 > 5;       // Expressão de comparação maior que
        let igualA = 7 === "7";       // Expressão de igualdade restrita

3. __Expressões Lógicas:__ São expressões que combinam valores booleanos usando operadores lógicos, como && (E) e || (OU). Elas são frequentemente usadas para criar condições complexas. Exemplos de expressões lógicas:

        let condicao = (idade >= 18) && (temCarteira == true); // Expressão lógica
4. __Expressões de Invocação (Chamadas de Funções):__ Também são consideradas expressões, pois representam a avaliação de uma função e podem retornar um valor.

        let resultado = calcularSoma(10, 20); // Expressão de chamada de função

5. __Expressões de Atribuição:__ São usadas para atribuir valores a variáveis.

        let x = 42; // Expressão de atribuição

6. __expressões de criação de objeto__ em JavaScript permitem que você crie novos objetos utilizando a sintaxe de chaves {}. Os objetos em JavaScript são coleções de propriedades, onde cada propriedade tem um nome (chave) e um valor associado. As expressões de criação de objeto permitem definir essas propriedades e seus valores iniciais.

        // Criando um objeto vazio
        let pessoa = {};

        // Definindo propriedades no objeto 'objeto.propriedade'
        pessoa.nome = "Alice";
        pessoa.idade = 30;
        pessoa.profissao = "Engenheira";

        console.log(pessoa); // Saída: { nome: 'Alice', idade: 30, profissao: 'Engenheira' }
        
7. __Expressões de Acesso à Propriedade:__  permitem que você obtenha o valor de uma propriedade de um objeto utilizando a notação de ponto (objeto.propriedade) ou a notação de colchetes (objeto['propriedade']). Aqui estão exemplos de ambas as notações:

        console.log(pessoa.nome); // Saída: "Alice"
        console.log(pessoa['idade']); // Saída: 30

8. __Inicializadores de Objeto e Array:__ são formas concisas de criar objetos e arrays com valores iniciais diretamente na sua declaração. Eles são definidos utilizando chaves {} para objetos e colchetes [] para arrays.

inicializador de objeto:

      let pessoa = {
        nome: "Alice",
        idade: 30
      };

inicializador de array:

      let numeros = [1, 2, 3, 4, 5];

### Operadores

1. __Operador in:__ O operador in é usado para verificar se uma propriedade existe em um objeto. Ele retorna true se a propriedade especificada estiver no objeto ou em sua cadeia de protótipos.

        let pessoa = { nome: "Alice", idade: 30 };
        console.log("nome" in pessoa); // Saída: true
        console.log("profissao" in pessoa); // Saída: false

2. __Operador instanceof:__ O operador instanceof é usado para verificar se um objeto é uma instância de uma determinada classe ou construtor.

        let objeto = new Date();
        console.log(objeto instanceof Date); // Saída: true
        console.log(objeto instanceof Array); // Saída: false

3. __eval():__ espera um único argumento. Se for passado qualquer valor que não seja uma string, ela simplesmente retorna esse valor. Se for passada uma string, ela tenta analisar a string como código JavaScript, lançando uma exceção SyntaxError em caso de falha. Se conseguir analisar a string, então ela avalia o código e retorna o valor da última expressão ou instrução da string ou undefined, caso a última expressão ou instrução não tenha valor algum. Se a string avaliada lança uma exceção, essaexceção é propagada a partir da chamada a eval().

        let codigo = "console.log('Olá, mundo!');";
        eval(codigo); // Saída: "Olá, mundo!"

4. __Operador typeof:__ O operador typeof é usado para verificar o tipo de um valor. Ele retorna uma string que indica o tipo do valor.

        console.log(typeof 42); // Saída: "number"
        console.log(typeof "Olá"); // Saída: "string"


5. __Operador delete:__ O operador delete é usado para remover uma propriedade de um objeto ou para remover um elemento de um array.

        let pessoa = { nome: "Alice", idade: 30 };
        delete pessoa.idade;
        console.log(pessoa); // Saída: { nome: "Alice" }

6. __Operador void:__ O operador void é usado para avaliar uma expressão sem retornar um valor definido. Ele é frequentemente usado para forçar a execução de um código sem retornar algo que possa ser atribuído a uma variável.

          let resultado = void console.log("Execução completa");
          // Saída: "Execução completa"
          console.log(resultado); // Saída: undefined

7. __Operador Vírgula ,:__ O operador de vírgula permite que você execute múltiplas expressões separadas por vírgulas, avaliando cada uma delas e retornando o valor da última expressão.

          let a = 1, b = 2, c = 3;
          console.log(a, b, c); // Saída: 1 2 3

As expressões relacionais e os operadores discutidos são partes importantes da linguagem JavaScript e são usados para realizar comparações, avaliar expressões e executar ações específicas em seu código.

# Subprogramas 

Subprogramas em JavaScript referem-se a blocos de código reutilizáveis que podem ser chamados várias vezes a partir de diferentes partes do programa. Eles também são conhecidos como funções. Subprogramas são uma maneira de modularizar o código, tornando-o mais organizado, reutilizável e mais fácil de entender. Em JavaScript, você pode definir subprogramas usando a palavra-chave function. Existem dois tipos principais de subprogramas em JavaScript:

1. __Funções:__ 

        function nomeDaFuncao(parametro1, parametro2) {
          // Código da função
          return resultado;
        }

        exemplo:

        function soma(a, b) {
          return a + b;
        }

        let resultado = soma(3, 5); // Chama a função

2. __Expressões de Funções Anônimas:__ Uma função anônima é definida como uma expressão e geralmente é atribuída a uma variável ou passada como argumento para outra função.

        function aplicarOperacao(array, operacao) {
        const resultado = [];
          for (const elemento of array) {
            resultado.push(operacao(elemento));
          }
          return resultado;
        }

        function dobrar(numero) {
          return numero * 2;
        }

        const numeros = [1, 2, 3];
        const dobrados = aplicarOperacao(numeros, dobrar);
        console.log(dobrados); // Saída: [2, 4, 6]


3. __Arrow Functions:__ As arrow functions são uma forma mais curta e concisa de escrever funções anônimas em JavaScript.

        const nomeDaFuncao = (parametro1, parametro2) => {
          // Código da função
          return resultado;
        };

        Exemplo:

        const potencia = (base, expoente) => base ** expoente;

        let resultado = potencia(2, 3); // Chama a função

### Passagem de Parâmetros:

A passagem de parâmetros envolve a transferência de valores de uma parte do programa para outra, geralmente entre funções. Em JavaScript, os parâmetros podem ser passados para funções quando elas são chamadas. Os valores passados podem ser usados dentro da função para realizar operações.

Tipos de Passagem de Parâmetros:

__Passagem por Valor:__ Nesse tipo, uma cópia do valor real do parâmetro é passada para a função. As alterações feitas nos parâmetros dentro da função não afetam os valores originais fora da função.

__Passagem por Referência:__ Aqui, um referência ao valor real (um endereço de memória) é passado para a função. Isso significa que as alterações feitas nos parâmetros dentro da função afetam os valores originais fora da função.

Implementação de Passagem de Parâmetro:

      // Passagem por valor (tipos primitivos)
      function incrementar(numero) {
        numero++;
      }

      let valor = 5;
      incrementar(valor); // O valor não é alterado fora da função
      console.log(valor); // Saída: 5

      // Passagem por referência (objetos e arrays)
      function modificarArray(arr) {
        arr.push(42);
      }

      let meuArray = [1, 2, 3];
      modificarArray(meuArray); // O array é alterado fora da função
      console.log(meuArray); // Saída: [1, 2, 3, 42]
