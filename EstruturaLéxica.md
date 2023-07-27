## Estruruta léxica

A estrutura léxica de uma linguagem de programação é o conjunto de regras elementares que especificam o modo de escrever programas nessa linguagem. É a sintaxe de nível mais baixo de uma
linguagem; especifica detalhes de como são os nomes de variáveis, os caracteres delimitadores para
comentários e como uma instrução do programa é separada da seguinte.

### conjunto de caracteres

Os programas JavaScript são escritos com o conjunto de caracteres Unicode. Unicode é um superconjunto de ASCII e Latin-1 e suporta praticamente todos os idiomas escritos usados hoje no
planeta

### Diferenciação de maiúsculas e minúsculas

JavaScript é uma linguagem que diferencia letras maiúsculas de minúsculas. Isso significa que palavras-chave, variáveis, nomes de função e outros identificadores da linguagem sempre devem ser digitados com a composição compatível de letras. A palavra-chave while, por exemplo, deve ser digitada
como “while” e não como “While” ou “WHILE.” Da mesma forma, online, Online, OnLine e ONLINE
são quatro nomes de variável distintos.

### Sequências de escape Unicode
Alguns componentes de hardware e software de computador não conseguem exibir ou introduzir o
conjunto completo de caracteres Unicode. Para ajudar os programadores que utilizam essa tecnologia mais antiga, JavaScript define sequências especiais de seis caracteres ASCII para representar qualquer código Unicode de 16 bits. Esses escapes Unicode começam com os caracteres \u e são seguidos
por exatamente quatro dígitos hexadecimais (usando as letras A–F maiúsculas ou minúsculas). Os
escapes Unicode podem aparecer em strings literais, expressões regulares literais e em identificadores
JavaScript (mas não em palavras-chave da linguagem). O escape Unicode para o caractere “é”, por
exemplo, é \u00E9, e as duas strings JavaScript a seguir são idênticas:

      "café" === "caf\u00e9" // => true
  
Os escapes Unicode também podem aparecer em comentários, mas como os comentários são ignorados, eles são tratados como caracteres ASCII nesse contexto e não são interpretados como
Unicode.

### Normalização
O Unicode permite mais de uma maneira de codificar o mesmo caractere. A string “é”, por exemplo, pode ser codificada como o caractere Unicode \u00E9 ou como um caractere ASCII “e” normal, seguido da marca de combinação de acento agudo \u0301. Essas duas codificações podem parecer exatamente a mesma quando exibidas por um editor de textos, mas têm diferentes codificações binárias e são consideradas diferentes pelo computador. O padrão Unicode define a codificação preferida para todos os caracteres e especifica um procedimento de normalização para converter texto em uma forma canônica conveniente para comparações. JavaScript presume que o código-fonte que
está interpretando já foi normalizado e não tenta normalizar identificadores, strings nem expressões
regulare

### Comentários
JavaScript aceita dois estilos de comentários. Qualquer texto entre // e o final de uma linha é tratado
como comentário e é ignorado por JavaScript. Qualquer texto entre os caracteres /* e */ também é
tratado como comentário; esses comentários podem abranger várias linhas, mas não podem ser aninhados. As linhas de código a seguir são todas comentários JavaScript válidos:

            // Este é um comentário de uma linha.
            /* Este também é um comentário */ // e aqui está outro comentário.
            /*
            * Este é ainda outro comentário.
            * Ele tem várias linhas.
            */
### Literais
Um literal é um valor de dados que aparece diretamente em um programa. Os valores seguintes são

todos literais:

      12 // O número doze
      1.2 // O número um ponto dois
      "hello world" // Uma string de texto
      'Hi' // Outra string
      true // Um valor booleano
      false // O outro valor booleano
      /javascript/gi // Uma "expressão regular" literal (para comparação de padrões)
      null // Ausência de um objeto

### identificadores

Em JavaScript, um identificador é um nome utilizado para identificar variáveis, funções, classes ou qualquer outro elemento nomeado dentro do código. Em outras palavras, é um nome que você escolhe para dar a uma entidade (variável, função, objeto, etc.) para poder referenciá-la e utilizá-la em seu programa.

As regras para formar identificadores em JavaScript são as seguintes:

Um identificador pode conter letras (maiúsculas e minúsculas), dígitos (0-9) e os caracteres especiais _ (underscore) e $ (cifrão).
Um identificador deve começar com uma letra, _ ou $. Ele não pode começar com um dígito.
Não é permitido o uso de espaços em um identificador.
O identificador pode ser qualquer sequência de caracteres válidos que não seja uma palavra reservada (palavras que possuem significado específico na linguagem e não podem ser usadas como identificadores).
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
      
É importante escolher nomes significativos e descritivos para identificadores, para que o código seja mais legível e compreensível para outras pessoas que venham a ler o seu código.

### Palavras reservadas fazem parte desse capitulo

JavaScript predefine diversas variáveis e funções globais e você deve evitar o uso de seus nomes em suas próprias variáveis e funções:

      arguments encodeURI Infinity Number RegExp
      Array encodeURIComponent isFinite Object String
      Boolean Error isNaN parseFloat SyntaxError
      Date eval JSON parseInt TypeError
      decodeURI EvalError Math RangeError undefined
      decodeURIComponent Function NaN ReferenceError URIError

### Pontos e vírgulas opcionais

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
