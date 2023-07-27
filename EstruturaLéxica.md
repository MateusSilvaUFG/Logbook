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

