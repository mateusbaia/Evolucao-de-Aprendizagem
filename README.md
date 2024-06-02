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

* <div id="funções">Funções  
  
  * Meu conhecimento sobre **funções**, é bem básico, e todo ele da linguagem JavaScript.
  Eu sabia que **funções** em JavaScript são usadas para declarar uma instrução ou até mesmo um conjunto de instruções.
   A sua declaração é geralmente feita da seguinte forma.  
   1. **Palavra de declaração** `function`, utilizada para definir uma função.  

   2. *Nome da função*: geralmente utilizado em funções nomeadas, também pode ser opcional no caso das funções anônimas.

   3. Um ou mais **parâmetros** valores de entrada quando recebidos na função, definidos entre parênteses, e separados por vírgulas quando forem 2 ou mais parâmetros. Eu já vi que em alguns casos parâmetros podem ser opcionais, ainda não sei os reais motivos.  

   4. **Conjunto de instruções** O código que utilizamos para ser executado quando a função for chamada é definido entre `{}` .

   5. A função em `JavaScript` retorna algo. O retorno é chamado pela palavra `return` , quando explicito; caso não seja explicito, a função retornará `undefined`, por padrão.

```js
Exemplo:
// Declaração de função nomeada.
function pessoa(nome) {
    if (nome === "Mateus") {
        return "Acesso Permitido"; // Retorno explícito.
    } else {
        return "Acesso Negado"; // Retorno explícito.
    }
}
let resultado = pessoa("Mateus");
console.log(resultado) // Acesso Permitido . 

// Declaração de uma função anônima atribuída a uma variável.
const anonima = function(play1, play2) {
    //Conjunto de instruções.
    if (play1 === play2) {
        return "Empate"
    } else if (play1 > play2) {
        return "Play1 é o vencedor" // Retorno explícito.
    } else
        return "Play2 é o vencedor" // Retorno explícito.
}

let vencedor = anonima(3, 2)
console.log(vencedor) // Play1 é o vencedor  .

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

</div>

* <div id="tiposDadosII"> Tipos de Dados II

  * Eu possuía um pouco de conhecimentos sobre alguns *tipos de dados II*, como o tipo number, string, boolean, any e void.
    1. Tipo `NUMBER`, é um objeto que nos permite trabalhar com valores numéricos.
    2. Tipo `STRING`, é usado para podermos representar e guardar informações de texto.
    3. Tipo `BOOLEAN` é um tipo usado na programação como um tipo lógico composto por dois valores que podem ser representados de forma numérica, como 0 ou 1, e de forma de texto, falso ou verdadeiro.
    4. Tipo `ANY`, é um tipo flexível e permissivo, ele permite que escrevamos códigos em TypeScript mais próximos ao JavaScript, sem utilizar uma segurança de tipo.
    5. Tipo `VOID`, é um tipo mais útil para retorno de função que não retorna nenhum valor. Caso atribuído a uma variável, pode não ser muito útil ao código, logo que, se tiver uma variável do tipo void, a mesma só poderá ser atribuída com `undefined`.

</div>

* <div id="tiposUtilitários"> Tipos Utilitários
  
  * Eu não tinha conhecimentos sobre os *tipos utilizados*.

</div>

* <div id="métodosStrings"> Métodos de Strings  

  * Eu conhecia um único **Método de Strings**, o método **includes**, ele pode ser usado para verificar se uma string possui um valor específico, e retorna true se conter o valor e false caso contrário.

```js
Exemplo:
// Variável nome, é uma String.
const nome = " Mateus ";
// Variável contemMa, que utiliza o métado includes para verificar se a variável nome contem "MA".
const contemMa = nome.includes("Ma");
// Mensagem no console
console.log(contemMa); //resultado = true;
```

</div>

* <div id="métodosArrays"> Métodos de Arrays  

  * Eu já tinha conhecimentos sobre alguns **Métodos Arrays**, conhecimentos da linguagem de programação JavaScript, como o método `push`, ele adiciona um ou mais elementos ao final do array retornando um novo array.

  ```js
  Exemplo:
  // Método push  
  // Variavel frutas, é um array composto por 3 elementos.
  const frutas = ['Morango', 'Uva', 'Banana'];
  //Adciona o novo elemento, sempre após o ultimo elemento do array.
  frutas.push('Manga');
  console.log(frutas); // ['Morango', 'Uva', 'Banana', 'Manga'] Novo array com a fruta adicionada no final.
  ```  

  * Eu conhecia o método `unshift`, um pouco de semelhança com o método `push`. Ele também adiciona um ou mais elementos dentro do array, mas ao contrário do `push`, ele sempre adiciona os elementos no início do array.

  ```js
  Exemplo:
  // Método unshift
  // Variavel frutas, é um array composto por 3 elementos.
  const frutas = ['Morango', 'Uva', 'Banana'];
  // Adiciona o novo elemento, sempre antés do primeiro elemento do array.
  frutas.unshift('Acerrola') 
  console.log(frutas) // ['Acerrola', 'Morango', 'Uva', 'Banana'] Novo array com a fruta adicionada no inicio.
  ```

  * Eu conhecia o método `pop`, ele remove sempre o último elemento do array e retorna o mesmo e um novo array sem elemento removido.  

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

  * Eu conhecia o método `shift`, ele, assim como o método `pop`, remove um ou mais elementos de dentro do array, mas ao contrário do método `pop`, ele sempre removera os elementos no início do array.  

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

  * Eu conhecia o método `reverse`, ele retorna o aray inverso do que foi passado inicialmente.  

  ```js
  Exemplo:
    // Método reverse
  // VAriavel numeros, é um array com três elementos.
  const numeros = [10, 25, 50];
  // Declaração do método reverse que retorna o array inverso do inicial. 
  numeros.reverse();
  console.log(numeros); // [50, 25, 10] Array inverso.
  ```

  * Eu sabia que, assim como as `Strings`, também podemos usar o método `includes`, para manipular arrays e verificar se contêm o elemento desejável dentro do array, a resposta sempre será true, ou false.  

  ```js
  Exemplo:
  // Método includes
  // Variavel alunos, é um array com três elementos.
  const alunos = ['Mateus', 'Caio', 'Leticia'];
  // verificar se elemento existe dentro do array.
  const temAluno = alunos.includes('Leticia');
  console.log(temAluno); // resultado = true.
  ```

</div>

* <div id="métodosArraysII"> Méttodos de Arrays II  

  * Eu já conhecia um pouco o método ``find`` ele é utilizado para fazer busca em um array através de uma instrução passada, ele retornará o primeiro elemento compatível com a instrução fornecida caso seja encontrado no array. Caso o elemento buscado não seja encontrado, ele retornará `undefined`  

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

  * Eu conhecia também um pouco o método `findIndex` apesar de ter uma sintaxe de uso, a meu ver, idêntica ao `find`, ele tem uma utilidade diferente. O método retorna o índice do elemento caso existente no array, se não for encontrado, o retorno será de −1.  

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

  * Eu tinha um pouco de conhecimento sobre o método `filter`. Ele copia e retorna um novo array, criando uma cópia superficial do array original, com as instruções fornecidas para a implementação da lógica de busca do método `filter`.

  ```js
  // Declaração de um array de objetos com propriedade nome e divida.
  const clientes = [
    { nome: "Mateus", divida: 180 },
    { nome: "Mateus", divida: 280 },
    { nome: "Mateus", divida: 190 }
  ]


  // Declaração do método filter com a variavel dividaMenor200.
  const dividaMenor200 = clientes.filter((cliente) => {
    // Declaração explicita do retorno com as instruções da busca com método filter.
    return cliente.nome === "Mateus" && cliente.divida < 200

  })

  console.log(dividaMenor200) // [ { nome: 'Mateus', divida: 180 }, { nome: 'Mateus', divida: 190 } ]

  ```

</div>

* <div id="métodosArraysIII"> Métodos de Arrays III  

  * Eu conhecia um pouco sobre o método `reduce`, ele aplica uma função de retorno de chamada **redutor** fornecida pelas instruções passando em cada elemento do array retornado um único valor, a primeira vez que o retorno do método é executado seu valor anterior não é existente, então o elemento de índice 0 do array será usado como valor inicial, e a interação será a partir do índice −1.  O valor inicial pode ser fornecido e usado como valor de retorno da primeira chamada do método.

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

</div>
  
### Conteúdos de carreira

* <div id="gestãoTempo"> Gestão de Tempo  

  * Eu conhecia pouco sobre gestão de tempo, sabia que é um processo de planejamento e de controle sobre o tempo que temos e como iremos dividir para uma melhor produtividade do nosso dia.

</div>

* <div id="curCartApre"> Currículo e Carta de Apresentação

  * Eu não conhecia boas práticas de currículo e carta de apresentação.

</div>

* <div id="LinkedIn"> LinkedIn  

  * Eu não conhecia muito sobre o bom uso do LinkedIn.

</div>

## Conteúdos que eu gostraria de aprender sobre os assuntos desse módulo

### Conteúdos de logíca  

* `Funções`  
  1. Gostaria de aprender quais são as melhores formas de declarar *funções*.
  2. Quais tipos de *funções* existem? Elas podem ser aplicadas para melhorar meus códigos e projetos.

* `Tipos de Dados`
  1. O que são os *tipos de dados* e quais são os benefícios do uso deles no meu código e projetos?
  2. Devo aprender e dar muita importância para o uso de *tipos de dados* em meus códigos e projetos.

* `Tipos Utilitarios`
  1. O que são os *tipos úteis*, devo utilizar eles sempre em meus códigos e projetos?

* `Métodos de Strings`
  1. Quais são os *métodos de strings* existentes que devo saber para melhorar meus códigos e projetos?
  2. Quando devo optar pelo uso dos *métodos de strings* em meus códigos?
  3. Existem algumas ocasiões em que não devo fazer uso de *métodos de strings*?

* `Métodos de Arrays`
  1. Em quais tipos de projetos reais é utilizado o uso de *métodos de array*?
  2. Posso fazer uso sempre dos *métodos de array* em meus códigos e projetos?
  3. Quais os ganhos do uso de *métodos de array* em questões de qualidade de código?

* `Métodos de Arrays II`
  1. Além da facilidade de uso de alguns dos *métodos de array II* em alguns códigos, eles trazem mais vantagens para os códigos?
  2. *Métodos de array II* são utilizados por muitas linguagens de programação?
  
* `Métodos de Arrays III`
  1. Quais são as consequências do uso exagerado de *métodos de arrays III* em códigos e projetos reais?
  2. Tenho que saber sobre todos os *métodos de arrys III* ?

### Conteúdos de carreira

* **Gestão de Tempo**
  1. Quais os sinais de que a minha gestão de tempo pode estar sendo mal realizada?
  2. Quais os métodos considerados eficazes para garantir uma melhor gestão de tempo?
  3. Como fazer uma boa gestão de tempo para garantir qualidade no meu trabalho e vida pessoal?

* **Curricúlo e Carta de Aprensentação**
  1. Como devo fazer meus currículos e carta de apresentação?
  2. Existem boas práticas e métodos para deixar meus currículos e carta de apresentação melhor apresentados?
  3. O que nunca fazer em meus currículos e carta de apresentação?
  
* **LinkedIn**
  1. Como ter um LinkedIn profissional e de boa qualidade?
  2. Como devo me apresentar no LinkedIn para conseguir destaque?
  3. Existem métodos para ter um LinkedIn com mais visibilidade pelas redes?

## Coteúdos que eu aprendi nesse módulo  

### Conteúdos lógicos

* `Funções`
  1. Aprendi um pouco mais sobre o conceito de *funções*, que *funções* podem ser criadas para facilitar a repetição de tarefas, agindo como um subprograma dentro de nossos programas, podendo ser reutilizadas sob demanda se necessário.

  2. Aprendi que a área onde é posto nosso processo de instrução através das *funções* é chamada de escopo.

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
  
  4. Eu aprendi que exite outra forma de declara uma função chamada `arrow function`, que basicamente é atribuir uma função a uma variavel, e essa variavel a receber uma função se torna um `function` sua maior diferença entre a declaração de função con a palavra reservada `function` é a sintáxia.

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
     Exemplo:
  // arrow function declarada com a variavel multiplicar, com dois parametros do tipo number e retorno também do tipo number.
  const multiplicar = (valor1: number , valor2: number): number => {
    return valor1 * valor2 //retorno  explicito
  }
  // chamar função com valor1 e valor1
  console.log(multiplicar(25, 35)) // 875
  ```
  
  6. Eu aprendi como faço tipagem de funções com objeto em `TypeScript`.  
  
  ``` ts
  Exemplo: 
  // Declaração dos tipos das propriedades do obejeto.
  type TUsuario = {
  nome: string,
  idade: number,
  altura: number,
  }
  // Declaração da função cadastrarUsuario com parametro usuario que tem o tipo TUsuario, 
  function cadastrarUsuario(usuario: TUsuario) {
    // Retorno explicido
    return ` Usuario Cadastrado: Nome ${usuario.nome}, Idade ${usuario.idade} anos, Altura ${usuario.altura}m `
  }
  // Declaração da variavel novoUsuario que armazena os dados do usuario cadastrado
  const novoUsuario = cadastrarUsuario({
    nome: 'Mateus Baia',
    idade: 28,
    altura: 168
  })

  console.log(novoUsuario) // Usuario Cadstrado: Nome Mateus Baia, Idade 28 anos, Altura 168m
  ```

* `Tipos de dados`
  1. Aprendi que em `TypeScript` temos uma palavra reservada, chamada `Type`, que utilizamos para criar tipos customizados, explicitamente, variáveis, objetos e funções.
  E que posso ter um tipo único, um tipo com objetos, e um array de tipos.

  2. Aprendi que podemos criar os tipos literais, os tipos literais em TypeScript, eles representam tipos que recebem um valor específico e não mais o valor do tipo que foi definido.

  ```ts
  Exemplo:
  //Declaração do tipo personalizado do objeto utilizando tipo literal para as propriedades modelo e marca.
  type TBolaNike = {
    modelo: 'Futebol'
    marca: 'Nike'
  }

  // Array de bolas que recebe o tipo TBolaNike que recebe um array inicialmente vazio.
  const bolas: TBolaNike[] = []

  // Declaração da variável bolas.length para acessar o tamanho do array para ser atribuído um novo objeto.
  bolas[bolas.length] = {
    // Se tentarmos definir outro tipo para as propriedades modelo e marca, veremos um erro, pois as mesmas só podem ser do tipo futebol e Nike.
    modelo: 'Futebol',
    marca: 'Nike'
  }
  ```  

  3. Aprendi que podemos customizar tipos com a união de tipos.

  ```ts
  Exemplo:
  // Declaração da variável propriedade com a união de tipos, nesse exemplo conseguimos ver que a variável propriedade poderá ser um NUMBER, ou uma STRING, ou um boolean
  const propriedade: number | string | boolean = 'Mateus'


  // tambem pode ser feita em um objeto

  //declaração do tipo do objeto, com união de tipos.
  type TCarro = {
    modelo?: string
    marca?: string
    ano?: string | number
  }

  //Declaração da variavel carros que recebe o tipo Tcarro que é um array 
  const carros: TCarro[] = []

  carros[carros.length] = {
    modelo: "gol", // poderá ser uma string ou undefined.
    ano: 2020  // poderá ser uma string number ou undefined.
    // Não foi declarada a propriedade marca, já que todos são opcionais, não é necessária a declaração. 
    // Isso acontece porque o próprio TypeScript já usa a união de tipos quando colocamos uma propriedade como opcional.
  }
  ```
  
### Contúdos carreira

* **Gestão de tempo**  
  1. Eu aprendi que ter uma boa gestão de tempo devemos nos organizar de forma mais produtiva, priorizando as tarefas importantes do nosso dia a dia sem negociação com a procrastinação.
  2.Aprendi que hoje já existem muitas ferramentas que podem nos auxiliar a gerir melhor nosso tempo para conseguirmos ter um controle maior das tarefas consideradas obrigatórias no nosso dia.
  Com isso, conseguimos ser mais produtivos e eficientes, utilizando melhor o nosso tempo de trabalho e a vida pessoal.  

* **Currículo e Carta de Aprensentação**
  1. Aprendi como devo montar um currículo profissional para ter uma boa apresentação, a importância de um currículo bem feito, informações que não devo pôr em meu currículo, e as que são essenciais.
  2. Aprendi o que é uma cover letter e a sua importância para uma busca por vaga de emprego.
  E aprendi como faço para criar uma cover letter, ou carta de apresentação, de qualidade.

* **LinkedIn**
  1. Aprendi que o LinkedIn é uma rede social com foco profissional que devemos utilizar para mostrar nossos conhecimentos, interagir com outros usuários para expandir nosso network, e utilizá-lo profissionalmente para buscarmos vagas de trabalho.
  2. Aprendi que um LinkedIn bem organizado e com estratégias de qualidades pode nos dar mais oportunidades para conseguirmos ter mais visibilidade e oportunidade de trabalho.
  Em especial, na nossa área de programação, nos mostra como profissionais atualizados e se aproximar de pessoas do nosso meio. Utilizar palavras-chave, otimizar nosso perfil, postar conteúdos de qualidade pode dar mais visibilidade e engajamento em nosso perfil.  
