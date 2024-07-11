# <span style="color: #ff6600; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);">Evolução de Aprendizagem com a Cubos</span>

## Conteúdos a serem trabalhados nesse módulo

### Conteúdos lógico

1. [Funções](#funções)
2. [Tipos de Dados II](#tiposDadosII)
3. [Tipos Utilitários](#tiposUtilitários)
4. [Métodos de Strings](#métodosStrings)
5. [Métodos de arrays](#métodosArrays)
6. [Métodos de arrays II](#métodosArraysII)
7. [Métodos de arrays III](#métodosArraysIII)

### Conteúdos de Carreira

1. [Gestão de Tempo](#gestãoTempo)
2. [Curriculo e Carta de Apresentação](#curCartApre)
3. [LinkedIn](#LinkedIn)

## Os meus conhecimentos sobre os assuntos a serem abordados nesse módulo

### Conteúdos Lógicos

 <div id="funções"></div>

- **Funções**
  - Meu conhecimento sobre **funções**, é bem básico, e todo ele da linguagem JavaScript.
    Eu sabia que **funções** em JavaScript são usadas para declarar uma instrução ou até mesmo um conjunto de instruções.
    A sua declaração é geralmente feita da seguinte forma.

    1. **Palavra de declaração** `function`, utilizada para definir uma função.

    2. _Nome da função_: geralmente utilizado em funções nomeadas, também pode ser opcional no caso das funções anônimas.

    3. Um ou mais **parâmetros** valores de entrada quando recebidos na função, definidos entre parênteses, e separados por vírgulas quando forem 2 ou mais parâmetros. Eu já vi que em alguns casos parâmetros podem ser opcionais, ainda não sei os reais motivos.

    4. **Conjunto de instruções** O código que utilizamos para ser executado quando a função for chamada é definido entre `{}` .

    5. A função em `JavaScript` retorna algo. O retorno é chamado pela palavra `return` , quando explicito; caso não seja explicito, a função retornará `undefined`, por padrão.

    ```js
    // Declaração de função nomeada.
    Exemplo: function pessoa(nome) {
      if (nome === "Mateus") {
        return "Acesso Permitido"; // Retorno explícito.
      } else {
        return "Acesso Negado"; // Retorno explícito.
      }
    }
    let resultado = pessoa("Mateus");
    console.log(resultado); // Acesso Permitido .

    // Declaração de uma função anônima atribuída a uma variável.
    const anonima = function (play1, play2) {
      //Conjunto de instruções.
      if (play1 === play2) {
        return "Empate";
      } else if (play1 > play2) {
        return "Play1 é o vencedor"; // Retorno explícito.
      } else return "Play2 é o vencedor"; // Retorno explícito.
    };

    let vencedor = anonima(3, 2);
    console.log(vencedor); // Play1 é o vencedor  .

    //Declaração de função nomeada.
    function pessoa(nome) {
      // Conjunto de instruções.
      if (nome != 1) {
        console.log(`Seja bem-vindo, ${nome}!`); // Mensagem no console.
      }
    }

    let resultado = pessoa("Mateus");
    console.log(resultado); // undefined, Não há nenhum valor retornado explicitamente pela função.
    ```

<div id="tiposDadosII"> </div> 

- **Tipos de Dados II**
  - Eu possuía um pouco de conhecimentos sobre alguns _tipos de dados II_, como o tipo number, string, boolean, any e void.  

    1. Tipo `NUMBER`, é um objeto que nos permite trabalhar com valores numéricos.
    2. Tipo `STRING`, é usado para podermos representar e guardar informações de texto.
    3. Tipo `BOOLEAN` é um tipo usado na programação como um tipo lógico composto por dois valores que podem ser representados de forma numérica, como 0 ou 1, e de forma de texto, falso ou verdadeiro.
    4. Tipo `ANY`, é um tipo flexível e permissivo, ele permite que escrevamos códigos em TypeScript mais próximos ao JavaScript, sem utilizar uma segurança de tipo.
    5. Tipo `VOID`, é um tipo mais útil para retorno de função que não retorna nenhum valor. Caso atribuído a uma variável, pode não ser muito útil ao código, logo que, se tiver uma variável do tipo void, a mesma só poderá ser atribuída com `undefined`.

<div id="tiposUtilitários"></div>  

- **Tipos Utilitários**

  - Eu não tinha conhecimentos sobre os _tipos utilizados_.

<div id="métodosStrings"></div>  

- **Métodos de Strings**
  - Eu conhecia um único **Método de Strings**, o método **includes**, ele pode ser usado para verificar se uma string possui um valor específico, e retorna true se conter o valor e false caso contrário.

    ```js
    Exemplo:
    // Variável nome, é uma String.
    const nome = " Mateus ";
    // Variável contemMa, que utiliza o métado includes para verificar se a variável nome contem "MA".
    const contemMa = nome.includes("Ma");
    // Mensagem no console
    console.log(contemMa); //resultado = true;
    ```

 <div id="métodosArrays"></div>  

- **Métodos de Arrays**  
  - Eu já tinha conhecimentos sobre alguns **Métodos Arrays**, conhecimentos da linguagem de programação JavaScript, como o método `push`, ele adiciona um ou mais elementos ao final do array retornando um novo array.

    ```js
    Exemplo:
    // Método push
    // Variavel frutas, é um array composto por 3 elementos.
    const frutas = ['Morango', 'Uva', 'Banana'];
    //Adciona o novo elemento, sempre após o ultimo elemento do array.
    frutas.push('Manga');
    console.log(frutas); // ['Morango', 'Uva', 'Banana', 'Manga'] Novo array com a fruta adicionada no final.
    ```

  - Eu conhecia o método `unshift`, um pouco de semelhança com o método `push`. Ele também adiciona um ou mais elementos dentro do array, mas ao contrário do `push`, ele sempre adiciona os elementos no início do array.

    ```js
    Exemplo:
    // Método unshift
    // Variavel frutas, é um array composto por 3 elementos.
    const frutas = ['Morango', 'Uva', 'Banana'];
    // Adiciona o novo elemento, sempre antés do primeiro elemento do array.
    frutas.unshift('Acerrola')
    console.log(frutas) // ['Acerrola', 'Morango', 'Uva', 'Banana'] Novo array com a fruta adicionada no inicio.
    ```

  - Eu conhecia o método `pop`, ele remove sempre o último elemento do array e retorna o mesmo e um novo array sem elemento removido.

    ```js
    //Método pop
    Exemplo:
    // Variavel Verduras, é um array composto por 3 elementos.
    const verduras = ['Couve', 'Taioba', 'Alface'];
    //Retirada do elemento, será sempre o ultimo elemento do array.
    const elementoRetirado = verduras.pop();
    console.log(elementoRetirado); // retorno do elemento retirado.
    console.log(verduras); // ['Couve', 'Taioba'] novo array com elemento retirado do final.
    ```

  - Eu conhecia o método `shift`, ele, assim como o método `pop`, remove um ou mais elementos de dentro do array, mas ao contrário do método `pop`, ele sempre removera os elementos no início do array.

    ```js
    //Método shift
    Exemplo:
    // Variavel Verduras, é um array composto por 3 elementos.
    const verduras = ['Couve', 'Taioba', 'Alface'];
    //Retirada do elemento, será sempre o primeiro elemento do array.
    const elementoRetirado = verduras.shift();
    console.log(elementoRetirado); // retorno do elemento retirado.
    console.log(verduras); // ['Taioba', 'Alface'] novo array com elemento retirado.
    ```

  - Eu conhecia o método `reverse`, ele retorna o aray inverso do que foi passado inicialmente.

    ```js
    Exemplo:
      // Método reverse
    // VAriavel numeros, é um array com três elementos.
    const numeros = [10, 25, 50];
    // Declaração do método reverse que retorna o array inverso do inicial.
    numeros.reverse();
    console.log(numeros); // [50, 25, 10] Array inverso.
    ```

  - Eu sabia que, assim como as `Strings`, também podemos usar o método `includes`, para manipular arrays e verificar se contêm o elemento desejável dentro do array, a resposta sempre será true, ou false.

    ```js
    Exemplo:
    // Método includes
    // Variavel alunos, é um array com três elementos.
    const alunos = ['Mateus', 'Caio', 'Leticia'];
    // verificar se elemento existe dentro do array.
    const temAluno = alunos.includes('Leticia');
    console.log(temAluno); // resultado = true.
    ```

<div id="métodosArraysII"></div>  

- **Méttodos de Arrays II**

  - Eu já conhecia um pouco o método `find` ele é utilizado para fazer busca em um array através de uma instrução passada, ele retornará o primeiro elemento compatível com a instrução fornecida caso seja encontrado no array. Caso o elemento buscado não seja encontrado, ele retornará `undefined`

    ```js
    Exemplo:
    // Declaração de um array de objetos com propriedade nome e idade.
    const clientes = [
      { nome: "Mateus", idade: 18 },
      { nome: "Mateus", idade: 28 },
      { nome: "Mateus", idade: 19 }
    ]

    // Declaração do método find com a variavel buscarCliente
    const buscarCliente = clientes.findIdex((cliente) => {
      // Declaração explicita do retorno com a instruções da busca com método find
      return cliente.nome === "Mateus" && cliente.idade === 28
    })

    console.log(buscarCliente) // { nome: 'Mateus', idade: 28 }
    ```

  - Eu conhecia também um pouco o método `findIndex` apesar de ter uma sintaxe de uso, a meu ver, idêntica ao `find`, ele tem uma utilidade diferente. O método retorna o índice do elemento caso existente no array, se não for encontrado, o retorno será de −1.

    ```js
    Exemplo:
    // Declaração de um array de objetos com propriedade nome e idade.
    const clientes = [
      { nome: "Mateus", idade: 18 },
      { nome: "Mateus", idade: 28 },
      { nome: "Mateus", idade: 19 }
    ]


      // Declaração do método findIndex com a variavel buscarIndice
      const buscarIndice = clientes.findIndex((cliente) => {
        // Declaração explicita do retorno com as instruções da busca com método findIndex
        return cliente.nome === "Mateus" && cliente.idade === 28

      })

    console.log(buscarIndice) // 1
    ```

  - Eu tinha um pouco de conhecimento sobre o método `filter`. Ele copia e retorna um novo array, criando uma cópia superficial do array original, com as instruções fornecidas para a implementação da lógica de busca do método `filter`.

    ```js
    // Declaração de um array de objetos com propriedade nome e divida.
    const clientes = [
      { nome: "Mateus", divida: 180 },
      { nome: "Mateus", divida: 280 },
      { nome: "Mateus", divida: 190 },
    ];

    // Declaração do método filter com a variavel dividaMenor200.
    const dividaMenor200 = clientes.filter((cliente) => {
      // Declaração explicita do retorno com as instruções da busca com método filter.
      return cliente.nome === "Mateus" && cliente.divida < 200;
    });

    console.log(dividaMenor200); // [ { nome: 'Mateus', divida: 180 }, { nome: 'Mateus', divida: 190 } ]
    ```

<div id="métodosArraysIII"></div>

- **Métodos de Arrays III**
  - Eu conhecia um pouco sobre o método `reduce`, ele aplica uma função de retorno de chamada **redutor** fornecida pelas instruções passando em cada elemento do array retornado um único valor, a primeira vez que o retorno do método é executado seu valor anterior não é existente, então o elemento de índice 0 do array será usado como valor inicial, e a interação será a partir do índice −1.  O valor inicial pode ser fornecido e usado como valor de retorno da primeira chamada do método.

    ```js
    Exemplo:
    // Declaração do array de objeto com as propriedades nome e divida.
    const clientes = [
      { nome: "Mateus", divida: 180 },
      { nome: "Mateus", divida: 280 },
      { nome: "Mateus", divida: 190 }
    ]

    // Declaração da função somarTotalDivida com parametro clientes.
    function somarTotalDivida(clientes) {
      // Declaração explicita do retorno da função com aplicação das instruções do método reduce para calcular total de  dividas.
      return clientes.reduce((acumulador, cliente) => acumulador + cliente.divida, 0)
    }
    // declaração da variavel totalDivida que armazena o resultado da função.
    const totalDivida = somarTotalDivida(clientes);
    console.log(totalDivida) // 650
    ```
  
### Conteúdos de carreira

 <div id="gestãoTempo"></div>

- **Gestão de Tempo**

  - Eu conhecia pouco sobre gestão de tempo, sabia que é um processo de planejamento e de controle sobre o tempo que temos e como iremos dividir para uma melhor produtividade do nosso dia.

<div id="curCartApre"></div>  

- **Currículo e Carta de Apresentação**

  - Eu não conhecia boas práticas de currículo e carta de apresentação.

<div id="LinkedIn"></div>  

- **LinkedIn**

  - Eu não conhecia muito sobre o bom uso do LinkedIn.

## Conteúdos que eu gostraria de aprender sobre os assuntos desse módulo

### Conteúdos de logíca

- `Funções`

  1. Gostaria de aprender quais são as melhores formas de declarar _funções_.
  2. Quais tipos de _funções_ existem? Elas podem ser aplicadas para melhorar meus códigos e projetos.

- `Tipos de Dados`

  1. O que são os _tipos de dados_ e quais são os benefícios do uso deles no meu código e projetos?
  2. Devo aprender e dar muita importância para o uso de _tipos de dados_ em meus códigos e projetos.

- `Tipos Utilitarios`

  1. O que são os _tipos úteis_, devo utilizar eles sempre em meus códigos e projetos?

- `Métodos de Strings`

  1. Quais são os _métodos de strings_ existentes que devo saber para melhorar meus códigos e projetos?
  2. Quando devo optar pelo uso dos _métodos de strings_ em meus códigos?
  3. Existem algumas ocasiões em que não devo fazer uso de _métodos de strings_?

- `Métodos de Arrays`

  1. Em quais tipos de projetos reais é utilizado o uso de _métodos de array_?
  2. Posso fazer uso sempre dos _métodos de array_ em meus códigos e projetos?
  3. Quais os ganhos do uso de _métodos de array_ em questões de qualidade de código?

- `Métodos de Arrays II`
  1. Além da facilidade de uso de alguns dos _métodos de array II_ em alguns códigos, eles trazem mais vantagens para os códigos?
  2. _Métodos de array II_ são utilizados por muitas linguagens de programação?
- `Métodos de Arrays III`
  1. Quais são as consequências do uso exagerado de _métodos de arrays III_ em códigos e projetos reais?
  2. Tenho que saber sobre todos os _métodos de arrys III_ ?

### Conteúdos de carreira

- **Gestão de Tempo**

  1. Quais os sinais de que a minha gestão de tempo pode estar sendo mal realizada?
  2. Quais os métodos considerados eficazes para garantir uma melhor gestão de tempo?
  3. Como fazer uma boa gestão de tempo para garantir qualidade no meu trabalho e vida pessoal?

- **Curricúlo e Carta de Aprensentação**
  1. Como devo fazer meus currículos e carta de apresentação?
  2. Existem boas práticas e métodos para deixar meus currículos e carta de apresentação melhor apresentados?
  3. O que nunca fazer em meus currículos e carta de apresentação?
- **LinkedIn**
  1. Como ter um LinkedIn profissional e de boa qualidade?
  2. Como devo me apresentar no LinkedIn para conseguir destaque?
  3. Existem métodos para ter um LinkedIn com mais visibilidade pelas redes?

## Coteúdos que eu aprendi nesse módulo

### Conteúdos lógicos

- **Funções**

  1. Aprendi um pouco mais sobre o conceito de _funções_, que _funções_ podem ser criadas para facilitar a repetição de tarefas, agindo como um subprograma dentro de nossos programas, podendo ser reutilizadas sob demanda se necessário.

  2. Aprendi que a área onde é posto nosso processo de instrução através das _funções_ é chamada de escopo.

  3. Aprendi que parâmetros de uma função só podem ser chamados dentro do escopo da função, e que também podemos criar uma função com parâmetro que recebe informações de um objeto.

  ```js
  Exemplo:
  // Obejeto recebido pelo parametro
  const pessoa = {
  nome: "Mateus Baia",
  idade: 28,
  altura: 168,
  };

  // Função para o cadastro do usuário
  function cadastraUsuario(usuario) {
    // Retono explicito com os dados do usuario cadastrado
    return `Usuario cadastrado: Nome ${usuario.nome}, Idade ${usuario.idade} anos, Altura ${usuario.altura}m`
  }

  // chamar a função para o cadastramento do usuario
  console.log(cadastraUsuario(pessoa)); // Usuario cadastrado: Nome Mateus Baia, Idade 28 anos, Altura 168m
  ```

  4. Aprendi que exite outra forma de declara uma função chamada `arrow function`, que basicamente é atribuir uma função a uma variavel, e essa variavel a receber uma função se torna um `function` sua maior diferença entre a declaração de função con a palavra reservada `function` é a sintáxia.

    ```js
     Exemplo:
    // Obejeto recebido pelo parametro
    const pessoa = {
    nome: "Mateus Baia",
    idade: 28,
    altura: 168,
    };

    // arrow function declarada com a variavel verificaNome.
    const verificaNome = (usuario) => {
    // conjuto de intruções
    if(usuario.nome != "Mateus Baia"){
      return 'ACESSO NEGADO'  // retorno explicito
    }else {
      return 'ACESSO PERMITIDO' // retorno explicito
    }
  }
  // chamar função pra verificação de nome.
  console.log(verificaNome(pessoa)) // ACESSO PERMITIDO
  ```

  5. Eu aprendi como faço a tipagem de função em `TypeScript`.

  ```ts
  // arrow function declarada com a variavel multiplicar, com dois parametros do tipo number e retorno também do tipo number.
  Exemplo: const multiplicar = (valor1: number, valor2: number): number => {
    return valor1 * valor2; //retorno  explicito
  };
  // chamar função com valor1 e valor1
  console.log(multiplicar(25, 35)); // 875
  ```

  6. Eu aprendi como faço tipagem de funções com objeto em `TypeScript`.

  ```ts
  // Declaração dos tipos das propriedades do obejeto.
  Exemplo: type TUsuario = {
    nome: string;
    idade: number;
    altura: number;
  };
  // Declaração da função cadastrarUsuario com parametro usuario que tem o tipo TUsuario,
  function cadastrarUsuario(usuario: TUsuario) {
    // Retorno explicido
    return ` Usuario Cadastrado: Nome ${usuario.nome}, Idade ${usuario.idade} anos, Altura ${usuario.altura}m `;
  }
  // Declaração da variavel novoUsuario que armazena os dados do usuario cadastrado
  const novoUsuario = cadastrarUsuario({
    nome: "Mateus Baia",
    idade: 28,
    altura: 168,
  });

  console.log(novoUsuario); // Usuario Cadstrado: Nome Mateus Baia, Idade 28 anos, Altura 168m
  ```

- **Tipos de dados II**

  1. Aprendi que em `TypeScript` temos uma palavra reservada, chamada `Type`, que utilizamos para criar tipos customizados, explicitamente, variáveis, objetos e funções.
  E que posso ter um tipo único, um tipo com objetos, e um array de tipos.

  2. Aprendi que podemos criar os tipos literais, os tipos literais em TypeScript, eles representam tipos que recebem um valor específico e não mais o valor do tipo que foi definido.

  ```ts
  //Declaração do tipo personalizado do objeto utilizando tipo literal para as propriedades modelo e marca.
  Exemplo: type TBolaNike = {
    modelo: "Futebol";
    marca: "Nike";
  };

  // Array de bolas que recebe o tipo TBolaNike que recebe um array inicialmente vazio.
  const bolas: TBolaNike[] = [];

  // Declaração da variável bolas.length para acessar o tamanho do array para ser atribuído um novo objeto.
  bolas[bolas.length] = {
    // Se tentarmos definir outro tipo para as propriedades modelo e marca, veremos um erro, pois as mesmas só podem ser do tipo futebol e Nike.
    modelo: "Futebol",
    marca: "Nike",
  };
  ```

  3. Aprendi que podemos customizar tipos com a união de tipos.

  ```ts
  // Declaração da variável propriedade com a união de tipos, nesse exemplo conseguimos ver que a variável propriedade poderá ser um NUMBER, ou uma STRING, ou um boolean
  Exemplo: const propriedade: number | string | boolean = "Mateus";

  // tambem pode ser feita em um objeto

  //declaração do tipo do objeto, com união de tipos.
  type TCarro = {
    modelo?: string;
    marca?: string;
    ano?: string | number;
  };

  //Declaração da variavel carros que recebe o tipo Tcarro que é um array
  const carros: TCarro[] = [];

  carros[carros.length] = {
    modelo: "gol", // poderá ser uma string ou undefined.
    ano: 2020, // poderá ser uma string number ou undefined.
    // Não foi declarada a propriedade marca, já que todos são opcionais, não é necessária a declaração.
    // Isso acontece porque o próprio TypeScript já usa a união de tipos quando colocamos uma propriedade como opcional.
  };
  ```

  4. Aprendi sobre os tipos tuplas, ela dá a permissão de que utilizamos tipos diferentes em um array desde que pré-declarado antes. O tipo tuplas possui um tamanho padrão pré-definido, sendo assim um array do tipo tupla só poderá receber propriedades do tamanho e do tipo pré-declarados.

  ```ts
  Exemplo: const iformacaoDiversas = [number, string, boolean];

  informacaoDiversas = [28, "Mateus", false];
  ```

  5. Aprendi sobre o tipo de união de tipos, permitido pelo uso do `&`, permiti que façamos a união de elementos de tipos diferentes. Em alguns casos, ele pode não ser adequado, pois pode trazer erros, pelo fato da união de dois tipos em uma variável pode retornar um never.

  ```ts
  // Quando não faz sentido o uso:
  Exemplo: type let: string & number; // ele retorna um tipo never então não pode ser usado.

  // Quando podemos utilizar?
  type TPessoa1 = {
  nome: string;
  idade: number;
  };

  type TPessoa2 = {
  sobrenome: string;
  telefone: number;
  };

  // Aqui atribuirmos a união dos dois tipos pessoas, tornando o tipo TPessoas um array de tipo com os dois tipos pessoas.
  type TPessoas = TPessoa1 & TPessoa2;

  //Tipo TPessoas com a união dos dois tipos.
  const pessoas: TPessoas[] = [
  {
  nome: "mateus",
  idade: 28,
  sobrenome: "Baia",
  telefone: 9995448354,
  },
  ];
  ```

  6. Aprendi sobre o tipo type Narrowing. Ele permitiu que manipulemos variáveis de tipos diferentes, criando condições específicas para poder somar ou uni-las conforme o seu tipo, mesmo tendo tipos diferentes.

  ```ts
  // Mesmo possuindo tipos diferentes, com o uso da técnica de type Narrowing podemos atribuir condições semelhantes para elementos de tipos diferentes.
  Exemplo: function typeNarrowing(
    numero1: number | string,
    numero2: number | string
  ) {
    if (typeof numero1 === "number" && typeof numero2 === "number") {
      return numero1 + numero2;
    } else if (typeof numero1 === "number" && typeof numero2 === "string") {
      return `${numero1} ${numero2}`;
    } else if (typeof numero1 === "string" && typeof numero2 === "number") {
      return Number(numero1) + numero2;
    } else {
      return `${numero1} ${numero2}`;
    }
  }
  // console.log(typeNarrowing(196, "321")); // Retornará a string, pois ele cairá na segunda condição.
  // console.log(typeNarrowing(196, 321));// Retornará o valor da soma, pois cairá na primeira condição.
  //console.log(typeNarrowing("196", 321)); // Retomará o valor da soma, pois cairá na terceira condição.
  console.log(typeNarrowing("196", "321")); // Retornará uma string, pois cairá na última condição.
  ```

  7. Aprendi um pouco sobre o tipo `Assertion`. Ele dá permissão para informarmos para o `typeScript` que ele possui um tipo específico. Não é considerável utilizar o type Assertion em qualquer situação, pois se o elemento esperado não existir, ele retornará undefined, então o ideal é utilizar quando lidarmos com códigos que tenhamos certeza de que ele enviará o tipo esperado mesmo não existindo.

- **Tipos Utilitarios**

  1. Aprendi que os tipos utilitarios em `TypeScript`são funções de tipos predefinidos usadas para criar operações e transformações em outro tipo existente. Seu uso é implementado pelo nome do tipo e o elemento de tipo existente.

  2. Aprendi que tipo utilitario `Partial` permiti alterar um tipo deixando suas propriedades opcionais mesmo quando o tipo foi previamente declarado com um tipo existente.

  ```ts
  Exemplo: type TPessoa = {
    nome: string;
    idade: number;
  };

  const pessoa: Pessoa = {
    nome: "João",
    idade: 30,
  };

  // Usando os tipos utilitários:
  type PessoaParcial = Partial<Pessoa>; // Todas as propriedades são opcionais.

  const pessoaParcial: PessoaParcial = { nome: "Maria" }; // Apenas a propriedade 'nome' é definida.
  ```

  3. Aprendi que o tipo utilitario `Required`é utilizado para deixar um tipo pré-definido como opcional obrigatório, agindo contrário do tipo `Partial`.

  ```ts
  Exemplo: type Pessoa = {
    nome?: string;
    idade?: number;
  };
  const pessoa: Pessoa = {
    nome: "João",
    idade: 30,
  };

  type PessoaObrigatorio = Required<Pessoa>; // Todas as propriedades são obrigatórias.

  const pessoaObrigatorio: PessoaObrigatorio = { nome: "Maria", idade: 15 }; // Apenas a propriedade 'nome' é definida, isso não seria permitido, pois todas as propriedades são obrigatórias.
  ```

  4. Aprendi que o tipo utilitario `Readonly` permite que deixemos um tipo com proibição de alteração, sendo permitido apenas a leitura do tipo.

  ```ts
  Exemplo: type Pessoa = {
    nome: string;
    idade: number;
  };

  const pessoa: Pessoa = {
    nome: "João",
    idade: 30,
  };

  type PessoaSomenteLeitura = Readonly<Pessoa>; // Todas as propriedades são somente leituras.

  pessoaParcial.idade = 25; // Isso não é permitido, pois 'idade' é somente leitura.
  ```

  5. Aprendi que o tipo utilitario `pick`é usado para criar alteração em um tipo e suas propriedades, com isso ele retorna um novo tipo apenas com as propriedades adicionadas.

  ```ts
    exemplo: type TPessoa = {
      nome: string;
      sobrenome: string;
      mae: string;
      pai: string;
      filho: string;
      endereco: string;
      email: string;
      senha: string
    }
    type novopersonagem Pick<TPessoa, 'nome' | 'sobrenome' | 'filho' | 'endereco' > // Novo tipo de Pessoa terar todas as propriedades passadas.
  ```

  6. Aprendi que o tipo utilitario `Omit` é aplicado em tipo objeto, e permiti que fassamos o contrario do _PICK_ com um tipo existente ele cria um novo tipo e remove as propriedades passadas, sendo assim ele retorna apenas um novo tipo sem as propriedades citadas.

  ```ts
  Exempo: type Pessoa = {
    nome: string;
    sobrenome: string;
    mae: string;
    pai: string;
    filho: string;
    endereco: string;
    email: string;
    senha: string

  };

  type novoTipo = Omit<Pessoa: 'nome' | 'email'>// Novo tipo, pessoa não terá as propriedades passadas.

  //DE MODO GERAL, ELES CRIAM A MESMA LÓGICA, A MAIOR MUDANÇA ESTÁ NO CENÁRIO ONDE SERÁ UTILIZADO COMO PODEMOS VER. Com O PICK IREMOS UTILIZAR MAIS PROPRIEDADES DO TIPO, POR ISSO ELE É UTILIZADO.
  ```

  8. Aprendi que o tipo utilitario `Exclude` é utilizado para excluir itens de uma união de tipos. Apesar da semelhança com o Omit, ele é utilizável em união de tipos e Omit em objetos.

  ```ts
  Exemplo: type Pagamentos = "Credito" | "Debito" | "Boleto" | "Pix";

  type Produto1 = Execlude<Pagamento, "Pix">;

  type Produto1 = Execlude<Pagamento, "Debito">;

  // Podemos ver que ele exclui formas de pagamento de cada produto, apesar da semelhança com o tipo Omit. Ele pode ser atribuído a um tipo literal de União de Tipos, e o tipo Omit em objetos.
  ```

   9. Aprendi que o tipo utilitario `Èxtract` é utilizado para incluir itens de união de tipos. Apesar da semelhança com o Pick ele é utilizável em união de tipos e Pick em objetos.  

  ```ts
  Exemplo: type Pagamentos = "Credito" | "Debito" | "Boleto" | "Pix" | "Dinheiro";

  type Produto1 = Execlude<Pagamento, "Debito" | "Credito">;

  type Produto2 = Execlude<Pagamento, "Dinheiro" | "Pix">;

  // Podemos ver que ele inclui algumas formas de pagamentos de cada produto, apesar da semelhança com o tipo Pick. Ele pode ser atribuído a um tipo literal de União de Tipos, e o Pick a um tipo objeto.

  // QUAL UTILIZAR ENTRA NA MESMA LÓGICA, DO PICK E OMIT QUAL FOR A MELHOR UTILIZAÇÃO DE ACORDO COM SEU CENÁRIO.
  ```

- **Métodos Strings**

  1. Eu aprendi que os métodos de strings permitem criarmos manipulações com strings por meio de métodos embutidos, como alterá-las, transformá-las, conferir tamanho, invertê-las e algumas outras manipulações.

  2. Eu aprendi que podemos utilizar o método `Trim` Para remover todos os espaços do início e do fim de uma string.

  ```ts
  Exemplo: const mensagem: string = "   Ei onde está você    ";

  console.log(mensagem.length); // rResultado: É um valor de 24, pois a string, contem espaços na frente e atrás.

  const mensagemReduzida = mensagem.trim();

  console.log(mensagemReduzida.length); // Podemos notar que ele retornará o valor 17, pois irá conter apenas a string e os espaços do meio, pois o método remove os espaços iniciais e finais.
  mensagem.trim();

  console.log(mensagem.length); // Resultado seria o mesmo valor 24, pois o método não altera diretamente uma string já armazenada.
  //O método não pode ser aplicado diretamente na string, pois ele não muda a string, pois ela não pode ser alterada, o que ele faz é criar uma nova string sem os espaços iniciais e finais.
  ```

  3. Aprendi que existem duas variações dentro do método Trim. Que são as `TrimStart` e `TrimEnd`, elas servem para quando queremos remover espaços específicos entre o início e o fim de uma string sendo o TrimStart para o início, e o TrimEnd para o final.

  4. Aprendi que os métodos `ToUpperCase` e `ToLowerCase`, o método ToUpperCase, para converter uma string toda para maiúsculas, e ToLowerCase, para convertê-la toda para minuscula.

  ```ts
  Exemplo: const texto: string = "olá, mundo!";
  console.log(texto.toUpperCase()); // Resultado: OLÁ, MUNDO!

  const texto: string = "OLÁ, MUNDO!";
  console.log(texto.toLowerCase()); // Resultado: olá, mundo!
  ```

  5. Aprendi que podemos utilizar os métodos `Substring` e o método `Slice`, eles permitem extrair sub cadeias de uma string especificando o índice, sendo o Substring do índice inicial e opcionalmente o final e o Slice, permiti extrair com índices negativos e pegar do final da string.

  ```ts
  Exemplo: `Substring`;
  const frase: string = "Kamehameha";

  console.log(frase.substring(3, 9)); // Resultado: extraindo (do indice 3 até o 9)RES: ehameh

  console.log(frase.substring(2)); // Resultado: extraindo (do índice 2 até o final) RES: mehameha

  `Slice`;
  const texto: string = "Kamehameha";

  console.log(texto.slice(1, 8)); // Resultado: extraindo (do indice 1 a 8 ) RES:  amehame

  console.log(texto.slice(-5)); // Resultado: extraindo (os últimos 5 caracteres) RES: ameha

  console.log(texto.slice(-5, 1)); // O indice de inicio é maior que indice final então retorna uma string vazia.
  ```

  6. Aprendi que posso utilizar o método de strings `Split` para dividir uma string em um array de strings com base em separador especificado.

  ```ts
  Exemplo: const texto: string = "'Kame','hame','ha','ha','ha','ha'";

  const palavras = texto.split(" ");

  console.log(palavras); // Resultado: [ "'Kame','hame','ha','ha','ha','ha'" ]
  ```

  7. Aprendi que posso utilizar o métodos de strings `Replace` e `ReplaceAll`, eles permitem subistituir as ocorrências de uma string por otro, similar uma a outra suas diferença está no fato de Replace, ele não considera expressões regulares, apenas strings literais. já o ReplaceAll Ele aceita expressões regulares como argumento.

  ```ts
  Exemplo: `Replace`;
  const frase: string = "O Goku é o mais fraco, e o Goku é o mais forte";

  const novaFrase = frase.replace("Goku", "Vegeta");

  console.log(novaFrase); // O Vegeta é o mais fraco, e o Goku é o mais forte

  `ReplaceAll`;
  const frase: string = "O Vegeta é o mais forte, e o Vegeta é o mais fraco.";
  const novaFrase = frase.replaceAll("Vegeta", "Goku");
  console.log(novaFrase); // Resultado:O Goku é o mais forte, e o Goku é o mais fraco.
  ```

  8. Aprendi que podemos utilizar os métodos `PadStart` e `PadEnd` para preencher uma string com um determinado caractere até atingir um tamanho mínimo determinado, sendo o PadStart preenchido para esquerda em sentido ao início e o PadEnd preenchido para o direito em sentido ao final.

  ```ts
  Exemplos:  `PadStart`
  const num1: string = "123";

  const num1Preenchido = num1.padStart(10, "0");

  console.log(num1Preenchido); // Resultado: 0000000123

  `PadEnd`
  const num2: string = "123";

  const num2Preenchido = num2.padEnd(10, "4");

  console.log(num2Preenchido); // Resultado: 1234444444
  ```

  9. Aprendi que também podemos utilizar o método de strings  `indexOf`. Ele dá a possibilidade de que encontramos a ocorrência de uma substring dentro da string, retornando o índice da primeira ocorrência, caso não encontre, ele retorna −1.

  ```ts
  Exemplos:
  const texto: string = "Onde está você Goku a terra precisa de você";

  console.log(texto.length) // Resultado: 43

  console.log(texto.indexOf("Goku")); // Resultado: 15

  console.log(texto.indexOf("vegeta")); // Resultado: -1
  ```

- **Método de array**
  1. Eu aprendi alguns métodos de array e aprimorei como posso fazer o uso de uma melhor fórmula dos métodos que eu já havia tido um pré-contado.

  2. Aprendi que, assim como no método de strings em métodos de array também podemos reutilizar alguns métodos, um deles é o `indexOf` ele permite percorrer um array e retorna o índice da primeira ocorrência de um elemento em um array. Caso o elemento não seja encontrado, o método retorna −1.

  ```ts
  Exempo: 
  const personagens: string[] = ['Goten', 'Gohan', 'Trunks', 'Pan', 'Goku'];

  const indiceGohan = personagens.indexOf('Gohan');
  console.log(indiceGohan); // Resultado: 1

  const indiceVegeta = personagens.indexOf('Vegeta');
  console.log(indiceVegeta); // Resultado: -1
  ```

  3. Aprendi que podemos utilizar o método `join` ele age juntando os elementos em um array em uma string, fazendo uso de um separador especificado. Caso nenhum separador for especificado, o método usará vírgula(',') como separador padrão.

  ```ts
  Exemplo:
  const personagens: string[] = ['Goten', 'Gohan', 'Trunks', 'Pan', 'Goku'];

  const stringPersonagem = personagens.join();

  console.log(stringPersonagem); // Resultado: Goten,Gohan,Trunks,Pan,Goku

  const stringPersonagem = personagens.join(" e ");

  console.log(stringPersonagem); // Resultado: Goten e Gohan e Trunks e Pan e Goku
  ```


  4. Aprendi que podemos utilizar o método `slice` para extrair uma cópia a partir de um subarray criado entre os índices início e fim de um array original, o array original não é modificado.
  
  ```ts
  Exemplo:
  const personagens: string[] = ['Goten', 'Gohan', 'Trunks', 'Pan', 'Goku'];

  const primeiroPersonagens = personagens.slice(0, 2);

  console.log(primeiroPersonagens); // Resultado: [ 'Goten', 'Gohan' ]

  const ultimosPersonagens = personagens.slice( -2);

  console.log(ultimosPersonagens); // Resultado: [ 'Pan', 'Goku' ]
  ```

- **Métodos de arrays II**

  1. Aprimorei alguns conhecimentos de métodos de array II, que eu já possuía conhecimentos prévios e conceitos de aplicação em TypeScript.

  2. Aprendi conceitos de callbacks com `setTimeuout` e com  `setInterval`como posso estar utilizando em minhas funções.

  3. Aprendi como posso estar utilizando o método de array `Every`, ele permite verificar se todos os elementos de um array passam em um determinado teste específico por uma função. Ele retorna true caso todos sejam aprovados e false caso contrário.

  ```ts
  Exemplo:
  const personagens: string[] = ['Goten', 'Goten', 'Goten', 'Goten'];

  const todosGoten = personagens.every(personagen => personagen === 'Goten');

  console.log(todosGoten); // Resultado: true

  const todosGonha = personagens.every(personagen => personagen === 'Gohan');

  console.log(todosGonha); // Resultado: false
  ```

  5. Aprendi como utilizar o método `some` ele permite verificar se ao menos um elemento dentro do array passa em um teste especificado por uma função. Em caso de sucesso, ele retorna true e, caso ao contrário, ele retorna false.

  ```ts
  Exemplo:
  const personagens: string[] = ['Goten', 'Gohan', 'Trunks', 'Pan', 'Goku'];

  const algumSemN = personagens.some(personagen => !personagen.includes ('n'));

  console.log(algumSemN); // Resultado: true

  const algumTemSeteLetras = personagens.some(personagen => personagen.length === 7);

  console.log(algumTemSeteLetras); // Resultado: false
  ```

  6. Aprendi como posso estar utilizando o método `map`ele permite que uma função, possa transformar cada elemento de um array em um novo valor, utilizando uma transformação uma vez por cada elemento existente no array. E retorna um novo array com os elementos modificados conforme foi passado na função.

  ```ts
  Exemplo:
  const personagens: string[] = ['Goten', 'Gohan', 'Trunks', 'Pan', 'Goku'];

  const nomesMinusculo = personagens.map(personagen => personagen.toLocaleLowerCase());

  console.log(nomesMinusculo); // Resultado: [ 'goten', 'gohan', 'trunks', 'pan', 'goku' ]


  const nomesMaiusculos = personagens.map(personagen => personagen.toLocaleUpperCase());

  console.log(nomesMaiusculos); // Resultado: [ 'GOTEN', 'GOHAN', 'TRUNKS', 'PAN', 'GOKU' ]
  ```

- **Métodos de Arrays III**

  1. Aprimorei conhecimento sobre o método de array `reduce` conceitos de aplicações do método em TypeScript, também aprendi como posso estar utilizando alguns outros métodos.

  2. Aprendi como posso está utilizando o método `sort`ele permitiu criar ordenação de elementos em um array conforme a tabela Unicode, Sendo assim ele não é utilizado por padrão quando buscamos uma ordenação crescente, pois como ele ordena conforme a tabela Unicode, o resultado crescente pode não ser o esperado, pois a tabela Unicode tem um formato padrão diferente. Caso queria uma ordenação crescente ou decrescente em ordem, é necessária a utilização de uma função dentro do método `sort` para especificar as condições de retorno desejadas.

  ```ts
  Exemplo: 
  //Padrão
  const numeros1: number[] = [1, 2, 3, 22, 22, 17, 350, 189];
  numeros1.sort()

  //Crescente
  const numeros2: number[] = [1, 2, 3, 22, 22, 17, 350, 189];
  // Função recebe dois parâmetros, pois ela irá comparar o primeiro índice com o próximo índice.
  numeros2.sort((numero1: number, numero2: number): number => {
      return numero1 - numero2
      
  })

  //Decrescente
  const numeros3: number[] = [1, 2, 3, 22, 22, 17, 350, 189];
  // Função recebe dois parâmetros, pois ela irá comparar o primeiro índice com o próximo índice.
  numeros3.sort((numero1: number, numero2: number): number => {
      return numero2 - numero1
  })
      
  console.log(numeros1); // Resultado padrão: 1, 17, 189, 2, 22, 22,   3, 350
  console.log(numeros2); // Resultado com crescente: [   1, 2,   3, 17, 22, 189, 350 ]
  console.log(numeros3);// resultado decrescente: [350, 189, 22, 22, 17, 3,  2,  1]
  ```

### Contúdos carreira

- **Gestão de tempo**

  1. Eu aprendi que ter uma boa gestão de tempo devemos nos organizar de forma mais produtiva, priorizando as tarefas importantes do nosso dia a dia sem negociação com a procrastinação.
  2. Aprendi que hoje já existem muitas ferramentas que podem nos auxiliar a gerir melhor nosso tempo para conseguirmos ter um controle maior das tarefas consideradas obrigatórias no nosso dia.
  Com isso, conseguimos ser mais produtivos e eficientes, utilizando melhor o nosso tempo de trabalho e a vida pessoal.

- **Currículo e Carta de Aprensentação**

    1. Aprendi como devo montar um currículo profissional para ter uma boa apresentação, a importância de um currículo bem feito, informações que não devo pôr em meu currículo, e as que são essenciais. 

    1. Aprendi o que é uma cover letter e a sua importância para uma busca por vaga de emprego.
    E aprendi como faço para criar uma cover letter, ou carta de apresentação, de qualidade.

- **LinkedIn**
    1. Aprendi que o LinkedIn é uma rede social com foco profissional que devemos utilizar para mostrar nossos conhecimentos, interagir com outros usuários para expandir nosso network, e utilizá-lo profissionalmente para buscarmos vagas de trabalho.

    1. Aprendi que um LinkedIn bem organizado e com estratégias de qualidades pode nos dar mais oportunidades para conseguirmos ter mais visibilidade e oportunidade de trabalho.
    Em especial, na nossa área de programação, nos mostra como profissionais atualizados e se aproximar de pessoas do nosso meio. Utilizar palavras-chave, otimizar nosso perfil, postar conteúdos de qualidade pode dar mais visibilidade e engajamento em nosso perfil.
