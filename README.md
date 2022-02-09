<h1 align="center">
  <br>
  Conceitos que todo desenvolvedor deve conhecer
  <br>
</h1>

## Introdução

Este repositório foi criado com a intenção de compartilhar oque venho aprendendo durante esse tempo na área para pessoas iniciantes.  

## Conteúdos

1. **[Como funciona a Internet](#1-como-funciona-a-internet)**
2. **[Tipos primitivos](#2-tipos-primitivos)**
3. **[Tipagem Estatica x Tipagem Dinamica](#3-tipagem-estatica-x-tipagem-dinamica)**
4. **[Tipagem Fraca x Tipagem Forte](#4-tipagem-fraca-x-tipagem-forte)**
5. **[Linguagem Compilada x Linguagem Interpretada](#5-linguagem-compilada-x-linguagem-interpretada)**
6. **[Requisitos funcionais x Requisitos não funcionais](#6-requisitos-funcionais-x-requisitos-não-funcionais)**
7. **[Code Smells](#7-code-smells)**
<!-- 6. **[Implícito, Explicito, Nominal, Estruturando e Chamada de métodos](#4-implícito-explícito-nominal-estruturando-e-chamada-de-métodos)**
7. **[== vs === vs typeof](#5--vs--vs-typeof)**
8. **[Escopo da Função, Escopo do Bloco e Escopo Léxico](#6-escopo-da-função-escopo-do-bloco-e-escopo-léxico)**
9. **[Expression vs Statement](#7-expression-vs-statement)**
10. **[IIFE, Modules e Namespaces](#8-iife-modules-e-namespaces)**
11. **[Message Queue e Event Loop](#9-message-queue-e-event-loop)**
12. **[setTimeout, setInterval e requestAnimationFrame](#10-settimeout-setinterval-e-requestanimationframe)**
13. **[JavaScript Engines](#11-javascript-engines)**
14. **[Bitwise Operators, Type Arrays e Array Buffers](#12-bitwise-operators-type-arrays-e-array-buffers)**
15. **[DOM e Layout Trees](#13-dom-e-layout-trees)**
16. **[Factories e Classes](#14-factories-e-classes)**
17. **[this, call, apply e bind](#15-this-call-apply-e-bind)**
18. **[new, Constructor, instanceof e Instances](#16-new-constructor-instanceof-e-instances)**
19. **[Prototype Inheritance e Prototype Chain](#17-prototype-inheritance-e-prototype-chain)**
20. **[Object.create e Object.assign](#18-objectcreate-e-objectassign)**
21. **[map, reduce, filter](#19-map-reduce-filter)**
22. **[Pure Functions, Side Effects e State Mutation](#20-pure-functions-side-effects-e-state-mutation)**
23. **[Closures](#21-closures)**
24. **[Funções de alta ordem](#22-funções-de-alta-ordem)**
25. **[Recursão](#23-recursão)**
26. **[Collections](#24-collections)**
27. **[Promises](#25-promises)**
28. **[async/await](#26-asyncawait)**
29. **[Estrutura dos dados](#27-estrutura-dos-dados)**
30. **[Expensive Operation e Big O Notation](#28-expensive-operation-e-big-o-notation)**
31. **[Algoritmos](#29-algoritmos)**
32. **[Herança, Polimorfismo e Reutilização de Código](#30-herança-polimorfismo-e-reutilização-de-código)**
33. **[Padrões de design](#31-padrões-de-design)**
34. **[Aplicações parciais, Currying, Compose e Pipe](#32-aplicações-parciais-currying-compose-e-pipe)**
35. **[Código limpo (clean)](#33-código-limpo-clean)** -->

---

<!-- ## 1. Pilha de chamadas

### Artigos (inglês/português)

 * 📜 [Entenda de uma vez por todas a pilha de chamadas (Callstack) do JavaScript — André D. Oliveira](https://js.pro.br/callstack-entenda-pilha-chamadas-javascript)
 * 📜 [Understanding Javascript Call Stack, Event Loops — Gaurav Pandvia](https://medium.com/@gaurav.pandvia/understanding-javascript-function-executions-tasks-event-loop-call-stack-more-part-1-5683dea1f5ec)
 * 📜 [Understanding the JavaScript Call Stack — Charles Freeborn](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)
 * 📜 [Javascript: What Is The Execution Context? What Is The Call Stack? — Valentino Gagliardi](https://www.valentinog.com/blog/js-execution-context-call-stack/)
 * 📜 [What is the JS Event Loop and Call Stack? — Jess Telford](https://gist.github.com/jesstelford/9a35d20a2aa044df8bf241e00d7bc2d0)
 * 📜 [Call Stack — MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)
 * 📜 [Understanding Execution Context and Execution Stack in Javascript — Sukhjinder Arora](https://blog.bitsrc.io/understanding-execution-context-and-execution-stack-in-javascript-1c9ea8642dd0)
 * 📜 [How JavaScript Works: An Overview of the Engine, the Runtime, and the Call Stack — Alexander Zlatkov](https://blog.sessionstack.com/how-does-javascript-actually-work-part-1-b0bacc073cf)
 * 📜 [The Ultimate Guide to Execution Contexts, Hoisting, Scopes, and Closures in JavaScript — Tyler McGinnis](https://tylermcginnis.com/ultimate-guide-to-execution-contexts-hoisting-scopes-and-closures-in-javascript/)
 -->
<!-- ### Vídeos

 * 🎥 [Javascript: the Call Stack explained — Coding Blocks India](https://www.youtube.com/watch?v=w6QGEiQceOM)
 * 🎥 [The JS Call Stack Explained In 9 Minutes — Colt Steele](https://www.youtube.com/watch?v=W8AeMrVtFLY)
 * 🎥 [JavaScript Execution Stack — Codecademy](https://www.youtube.com/watch?v=jT0USJeNFEA)
 * 🎥 [What is the Call Stack? — Eric Traub](https://www.youtube.com/watch?v=w7QWQlkLY_s)
 * 🎥 [The Call Stack — Kevin Drumm](https://www.youtube.com/watch?v=Q2sFmqvpBe0)
 * 🎥 [Understanding JavaScript Execution — Codesmith](https://www.youtube.com/watch?v=Z6a1cLyq7Ac&list=PLWrQZnG8l0E4kd1T_nyuVoxQUaYEWFgcD)
 * 🎥 [Call Stack & Event Loop — movies com](https://www.youtube.com/watch?v=mk0lu9MKBto)
 * 🎥 [The Ultimate Guide to Execution Contexts, Hoisting, Scopes, and Closures in JavaScript — Tyler McGinnis](https://www.youtube.com/watch?v=Nt-qa_LlUH0)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)** -->

---


## 1. Como funciona a internet?
    
   A internet é uma rede que interconecta computadores e outros dispositivos como seu celular em escala global para a transfêrencia de dados entre eles. Já o World Wide Web é uma aplicação onde páginas são interligadas através de links e que se utiliza da internet para funcionar. 
    
  - *Você sabe como os computadores comunicam entre si?*

       Toda comunicação é realizada por uma interconexão entre computadores que permite que essa comunicação entre si seja realizada, chamado de rede de computadores. Esta comunicação pode ser feita através de cabos ou sem fios. 
            
      ![image](https://user-images.githubusercontent.com/31746775/153097067-94a86673-c698-4836-b58e-774081130d5d.png)

  - *Bora para um exemplo?*
       
       Vamos supor que você queira acessar o site https://g1.globo.com/ para ler algumas noticias. Você abre seu navegador e digita o endereço, e passos poucos segundos, a página inicial do site é exibida. 
       
   - *Como tudo isso funciona?*
        
        Isso acontece porque os computadores possuem um endereço numérico unico chamado endereço IP, e além desse endereço, possui inúmeras portas por onde as aplicaçãoes e processos se comunicam. Para que você acesse a página desejada, de fato, o seu computador precisa antes estabelecer uma conexão com o compuador onde a pagina solicitada está hospedada. 
        
        Vamos supor que o cliente de endereço IP 177.178.79.80, queira através da porta 65000, iniciar uma conexão com o servidor de endereço IP  185.186.87.88 na porta 80 para obter a página inicial do G1.
        
        ![image](https://user-images.githubusercontent.com/31746775/153097968-072b3764-c97d-4745-8c17-47ac669f403d.png)

   - *Você sabe oque é DNS e portas conhecidas?*
   
      Quando um computador está ligado em rede, ele está configurado para acessar um servidor especial chamado servidor de nomes ou servidor DNS, como é mais conhecido. Este servidor funciona como uma lista telefônica.

      Quando digitamos https://g1.globo.com/ na barra de endereços, estamos informando o endereço ou a URL (Uniform Resource Locator) do site que desejamos acessar. Se o navegador não conhecer o endereço IP para esta URL – afinal, ele deve visitá-la várias vezes ao dia 🙂 – ele se conecta ao servidor DNS e pergunta: 
      
          Olá, tudo bem? Tenho a URL https://g1.globo.com/, você pode me informar o endereço IP dela? 
          Eis que o servidor DNS responde: Pois não, o endereço IP desta URL é 185.186.87.88.

      As portas disponíveis num computador, elas são conhecidas de acordo com o serviço que oferecem. Se precisar de um serviço de transferência de arquivos ou FTP, ele pode ser encontrado na porta 21. Se precisar de um shell remoto e seguro ou SSH, ele estará na porta 22. Se precisar de um serviço de entrega de e-mail ou SMTP, ele estará na porta 25. Ou, ainda, se precisar de um serviço de entrega de páginas web, ele estará na porta 80.

      Todos como se fossem os estabelecimentos do bairro onde você mora, muito bem conhecidos e raramente mudam de lugar.

      O servidor DNS funciona como uma lista telefônica para encontrar o endereço IP da URL solicitada. Já as portas são conhecidas de acordo com os serviços oferecidos. O serviço de entrega de páginas web encontra-se na porta 80 e o serviço de entrega de e-mail encontra-se na porta 25, por exemplo.

      - *TCP/IP, como os computadores se comunicam*
       
        Uma vez conhecido o endereço IP do destino e a porta na qual deseja se conectar, o cliente precisa estabelecer uma conexão com o servidor. A conexão é estabelecida da seguinte maneira:

            Cliente: Boa tarde 185.186.87.88, desejo estabelecer uma conexão na porta 80?
            Servidor: Boa tarde 177.178.79.80. Pode realizar a conexão.
            Cliente: Ok, iniciarei a conexão. Os pacotes começam a ser enviados a partir deste momento…

      Este tipo de conexão utiliza o protocolo TCP ou Transmission Control Protocol e é através deste protocolo que o cliente e o servidor conversam entre si. Através desta conexão ocorre o envio de pacotes, fragmentos menores dos dados que serão trafegados que contém informações como a porta de origem, a porta de destino e a sequência que devem ser reconstruídos ao chegar no destino.

      Este é um tipo especial de conexão pois ela é ponto-a-ponto, ou seja, a comunicação pode ser feita em duas vias (o cliente fala com o servidor e o servidor fala com o cliente). Outra característica importante é a garantia de entrega onde todos os pacotes que saem da origem possuem a garantia de que chegarão ao destino e que serão entregues de forma ordenada e sem modificações. Outra característica importante ainda é o controle de fluxo que controla a quantidade de pacotes enviados ou recebidos aumentando ou diminuindo de acordo com a necessidade.
      
<!-- 
      Ou, numa breve alusão ao serviço de correios de carta registrada, as suas correspondências chegarão ao destino, na ordem correta e não serão violadas ou abertas. E, se sua caixa de correio da sua casa estiver cheia, as correspondências serão entregues numa frequência menor até que sua caixa de correio tenha mais espaço!

      O TCP é um protocolo de rede que permite a comunicação entre computadores e uma conexão deve ser estabelecida antes do início do envio de pacotes. Ele é um protocolo ponto-a-ponto, possui garantia de entrega de pacotes de forma ordenada e sem modificações e possui controle de fluxo.

      Certo, mas o que acontece quando a conexão é estabelecida? Existe uma aplicação conhecida como servidor web que recebe e manipula todos os pacotes que vem pela porta 80. Vamos ver o seu funcionamento mais adiante…

      HTTP, o idioma dos navegadores e servidores web!
      Imagine o seguinte, você mora no prédio localizado no endereço IP 185.186.87.88 e o seu apartamento é o de número 80. O seu trabalho é enviar páginas com as informações variadas para quem as solicita através do correio. Uma pessoa qualquer te envia uma carta solicitando uma página com informações sobre futebol, por exemplo. Você recebe esta carta, abre ela, analisa a solicitação, monta a página com a informação solicitada, coloca a página num envelope e a envia de volta para o remetente. Só que esta comunicação se dá num idioma próprio, que somente vocês entendem.

      Se alguém, por engano, enviar uma carta solicitando uma página com informações sobre viagens para o seu vizinho do 21, o Sr. Fábio Teixeira Pimentel (ou FTP para os íntimos), não receberá nada de volta. Isso acontece porque ele não entenderá o idioma escrito na carta e, de qualquer forma, ele só trabalha com transferência de arquivos e não com o envio de páginas.

      Esse idioma é o HTTP ou Hypertext Transfer Protocol e é o idioma que os navegadores e os servidores web conversam. É através deste idioma que o seu navegador informa ao servidor web qual a sua versão, qual o seu idioma, se aceita conteúdo compactado ou não e qual página foi solicitada. E, da mesma forma, é através deste idioma que o servidor web informa ao seu navegador se a página solicitada existe, qual o seu formato, se a página enviada foi compactada, se existe algum cookie para ser gravado no seu computador e, principalmente, o conteúdo da página solicitada.

      Quando o navegador solicita uma página web é chamado de requisição e quando o servidor web envia a página web solicitada de volta para o navegador é chamado de resposta. Cada requisição realizada pelo navegador é independente umas das outras e, por este motivo, o HTTP é considerado um protocolo sem estado ou stateless. E o que isso quer dizer? Quando você realiza uma nova requisição (ao mudar de página no site, por exemplo) o servidor web não lembra que você realizou uma requisição anterior. -->

        
  
  Não ficou claro, que tal assistir um video? 
  
   * 🎥 [Tipos Primitivos - Curso Introdutório de JavaScript GRATUITO | Trybe](https://www.youtube.com/watch?v=a1NiHwH9clE&ab_channel=Trybe)

**[⬆ Voltar ao topo](#conteúdos)**
   
---

## 2. Tipos primitivos

  - *Oque são tipos de dados primitivos?*
    
    Para criar algoritmos utilizamos variaveis para manipular dados, por exemplo nome, idade, altura. Para otimizar a utilização da memória, cada variavel armazena apenas um tipo de dado. 
    A variável nome, deve armazenar textos, já a variavel idade deve armazenar apenas numeros inteiros, na variavel sexo podemos armazenar apenas caracteres. 
    
  - *Quais são os tipos de dados primitivos?*
      
    Em computação existem apenas 4 tipos, algumas linguagens subdividem esses tipos de dados em outros de acordo com a capacidade de memoria. 
    São eles:
    
          - INTEIRO: Representa valores numéricos negativo ou positivo sem casa decimal, ou seja, valores inteiros. 
          - REAL: Representa valores númericos negativo ou positivo com casa decimal, ou seja valores reais.
          - LOGICO: Representa valores booleanos, assumindo apenas dois estados, VERDADEIRO ou FALSO.
          - TEXTO: Representa uma sequencia de um ou mais caracteres, colocamos os valores do tipo texto entre ""

  Não ficou claro, que tal assistir um video? 
  
   * 🎥 [Tipos Primitivos - Curso Introdutório de JavaScript GRATUITO | Trybe](https://www.youtube.com/watch?v=a1NiHwH9clE&ab_channel=Trybe)

**[⬆ Voltar ao topo](#conteúdos)**
   
---

## 3. Tipagem Estatica x Tipagem Dinamica

  - *Você sabe a diferença entre tipagem Estatica e Dinâmica?*
    
    Linguagens com tipagem estática não permitem ao desenvolvedor alterar o tipo da variavel depois de declarada. Geralmente a verificação de tipo é feita em tempo de compilação. Podemos ver o exemplo na linguagem Java: 


        public class MyClass {
            public static void main(String args[]) {
              int variavel = 10;

              variavel = "Elton Fonseca"; //error: incompatible types: String cannot be converted to int
            }
        }
        

    Já a tipagem Dinâmica esta ligado a habilidade da linguagem de programação em escolher o tipo de dado de acordo com o valor atribuido á variavel em tempo de execução dinamicamente. Veja o exemplo em PHP: 
  
          $variavel = "Elton Fonseca";

          echo gettype($variavel); //string

          $variavel = 340;

          echo gettype($variavel); //integer

          $variavel = 340.89;

          echo gettype($variavel); //double

          $variavel = true;

          echo gettype($variavel); //boolean


    Obs: Isso não quer dizer que as linguagens de tipagem dinâmica não possui tipos, na verdade, ela possui tipos porém a diferença esta apenas na capacidade da linguagem em escolher o tipo automaticamente. 
  
    Algumas linguagens estática podem fazer a inferencia de tipo na declaração de variaveis, mas não permite que o tipo seja alterado após a declaração.  
  
          using System;

          public class Program
          {
              public static void Main()
              {
                  var variavel = "Treinaweb";

                  Console.WriteLine(variavel.GetType()); //System.String

                  variavel = 28; //Compilation error (line 11, col 14): Cannot implicitly convert type 'int' to 'string'
              }
          }
  
    Não ficou claro, que tal assistir um video? 
  
      * 🎥 [Tipagem (Entenda Como Sua Linguagem de Programação Funciona) ](https://www.youtube.com/watch?v=BkkWfeCV2o0&ab_channel=C%C3%B3digoFonteTV)

**[⬆ Voltar ao topo](#conteúdos)**

---

## 4. Tipagem Fraca x Tipagem Forte

  - *Você sabe a diferença entre tipagem fraca e forte?*
    
    A tipagem fraca está ligada a caracteristica da linguagem de realizar conversões automaticamente entre tipos diferentes de dados. Veja o exemplo abaixo em JS: 


        var nome = "Elton Fonseca"; //string

        var idade = 28; //number

        console.log(nome + " " + idade); //Elton Fonseca 28

        

    Linguagens fortemente tipadas não realizam conversões automaticamente. Vamos pegar como exemplo a linguagem Python. Ela possui tipagem forte, se formos executar esse exemplo teriamos um erro:  
  
        nome = "Elton Fonseca" #str
        idade = 28 #int

        print(nome + " " + idade) #TypeError: can only concatenate str (not "int") to str

  
    Não ficou claro, que tal assistir um video? 
    
      * 🎥 [Tipagem (Entenda Como Sua Linguagem de Programação Funciona) ](https://www.youtube.com/watch?v=BkkWfeCV2o0&ab_channel=C%C3%B3digoFonteTV)


**[⬆ Voltar ao topo](#conteúdos)**

---

## 5. Linguagem Compilada x Linguagem Interpretada

   Antes de entramos a fundo sobre a diferença primeiro precisamos lembrar qual é nosso objetivo ao criar um programa. Nosso foco é que o codigo que desenvolvemos seja executado pelo computador e possamos assim ver um resultado na tela, não importa qual linguagem de programação tenhamos usado. Importante lembrar que o compurador não compreende as linguagens de programação, pois ela só entende linguagem de máquina, ou seja (0 e 1) por isso precisamos transformar nosso codigo em binario. 
    
  - *Você sabe a diferença entre linguagem compilada x linguagem interpretada?*
    
    - Codigo Compilado: 
        Compilar significa converter um objeto em outro, ou seja traduzir uma linguagem x em linguagem de maquina atraves de um programa chamado compilador.  
    
    O compilador seleciona o nosso codigo inteiro, converte-o para binario e guarda o resultado em um unico "pacote", como se fosse um "arquivo zipado", que é enviado para nosso cliente final já pronto para ser executado.
    
    ![image](https://github.com/emimuniz/study-guide/blob/main/Asset/linguagemcompilada.png)


    Existem algumas vantagens de usar uma linguagem compilada, primeiro que o cliente final não tem acesso ao codigo-fonte de nosso projeto, visto que recebe apenas o codigo binario para ser executado. Uma outra vantagem é a perfomance, quando compilamos o codigo inteiro, não precisamos ficar repetindo esse processo.
        
      - Codigo Interpretado:
        Quando pensamos em interpretar, pode ser que pensemos em alguém que trabalhe como intérprete. Isso envolve receber uma informação de uma linguagem fonte e transmiti-la de maneira traduzida para uma linguagem alvo.

Uma linguagem interpretada executa um processo similar. Ela será interpretada por meio de um programa chamado interpretador, que irá então converter nosso código para linguagem de máquina. Contudo, esse processo irá ocorrer aos poucos, pois o interpretador irá realizar a conversão analisando linha por linha, e não o programa inteiro, diferentemente do que ocorre com o compilador.

   ![image](https://github.com/emimuniz/study-guide/blob/main/Asset/linguageminterpretada.png)
   
  
Conseguimos perceber que o processo de interpretação será mais lento, pois será executado de maneira repetida, e isso diminui a performance. Sabemos que nosso usuário final provavelmente não irá perceber essa diferença de velocidade, pois isso ocorre por “debaixo dos panos”. Entretanto, sabemos que esse é um fator muito importante em qualquer programa.

Mesmo possuindo a desvantagem da performance, as linguagens interpretadas possuem a vantagem de ser mais simples de “debugar”. Como a interpretação ocorre aos poucos, podemos visualizar com mais facilidade os erros que podem aparecer, e se constatarmos algum problema, poderemos prontamente resolvê-los. Isso é uma vantagem do código interpretado em relação ao compilado, que é mais difícil de debugar, visto que o código é executado todo de uma só vez.

   - JIT: 
     Quando falamos de JIT na programação, estamos nos referindo a uma técnica que envolve mesclar conceitos de códigos compilados e interpretados. Com o JIT nós continuamos a interpretar os códigos. 

Entretanto, nós também iremos compilá-los, mas apenas a parte do código que iremos usar no momento da execução. Isso representa um aumento muito grande de performance. Pois iremos usar o processo de compilação, que já é rápido, e ele será executado em partes isoladas do código, apenas na hora certa (“just in time”).

Assim, nós temos à nossa disposição “o melhor dos dois mundos”. Temos a velocidade da compilação junto com a simplicidade de debugar nosso código.

Linguagens que implementaram a técnica do JIT notaram grandes mudanças no desempenho dos seus códigos. Entre esses exemplos estão o JavaScript e o PHP a partir da versão 8.

Não ficou claro, que tal assistir um video? 
  
   * 🎥 [Como Funcionam as Linguagens](https://www.youtube.com/watch?v=Ol8KcAc7N2c&t=572s&ab_channel=EstudonautaCursos)


**[⬆ Voltar ao topo](#conteúdos)**

---

## 6. Requisitos funcionais x Requisitos não funcionais

   Requisitos funcionais definem o que um sistema deve fazer; isto é, quais funcionalidades ou serviços ele deve implementar. 
   Já os requisitos não funcionais definem como um sistema deve operar, sob quais restrições e com qual qualidade de serviço. 
   
   São exemplos de não funcionais:
       - Desempenho 
       - Disponibilidade
       - Tolerância a falhas
       - Segurança 
       - Privacidade 
       - Interoperabilidade 
       - Capacidade
       - Manutenibilidade
       - Usabiidade
       
       
  Que tal um exemplo?
     Vamos supor que você tenha que informar os requisitos de um sistema home-banking. 
     
     Quais serão os requisitos funcionais?
        - Informar o saldo da conta
        - Realizar a trânsferencia entre contas
        - Pagar o boleto bancário
        - Cancelar um cartão de Credito 
        
     Quais serão os requisitos não funcionais?
        - Desempenho: Informar o saldo da conta em menos de 5segundos.
        - Disponibilidade: Estar no ar 99.99% do tempo.
        - Tolerância a falhas: Continuar operando mesmo se um centro de dados sair.
        - Segurança: Criptografar todos os dados trocados com as agências.
        - Privacidade: Não disponibilizar para terceiros dados dos clientes.
        - Interoperabilidade: Integrar-se com os sistemas do Banco Central.
        - Capacidade: Ser capaz de armazenar dados de 1 milhão de clientes.
        - Usabilidade: Ter uma versão para deficientes visuais
     

Não ficou claro, que tal assistir um video? 
  
   * 🎥 [Requisito Funcional e Não Funcional de Software: entenda a diferença.](https://www.youtube.com/watch?v=YLd6AWKVyas&ab_channel=pessonizando)


**[⬆ Voltar ao topo](#conteúdos)**

---

## 7. Code Smells

   Também conhecidos como bad smells - são indicadores de código de baixa qualidade, isto é, código dificil de manter, entender, modificar ou testar. Em resumo codigo que não esta "cheirando bem" e que portanto talvez possa ser refatorada. No entanto, nessa definição, o termo "indicadores" significa que não devemos considerar que todo code smell deve ser imediatamente refatorado. Essa decisão depende de outros fatores, como importancia do trecho de codigo e a frequência com ele precisará ser mantido. 
   

   - *Código Duplicado*
    
   Esse principal code smell e aquele com maior potencial para prejudicar a evolução de um sistema. Codigo duplicado aumenta o esforço de manutenção, pois alterações têm que ser replicadas em mais de uma parte do código. Corre-se o risco de alterar uma parte e esquecer de uma outra. 
    
   - *Métodos Longos*
   
   Em qualquer sistema, métodos devem ser pequenos, com nomes auto-explicativos e poucas linhas de código. Métodos Longos são considerados um code smell, pois eles tornam o código mais dificil de entender e manter. Quando nos deparamos com um método longo, devemos considerar a possibilidade de usar uma estração de Método para quebra-lo em métodos menores. 
   
   - *Classes Grandes*
  
  Assim como métodos, classes não devem assumir mais responsabilidades e prover serviços que não são coesos. Por isso, Classes Grandes é considerado um code smell, pois, assim como métodos longos, elas tornam o código mais dificil de entender e manter. Além de ser mais difícil de reusar essas classes em outro pacote ou sistema. Classes grandes são caracterizadas por um grande número de atributos, com baixa coesão entre eles. 
  
  - *Feature Envy* 
  
  Esse smell designa um método que aparece "injevar" os dados e métodos de uma outra classe. Dizendo de outro modo, ele acessa mais atributos e métodos de uma classe B do que sua classe A. Portanto, deve-se analisar a possibilidade de usar Movimentação de Método para migra-lo para classe "invejada"
  
  - *Métodos com muitos Parâmetros*
  
  Além de pequenos, métodos, na medida do possivel devem ter poucos parâmetros. Isto é, metódos com muitos parâmetros é um smell, que pode ser eliminado de duas formas principais. Primeiro, deve-se verificar se um dos parametros pode ser obtido diretamente pelo método chamado. 



Não ficou claro, que tal assistir um video? 
  
   * 🎥 [Code Smell (A arte de farejar código ruim)](https://www.youtube.com/watch?v=SQqqiC0YpA0&ab_channel=C%C3%B3digoFonteTV)


**[⬆ Voltar ao topo](#conteúdos)**

---


<!-- ## 4. Implícito, Explícito, Nominal, Estruturando e Chamada de métodos

### Artigos (inglês)

 * 📜 [What you need to know about Javascript's Implicit Coercion — Promise Tochi](https://dev.to/promhize/what-you-need-to-know-about-javascripts-implicit-coercion-e23)
 * 📜 [JavaScript Type Coercion Explained — Alexey Samoshkin](https://medium.freecodecamp.org/js-type-coercion-explained-27ba3d9a2839)
 * 📜 [Javascript Coercion Explained — Ben Garrison](https://hackernoon.com/javascript-coercion-explained-545c895213d3)
 * 📜 [What exactly is Type Coercion in Javascript? - Stack Overflow](https://stackoverflow.com/questions/19915688/what-exactly-is-type-coercion-in-javascript)
 * 📜 [You Don't Know JS: Types & Grammar [Book] — Kyle Simpson](https://www.oreilly.com/library/view/you-dont-know/9781491905159/ch04.html)
 * 📜 [(Not) Everything in JavaScript is an Object - Daniel Li](http://blog.brew.com.hk/not-everything-in-javascript-is-an-object/)
 * 📜 [Type Coercion in JavaScript, and why everyone gets it wrong.](https://thedevs.network/blog/type-coercion-in-javascript-and-why-everyone-gets-it-wrong)

 ### Vídeos

 * 🎥 [== ? === ??? ...#@^% - Shirmung Bielefeld](https://www.youtube.com/watch?v=qGyqzN0bjhc&t)
 * 🎥 [Coercion in Javascript - Hitesh Choudhary](https://www.youtube.com/watch?v=b04Q_vyqEG8)
 * 🎥 [JavaScript Questions: What is Coercion? - Steven Hancock](https://www.youtube.com/watch?v=z4-8wMSPJyI)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 5. == vs === vs typeof

### Artigos (inglês)

 * 📜 [JavaScript Double Equals vs. Triple Equals — Brandon Morelli](https://codeburst.io/javascript-double-equals-vs-triple-equals-61d4ce5a121a)
 * 📜 [What is the difference between =, ==, and === in JS? — Codecademy](https://www.codecademy.com/en/forum_questions/558ea4f5e39efed371000508)
 * 📜 [Should I use === or == equality comparison operator in JavaScript? — Panu Pitkamaki](https://bytearcher.com/articles/equality-comparison-operator-javascript/)
 * 📜 [== vs === JavaScript: Double Equals and Coercion — AJ Meyghani](https://www.codementor.io/javascript/tutorial/double-equals-and-coercion-in-javascript)
 * 📜 [Why Use the Triple-Equals Operator in JavaScript? — Louis Lazaris](https://www.impressivewebs.com/why-use-triple-equals-javascipt/)
 * 📜 [What is the difference between == and === in JavaScript? — Craig Buckler](https://www.oreilly.com/learning/what-is-the-difference-between-and-in-javascript)
 * 📜 [Why javascript's typeof always return "object"? — Stack Overflow](https://stackoverflow.com/questions/3787901/why-javascripts-typeof-always-return-object)
 * 📜 [Checking Types in Javascript — Toby Ho](http://tobyho.com/2011/01/28/checking-types-in-javascript/)
 * 📜 [How to better check data types in JavaScript — Webbjocke](https://webbjocke.com/javascript-check-data-types/)
 * 📜 [Checking for the Absence of a Value in JavaScript — Tomer Aberbach](https://tomeraberba.ch/html/post/checking-for-the-absence-of-a-value-in-javascript.html)

 ### Artigos (português)

 * 📜 [Qual é a diferença entre "==" e "===" no JavaScript ?](https://spacetraveling-tun.vercel.app/post/javascript-e-uma-linguagem-de-tipagem-dinamica.-isso)

### Vídeos

 * 🎥 [JavaScript - The typeof operator — Java Brains](https://www.youtube.com/watch?v=ol_su88I3kw)
 * 🎥 [Javascript typeof operator — DevDelight](https://www.youtube.com/watch?v=qPYhTPt_SbQ)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 6. Escopo da Função, Escopo do Bloco e Escopo léxico

### Artigos (inglês)

 * 📜 [You Don't Know JS: Scope & Closures [Book] — Kyle Simpson](https://github.com/getify/You-Dont-Know-JS/blob/1st-ed/scope%20%26%20closures/ch3.md)
 * 📜 [The battle between Function Scope and Block Scope — Marius Herring](http://www.deadcoderising.com/2017-04-11-es6-var-let-and-const-the-battle-between-function-scope-and-block-scope/)
 * 📜 [Emulating Block Scope in JavaScript — Josh Clanton](http://adripofjavascript.com/blog/drips/emulating-block-scope-in-javascript.html)
 * 📜 [The Difference Between Function and Block Scope in JavaScript — Joseph Cardillo](https://medium.com/@josephcardillo/the-difference-between-function-and-block-scope-in-javascript-4296b2322abe)
 * 📜 [Function Scopes and Block Scopes in JavaScript — Samer Buna](https://edgecoders.com/function-scopes-and-block-scopes-in-javascript-25bbd7f293d7)
 * 📜 [Understanding Scope and Context in JavaScript | Ryan Morr](http://ryanmorr.com/understanding-scope-and-context-in-javascript/)
 * 📜 [JavaScript Scope and Closures — Zell Liew](https://css-tricks.com/javascript-scope-closures/)
 * 📜 [Understanding Scope in JavaScript — Wissam Abirached](https://developer.telerik.com/topics/web-development/understanding-scope-in-javascript/)
 * 📜 [Speaking JavaScript - Variables: Scopes, Environments, and Closures — Dr. Axel Rauschmayer](http://speakingjs.com/es5/ch16.html)
 * 📜 [Understanding Scope in JavaScript ― Hammad Ahmed](https://scotch.io/tutorials/understanding-scope-in-javascript)

### Vídeos

 * 🎥 [What Makes Javascript Weird ... and Awesome pt. 4 — LearnCode.academy](https://www.youtube.com/watch?v=SBwoFkRjZvE)
 * 🎥 [Variable Scope in JavaScript — Kirupa Chinnathambi](https://www.youtube.com/watch?v=dhp57T3p760)
 * 🎥 [JavaScript Block Scope and Function Scope — mmtuts](https://www.youtube.com/watch?v=aK_nuUAdr8E)
 * 🎥 [What the Heck is Lexical Scope? — NWCalvank](https://www.youtube.com/watch?v=GhNA0r10MmA)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 7. Expression vs Statement

### Artigos (inglês)

 * 📜 [All you need to know about Javascript's Expressions, Statements and Expression Statements — Promise Tochi](https://dev.to/promhize/javascript-in-depth-all-you-need-to-know-about-expressions-statements-and-expression-statements-5k2)
 * 📜 [Function Expressions vs Function Declarations — Paul Wilkins](https://www.sitepoint.com/function-expressions-vs-declarations/)
 * 📜 [JavaScript Function — Declaration vs Expression — Ravi Roshan](https://medium.com/@raviroshan.talk/javascript-function-declaration-vs-expression-f5873b8c7b38)
 * 📜 [Function Declarations vs. Function Expressions — Mandeep Singh](https://medium.com/@mandeep1012/function-declarations-vs-function-expressions-b43646042052)
 * 📜 [Function Declarations vs. Function Expressions — Anguls Croll](https://javascriptweblog.wordpress.com/2010/07/06/function-declarations-vs-function-expressions/)

### Vídeos

 * 🎥 [Expressions vs. Statements in JavaScript — Hexlet](https://www.youtube.com/watch?v=WVyCrI1cHi8)
 * 🎥 [JavaScript - Expression vs. Statement — WebTunings](https://www.youtube.com/watch?v=3jDpNGJkupA)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 8. IIFE, Modules e Namespaces

### Artigos (inglês)

 * 📜 [Mastering Immediately-Invoked Function Expressions ― Chandra Gundamaraju](https://medium.com/@vvkchandra/essential-javascript-mastering-immediately-invoked-function-expressions-67791338ddc6)
 * 📜 [Do ES6 Modules make the case of IIFEs obsolete?](https://hashnode.com/post/do-es6-modules-make-the-case-of-iifes-obsolete-civ96wet80scqgc538un20es0)
 * 📜 [A 10 minute primer to JavaScript modules, module formats, module loaders and module bundlers ― Jurgen Van de Moere](https://www.jvandemo.com/a-10-minute-primer-to-javascript-modules-module-formats-module-loaders-and-module-bundlers/)
 * 📜 [Modules ― Exploring JS](http://exploringjs.com/es6/ch_modules.html)
 * 📜 [ES modules: A cartoon deep-dive — Lin Clark](https://hacks.mozilla.org/2018/03/es-modules-a-cartoon-deep-dive/)
 * 📜 [Understanding ES6 Modules — Craig Buckler](https://www.sitepoint.com/understanding-es6-modules/)
 * 📜 [An overview of ES6 Modules in JavaScript — Brent Graham](https://blog.cloud66.com/an-overview-of-es6-modules-in-javascript/)
 * 📜 [ES6 Modules in Depth — Nicolás Bevacqua](https://ponyfoo.com/articles/es6-modules-in-depth)
 * 📜 [ES6 modules, Node.js and the Michael Jackson Solution — Alberto Gimeno](https://medium.com/dailyjs/es6-modules-node-js-and-the-michael-jackson-solution-828dc244b8b)

### Vídeos

 * 🎥 [Immediately Invoked Function Expression - Beau teaches JavaScript — freeCodeCamp](https://www.youtube.com/watch?v=3cbiZV4H22c)
 * 🎥 [Understanding JavaScript IIFE](https://www.youtube.com/watch?v=I5EntfMeIIQ)
 * 🎥 [JavaScript Modules: ES6 Import and Export — Kyle Robinson](https://www.youtube.com/watch?v=_3oSWwapPKQ)
 * 🎥 [ES6 - Modules — Ryan Christiani](https://www.youtube.com/watch?v=aQr2bV1BPyE)
 * 🎥 [ES6 Modules in the Real World — Sam Thorogood](https://www.youtube.com/watch?v=fIP4pjAqCtQ)
 * 🎥 [ES6 Modules — TempleCoding](https://www.youtube.com/watch?v=5P04OK6KlXA)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 9. Message Queue e Event Loop

### Artigos (inglês)

 * 📜 [JavaScript Event Loop Explained — Anoop Raveendran](https://medium.com/front-end-hacking/javascript-event-loop-explained-4cd26af121d4)
 * 📜 [The JavaScript Event Loop: Explained — Erin Sweson-Healey](https://blog.carbonfive.com/2013/10/27/the-javascript-event-loop-explained/)
 * 📜 [What is the Event Loop in Javascript — WP Tutor.io](https://www.wptutor.io/web/js/javascript-event-loop)
 * 📜 [Understanding JS: The Event Loop — Alexander Kondov](https://hackernoon.com/understanding-js-the-event-loop-959beae3ac40)
 * 📜 [Understanding the JavaScript Event Loop — Ashish Gupta](https://www.zeolearn.com/magazine/understanding-the-javascript-event-loop)
 * 📜 [Event Loop in Javascript — Manjula Dube](https://code.likeagirl.io/what-the-heck-is-event-loop-1e414fccef49)
 * 📜 [The JavaScript Event Loop — Flavio Copes](https://flaviocopes.com/javascript-event-loop/)
 * 📜 [How JavaScript works: Event loop — Alexander Zlatkov](https://blog.sessionstack.com/how-javascript-works-event-loop-and-the-rise-of-async-programming-5-ways-to-better-coding-with-2f077c4438b5)

### Vídeos

 * 🎥 [What the heck is the event loop anyway? | JSConf EU — Philip Roberts](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
 * 🎥 [JavaScript Event Loop — ComScience Simplified](https://www.youtube.com/watch?v=XzXIMZMN9k4)
 * 🎥 [I'm stuck in an Event Loop — Philip Roberts](https://www.youtube.com/watch?v=6MXRNXXgP_0)
 * 🎥 [In The Loop - Jake Archibald | JSConf.Asia 2018](https://www.youtube.com/watch?v=cCOL7MC4Pl0)


**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 10. setTimeout, setInterval e requestAnimationFrame

### Artigos (inglês)

 * 📜 [setTimeout and setInterval — JavaScript.Info](https://javascript.info/settimeout-setinterval)
 * 📜 [Why not to use setInterval — Akanksha Sharma](https://dev.to/akanksha_9560/why-not-to-use-setinterval--2na9)
 * 📜 [setTimeout VS setInterval — Develoger](https://develoger.com/settimeout-vs-setinterval-cff85142555b)
 * 📜 [Using requestAnimationFrame — Chris Coyier](https://css-tricks.com/using-requestanimationframe/)
 * 📜 [Understanding JavaScript's requestAnimationFrame() — JavaScript Kit](http://www.javascriptkit.com/javatutors/requestanimationframe.shtml)
 * 📜 [Handling time intervals in JavaScript - Amit Merchant](https://www.amitmerchant.com/Handling-Time-Intervals-In-Javascript/)

### Vídeos

 * 🎥 [Javascript: How setTimeout and setInterval works — Coding Blocks India](https://www.youtube.com/watch?v=6bPKyl8WYWI)
 * 🎥 [setTimeout and setInterval in JavaScript — techsith](https://www.youtube.com/watch?v=TbCgGWe8LN8)
 * 🎥 [JavaScript Timers — Steve Griffith](https://www.youtube.com/watch?v=0VVJSvlUgtg)
 * 🎥 [JavaScript setTimeout, setInterval & clearInterval — DoingITeasyChannel](https://www.youtube.com/watch?v=BVALvvy5bZY)
 * 🎥 [JavaScript setTimeOut and setInterval Explained — Theodore Anderson](https://www.youtube.com/watch?v=mVKfrWCOB60)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 11. JavaScript Engines

### Artigos (inglês)

 * 📜 [JavaScript Engines — Jen Looper](http://www.softwaremag.com/javascript-engines/)
 * 📜 [Understanding How the Chrome V8 Engine Translates JavaScript into Machine Code — DroidHead](https://medium.freecodecamp.org/understanding-the-core-of-nodejs-the-powerful-chrome-v8-engine-79e7eb8af964)
 * 📜 [Understanding V8’s Bytecode — Franziska Hinkelmann](https://medium.com/dailyjs/understanding-v8s-bytecode-317d46c94775)
 * 📜 [How the V8 engine works? — Thibault Laurens](http://thibaultlaurens.github.io/javascript/2013/04/29/how-the-v8-engine-works/)
 * 📜 [A Brief History of Google’s V8 Javascript Engine — Clair Smith](https://www.mediacurrent.com/blog/brief-history-googles-v8-javascript-engine/)
 * 📜 [JavaScript essentials: why you should know how the engine works - Rainer Hahnekamp](https://medium.freecodecamp.org/javascript-essentials-why-you-should-know-how-the-engine-works-c2cc0d321553)

### Artigos (português)

 * 📜 [Programação assíncrona, Event Loop e NodeJs](https://spacetraveling-tun.vercel.app/post/a-programacao-assincrona)

### Vídeos

 * 🎥 [JavaScript Engines: The Good Parts™ — Mathias Bynens & Benedikt Meurer](https://www.youtube.com/watch?v=5nmpokoRaZI)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 12. Bitwise Operators, Type Arrays e Array Buffers

### Artigos (inglês)

 * 📜 [Programming with JS: Bitwise Operations — Alexander Kondov](https://hackernoon.com/programming-with-js-bitwise-operations-393eb0745dc4)
 * 📜 [Using JavaScript’s Bitwise Operators in Real Life — ian m](https://codeburst.io/using-javascript-bitwise-operators-in-real-life-f551a731ff5)
 * 📜 [JavaScript Bitwise Operators — w3resource](https://www.w3resource.com/javascript/operators/bitwise-operator.php)
 * 📜 [Bitwise Operators in Javascript — Joe Cha](https://medium.com/bother7-blog/bitwise-operators-in-javascript-65c4c69be0d3)
 * 📜 [A Comprehensive Primer on Binary Computation and Bitwise Operators in Javascript — Paul Brown](https://medium.com/techtrument/a-comprehensive-primer-on-binary-computation-and-bitwise-operators-in-javascript-81acf8341f04)

 ### Vídeos

 * 🎥 [JavaScript Bitwise Operators — Programming with Mosh](https://www.youtube.com/watch?v=mesu75PTDC8)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 13. DOM e Layout Trees

### Artigos (inglês)

 * 📜 [How To Understand and Modify the DOM in JavaScript — Tania Rascia](https://www.digitalocean.com/community/tutorials/introduction-to-the-dom)
 * 📜 [JavaScript DOM Tutorial with Example — Guru99](https://www.guru99.com/how-to-use-dom-and-events-in-javascript.html)
 * 📜 [What is the DOM? — Chris Coyier](https://css-tricks.com/dom/)
 * 📜 [Traversing the DOM with JavaScript — Zell Liew](https://zellwk.com/blog/dom-traversals/)
 * 📜 [Eloquent JavaScript [Book] — The Document Object Model](https://eloquentjavascript.net/14_dom.html)
 * 📜 [DOM Tree](https://javascript.info/dom-nodes)
 * 📜 [Render Tree Construction — Ilya Grigorik](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-tree-construction)

 ### Vídeos

 * 🎥 [JavaScript DOM — The Net Ninja](https://www.youtube.com/watch?v=FIORjGvT0kk)
 * 🎥 [JavaScript DOM Crash Course — Traversy Media](https://www.youtube.com/watch?v=0ik6X4DJKCc)


**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 14. Factories e Classes

### Artigos (inglês)

 * 📜 [How To Use Classes in JavaScript — Tania Rascia](https://www.digitalocean.com/community/tutorials/understanding-classes-in-javascript)
 * 📜 [Javascript Classes — Under The Hood — Majid](https://medium.com/tech-tajawal/javascript-classes-under-the-hood-6b26d2667677)
 * 📜 [ES6 Classes — Nathaniel Foster](https://www.javascriptjanuary.com/blog/es6-classes)
 * 📜 [Better JavaScript with ES6, Pt. II: A Deep Dive into Classes ― Peleke Sengstacke](https://scotch.io/tutorials/better-javascript-with-es6-pt-ii-a-deep-dive-into-classes)
 * 📜 [Understand the Factory Design Pattern in Plain JavaScript — Aditya Agarwal](https://medium.com/front-end-hacking/understand-the-factory-design-pattern-in-plain-javascript-20b348c832bd)
 * 📜 [JavaScript Factory Functions vs Constructor Functions vs Classes — Eric Elliott](https://medium.com/javascript-scene/javascript-factory-functions-vs-constructor-functions-vs-classes-2f22ceddf33e)
 * 📜 [JavaScript Factory Functions with ES6+ — Eric Elliott](https://medium.com/javascript-scene/javascript-factory-functions-with-es6-4d224591a8b1)
 * 📜 [Factory Functions in JavaScript — Josh Miller](https://atendesigngroup.com/blog/factory-functions-javascript)
 * 📜 [The Factory Pattern in JS ES6 — SnstsDev](https://medium.com/@SntsDev/the-factory-pattern-in-js-es6-78f0afad17e9)
 * 📜 [Class vs Factory function: exploring the way forward — Cristi Salcescu](https://medium.freecodecamp.org/class-vs-factory-function-exploring-the-way-forward-73258b6a8d15)

 ### Vídeos

 * 🎥 [JavaScript Factory Functions — Programming with Mosh](https://www.youtube.com/watch?v=jpegXpQpb3o)
 * 🎥 [Factory Functions in JavaScript — Fun Fun Function](https://www.youtube.com/watch?v=ImwrezYhw4w)
 * 🎥 [Javascript Tutorial Function Factories — Crypto Chan](https://www.youtube.com/watch?v=R7-IwpH80UE)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 15. this, call, apply e bind

### Artigos (inglês)

 * 📜 [How-to: call() , apply() and bind() in JavaScript — Niladri Sekhar Dutta](https://www.codementor.io/niladrisekhardutta/how-to-call-apply-and-bind-in-javascript-8i1jca6jp)
 * 📜 [JavaScript’s Apply, Call, and Bind Methods are Essential for JavaScript Professionals — Richard Bovell](http://javascriptissexy.com/javascript-apply-call-and-bind-methods-are-essential-for-javascript-professionals/)
 * 📜 [WTF is this - Understanding the this keyword, call, apply, and bind in JavaScript — Tyler McGinnis](https://tylermcginnis.com/this-keyword-call-apply-bind-javascript/)
 * 📜 [Javascript: call(), apply() and bind() — Omer Goldberg](https://medium.com/@omergoldberg/javascript-call-apply-and-bind-e5c27301f7bb)
 * 📜 [The difference between call / apply / bind — Ivan Sifrim](https://medium.com/@ivansifrim/the-differences-between-call-apply-bind-276724bb825b)
 * 📜 [call(), apply() and bind() methods in JavaScript](https://tech.io/playgrounds/9799/learn-solve-call-apply-and-bind-methods-in-javascript)
 * 📜 [Mastering 'this' in JavaScript: Callbacks and bind(), apply(), call() — Michelle Gienow](https://thenewstack.io/mastering-javascript-callbacks-bind-apply-call/)
 * 📜 [JavaScript’s apply, call, and bind explained by hosting a cookout — Kevin Kononenko](https://dev.to/kbk0125/javascripts-apply-call-and-bind-explained-by-hosting-a-cookout-32jo)
 * 📜 [How AND When to use bind, call, and apply in Javascript — Eigen X](https://www.eigenx.com/blog/https/mediumcom/eigen-x/how-and-when-to-use-bind-call-and-apply-in-javascript-77b6f42898fb)
 * 📜 [JavaScript .bind() vs .apply() and .call() — Hack Sparrow](https://www.hacksparrow.com/javascript-bind-vs-apply-and-call.html)
 * 📜 [call() — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/call)
 * 📜 [bind() — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Function/bind)
 * 📜 [apply() — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/apply)
 * 📜 [What is 'this' in JavaScript? — Daniel Li](http://blog.brew.com.hk/what-is-this-in-javascript/)
 * 📜 [Let me explain to you what is `this`. (Javascript) — Jason Yu](https://dev.to/ycmjason/let-me-explain-to-you-what-is-this-javascript-44ja)

  ### Vídeos

 * 🎥 [JavaScript call, apply and bind — techsith](https://www.youtube.com/watch?v=c0mLRpw-9rI)
 * 🎥 [JavaScript Practical Applications of Call, Apply and Bind functions— techsith](https://www.youtube.com/watch?v=AYVYxezrMWA)
 * 🎥 [JavaScript (call, bind, apply) — curious aatma](https://www.youtube.com/watch?v=Uy0NOXLBraE)
 * 🎥 [Understanding Functions and 'this' In The World of ES2017 — Bryan Hughes](https://www.youtube.com/watch?v=AOSYY1_np_4)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 16. new, Constructor, instanceof e Instances

### Artigos (inglês)

 * 📜 [JavaScript For Beginners: the ‘new’ operator — Brandon Morelli](https://codeburst.io/javascript-for-beginners-the-new-operator-cee35beb669e)
 * 📜 [Let’s demystify JavaScript’s ‘new’ keyword — Cynthia Lee](https://medium.freecodecamp.org/demystifying-javascripts-new-keyword-874df126184c)
 * 📜 [Constructor, operator "new" — JavaScript.Info](https://javascript.info/constructor-new)
 * 📜 [Understanding JavaScript Constructors — Faraz Kelhini](https://css-tricks.com/understanding-javascript-constructors/)
 * 📜 [Use Constructor Functions — Openclassrooms](https://openclassrooms.com/en/courses/3523231-learn-to-code-with-javascript/4379006-use-constructor-functions)
 * 📜 [Beyond `typeof` and `instanceof`: simplifying dynamic type checks — Dr. Axel Rauschmayer](http://2ality.com/2017/08/type-right.html)
 * 📜 [What Is the Instanceof Operator in JavaScript — appendTo](https://appendto.com/2016/10/what-is-the-instanceof-operator-in-javascript/)
 * 📜 [JavaScript instanceof vs typeof — Gary Rafferty](http://garyrafferty.com/2012/12/07/JavaScript-instanceof-vs-typeof.html)
 * 📜 [Function and Object, instances of each other — Kiro Risk](https://javascriptrefined.io/function-and-object-instances-of-each-other-1e1095d5faac)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 17. Prototype Inheritance e Prototype Chain

### Artigos (inglês)

 * 📜 [Javascript : Prototype vs Class — Valentin PARSY](https://medium.com/@parsyval/javascript-prototype-vs-class-a7015d5473b)
 * 📜 [JavaScript engine fundamentals: optimizing prototypes — Mathias Bynens](https://mathiasbynens.be/notes/prototypes)
 * 📜 [JavaScript Prototype — NC Patro](https://codeburst.io/javascript-prototype-cb29d82b8809)
 * 📜 [Prototype in Javascript — Sandeep Ranjan](https://www.codementor.io/sandeepranjan2007/prototype-in-javascipt-knbve0lqo)
 * 📜 [Prototypes in JavaScript — Rupesh Mishra](https://hackernoon.com/prototypes-in-javascript-5bba2990e04b)
 * 📜 [Prototype in JavaScript: it’s quirky, but here’s how it works — Pranav Jindal](https://medium.freecodecamp.org/prototype-in-js-busted-5547ec68872)
 * 📜 [Inheritance and the prototype chain — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)
 * 📜 [Master the JavaScript Interview: What’s the Difference Between Class & Prototypal Inheritance? — Eric Elliott](https://medium.com/javascript-scene/master-the-javascript-interview-what-s-the-difference-between-class-prototypal-inheritance-e4cd0a7562e9)
 * 📜 [Understanding JavaScript: Prototype and Inheritance — Alexander Kondov](https://hackernoon.com/understanding-javascript-prototype-and-inheritance-d55a9a23bde2)
 * 📜 [Prototypal Inheritance — JavaScript.Info](https://javascript.info/prototype-inheritance)
 * 📜 [How To Work with Prototypes and Inheritance in JavaScript — Tania Rascia](https://www.digitalocean.com/community/tutorials/understanding-prototypes-and-inheritance-in-javascript)
 * 📜 [Master JavaScript Prototypes & Inheritance — Arnav Aggarwal](https://codeburst.io/master-javascript-prototypes-inheritance-d0a9a5a75c4e)
 * 📜 [You Don't Know JS [Book] Chapter 5: Prototypes — Kyle Simpson](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20%26%20object%20prototypes/ch5.md)
 * 📜 [JavaScript’s Prototypal Inheritance Explained Using CSS — Nash Vail](https://medium.freecodecamp.org/understanding-prototypal-inheritance-in-javascript-with-css-93b2fcda75e4)
 * 📜 [Prototypal Inheritance in JavaScript — Jannis Redmann](https://gist.github.com/derhuerst/a585c4916b1c361cc6f0)
 * 📜 [Classical and Prototypical Inheritance in JavaScript — Danny Cornelisse](http://www.competa.com/blog/classical-prototypical-inheritance-javascript/)
 * 📜 [Demystifying ES6 Classes And Prototypal Inheritance ― Neo Ighodaro](https://scotch.io/tutorials/demystifying-es6-classes-and-prototypal-inheritance)
 * 📜 [Intro To Prototypal Inheritance — Dharani Jayakanthan](https://dev.to/danny/intro-to-prototypal-inheritance---js-9di)
 * 📜 [Classes in JavaScript - Explained — Daniel Li](http://blog.brew.com.hk/classes-in-javascript-explained/)
 * 📜 [You Don't Know JS: this & Object Prototypes — Kyle Simpson](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20%26%20object%20prototypes/ch4.md)

 ### Vídeos

 * 🎥 [Javascript Prototype Inheritance — Avelx](https://www.youtube.com/watch?v=sOrtAjyk4lQ)
 * 🎥 [JavaScript Prototype Inheritance Explained pt. I — techsith](https://www.youtube.com/watch?v=7oNWNlMrkpc)
 * 🎥 [JavaScript Prototype Inheritance Explained pt. II — techsith](https://www.youtube.com/watch?v=uIlj6_z_wL8)
 * 🎥 [JavaScript Prototype Inheritance Explained — Kyle Robinson](https://www.youtube.com/watch?v=qMO-LTOrJaE)
 * 🎥 [Advanced Javascript - Prototypal Inheritance In 1 Minute](https://www.youtube.com/watch?v=G6l5CHl67HQ)
 * 🎥 [An Overview Of Classical Javascript Classes and Prototypal Inheritance — Pentacode](https://www.youtube.com/watch?v=phwzuiJJPpQ)
 * 🎥 [Object Oriented JavaScript - Prototype — The Net Ninja](https://www.youtube.com/watch?v=4jb4AYEyhRc)
 * 🎥 [Prototype in JavaScript — kudvenkat](https://www.youtube.com/watch?v=2rkEbcptR64)
 * 🎥 [JavaScript Using Prototypes — O'Reilly](https://www.youtube.com/watch?v=oCwCcNvaXAQ)
 * 🎥 [A Beginner's Guide to Javascript's Prototype — Tyler Mcginnis](https://www.youtube.com/watch?v=XskMWBXNbp0)


**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 18. Object.create e Object.assign

### Artigos (inglês)

 * 📜 [Object.create() — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/create)
 * 📜 [Object.create in JavaScript — Rupesh Mishra](https://hackernoon.com/object-create-in-javascript-fa8674df6ed2)
 * 📜 [Object.create(): the New Way to Create Objects in JavaScript — Rob Gravelle](https://www.htmlgoodies.com/beyond/javascript/object.create-the-new-way-to-create-objects-in-javascript.html)
 * 📜 [Basic Inheritance with Object.create — Joshua Clanton](http://adripofjavascript.com/blog/drips/basic-inheritance-with-object-create.html)
 * 📜 [Object.create() In JavaScript — GeeksforGeeks](https://www.geeksforgeeks.org/object-create-javascript/)
 * 📜 [Understanding the difference between Object.create() and the new operator — Jonathan Voxland](https://medium.com/@jonathanvox01/understanding-the-difference-between-object-create-and-the-new-operator-b2a2f4749358)
 * 📜 [JavaScript Object Creation: Patterns and Best Practices — Jeff Mott](https://www.sitepoint.com/javascript-object-creation-patterns-best-practises/)
 * 📜 [Dealing With Objects in JavaScript With Object.assign, Object.keys and hasOwnProperty](https://alligator.io/js/dealing-with-objects/)
 * 📜 [Copying Objects in JavaScript ― Orinami Olatunji](https://scotch.io/bar-talk/copying-objects-in-javascript)
 * 📜 [Object.assign() — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
 * 📜 [JavaScript: Object.assign() — Thiago S. Adriano](https://codeburst.io/javascript-object-assign-bc9696dcbb6e)

 ### Vídeos

 * 🎥 [Object.assign() explained — Aaron Writes Code](https://www.youtube.com/watch?v=aw7NfYhR5rc)
 * 🎥 [Object.assign() Method — techsith](https://www.youtube.com/watch?v=9Ky4X6inpi4)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 19. map, reduce, filter

### Artigos (português)

 * 📜 [map(), filter() e reduce() em JavaScript — Tárcio Zemel](http://desenvolvimentoparaweb.com/javascript/map-filter-reduce-javascript/)
 * 📜 [JavaScript: Conhecendo map(), filter() e reduce() — Thiago S. Adriano](https://medium.com/@programadriano/javascript-conhecendo-map-filter-e-reduce-ce072d8f0ec5)

### Artigos (inglês)

 * 📜 [JavaScript Functional Programming — map, filter and reduce — Bojan Gvozderac](https://medium.com/jsguru/javascript-functional-programming-map-filter-and-reduce-846ff9ba492d)
 * 📜 [Learn map, filter and reduce in Javascript — João Miguel Cunha](https://medium.com/@joomiguelcunha/learn-map-filter-and-reduce-in-javascript-ea59009593c4)
 * 📜 [JavaScript’s Map, Reduce, and Filter — Dan Martensen](https://danmartensen.svbtle.com/javascripts-map-reduce-and-filter)
 * 📜 [How to Use Map, Filter, & Reduce in JavaScript — Peleke Sengstacke](https://code.tutsplus.com/tutorials/how-to-use-map-filter-reduce-in-javascript--cms-26209)
 * 📜 [JavaScript — Learn to Chain Map, Filter, and Reduce — Brandon Morelli](https://codeburst.io/javascript-learn-to-chain-map-filter-and-reduce-acd2d0562cd4)
 * 📜 [Javascript data structure with map, reduce, filter and ES6 — Deepak Gupta](https://codeburst.io/write-beautiful-javascript-with-%CE%BB-fp-es6-350cd64ab5bf)
 * 📜 [Understanding map, filter and reduce in Javascript — Luuk Gruijs](https://hackernoon.com/understanding-map-filter-and-reduce-in-javascript-5df1c7eee464)
 * 📜 [Functional Programming in JS: map, filter, reduce (Pt. 5) — Omer Goldberg](https://hackernoon.com/functional-programming-in-js-map-filter-reduce-pt-5-308a205fdd5f)
 * 📜 [JavaScript: Map, Filter, Reduce — William S. Vincent](https://wsvincent.com/functional-javascript-map-filter-reduce/)
 * 📜 [Arrow Functions: Fat and Concise Syntax in JavaScript — Kyle Pennell](https://www.sitepoint.com/es6-arrow-functions-new-fat-concise-syntax-javascript/)
 * 📜 [JavaScript: Arrow Functions for Beginners — Brandon Morelli](https://codeburst.io/javascript-arrow-functions-for-beginners-926947fc0cdc)
 * 📜 [When (and why) you should use ES6 arrow functions — and when you shouldn’t — Cynthia Lee](https://medium.freecodecamp.org/when-and-why-you-should-use-es6-arrow-functions-and-when-you-shouldnt-3d851d7f0b26)
 * 📜 [JavaScript — Learn & Understand Arrow Functions — Brandon Morelli](https://codeburst.io/javascript-learn-understand-arrow-functions-fe2083533946)
 * 📜 [(JavaScript )=> Arrow functions — sigu](https://medium.com/podiihq/javascript-arrow-functions-27d4c3334b83)
 * 📜 [A possibility to use Async/Await for filter(), find(), forEach(), map() and reduce() methods in Array - Ruwan Geeganage](https://www.linkedin.com/pulse/possibility-use-asyncawait-filter-find-foreach-map-reduce-geeganage/)

 ### Vídeos

 * 🎥 [Map, Filter and Reduce — Lydia Hallie](https://www.youtube.com/watch?v=UXiYii0Y7Nw)
 * 🎥 [Functional JavaScript: Map, forEach, Reduce, Filter — Theodore Anderson](https://www.youtube.com/watch?v=vytzLlY_wmU)
 * 🎥 [JavaScript Array superpowers: Map, Filter, Reduce (part I) — Michael Rosata](https://www.youtube.com/watch?v=qTeeVd8hOFY)
 * 🎥 [JavaScript Array superpowers: Map, Filter, Reduce (part 2) — Michael Rosata](https://www.youtube.com/watch?v=gIm9xLYudL0)
 * 🎥 [JavaScript Higher Order Functions - Filter, Map, Sort & Reduce — Epicop](https://www.youtube.com/watch?v=zYBeEPxNSbw)
 * 🎥 [[Array Methods 2/3] .filter + .map + .reduce — CodeWithNick](https://www.youtube.com/watch?v=4qWlqD0yYTU)
 * 🎥 [Arrow functions in JavaScript - What, Why and How — Fun Fun Function](https://www.youtube.com/watch?v=6sQDTgOqh-I)


**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 20. Pure Functions, Side Effects e State Mutation

### Artigos (inglês)

 * 📜 [Javascript and Functional Programming — Pure Functions — Omer Goldberg](https://hackernoon.com/javascript-and-functional-programming-pt-3-pure-functions-d572bb52e21c)
 * 📜 [Master the JavaScript Interview: What is a Pure Function? — Eric Elliott](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976)
 * 📜 [JavaScript: What Are Pure Functions And Why Use Them? — James Jeffery](https://medium.com/@jamesjefferyuk/javascript-what-are-pure-functions-4d4d5392d49c)
 * 📜 [Pure functions in JavaScript — @nicoespeon](http://www.nicoespeon.com/en/2015/01/pure-functions-javascript/)
 * 📜 [Functional Programming: Pure Functions — Arne Brasseur](https://www.sitepoint.com/functional-programming-pure-functions/)
 * 📜 [Pure Functions In Javascript — Krunal](https://appdividend.com/2017/04/10/pure-functions-in-javascript/)
 * 📜 [Making your JavaScript Pure — Jack Franklin](https://alistapart.com/article/making-your-javascript-pure)
 * 📜 [To mutate, or not to mutate, in JavaScript](https://slemgrim.com/mutate-or-not-to-mutate/)
 * 📜 [Arrays, Objects and Mutations — Federico Knüssel](https://medium.com/@fknussel/arrays-objects-and-mutations-6b23348b54aa)
 * 📜 [The State of Immutability — Maciej Sikora](https://medium.com/dailyjs/the-state-of-immutability-169d2cd11310)
 * 📜 [How to deal with dirty side effects in your pure functional JavaScript — James Sinclair](https://jrsinclair.com/articles/2018/how-to-deal-with-dirty-side-effects-in-your-pure-functional-javascript/)
 * 📜 [Preventing Side Effects in JavaScript — David Walsh](https://davidwalsh.name/preventing-sideeffects-javascript)

 ### Vídeos

 * 🎥 [Pure Functions — Hexlet](https://www.youtube.com/watch?v=dZ41D6LDSBg)
 * 🎥 [Pure Functions - Functional Programming in JavaScript — Paul McBride](https://www.youtube.com/watch?v=Jh_Uzqzz_wM)
 * 🎥 [JavaScript Pure Functions — Seth Alexander](https://www.youtube.com/watch?v=frT3H-eBmPc)


**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 21. Closures

### Artigos (inglês)

 * 📜 [Closures — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)
 * 📜 [I never understood JavaScript closures — Olivier De Meulder](https://medium.com/dailyjs/i-never-understood-javascript-closures-9663703368e8)
 * 📜 [Closure — JavaScript.Info](https://javascript.info/closure)
 * 📜 [Understand JavaScript Closures With Ease — Richard Bovell](http://javascriptissexy.com/understand-javascript-closures-with-ease/)
 * 📜 [Understanding JavaScript Closures — Codesmith](https://codeburst.io/understanding-javascript-closures-da6aab330302)
 * 📜 [Understand Closures in JavaScript — Brandon Morelli](https://codeburst.io/understand-closures-in-javascript-d07852fa51e7)
 * 📜 [A simple guide to help you understand closures in JavaScript — Prashant Ram](https://medium.freecodecamp.org/javascript-closures-simplified-d0d23fa06ba4)
 * 📜 [Understanding JavaScript Closures: A Practical Approach — Paul Upendo](https://scotch.io/tutorials/understanding-javascript-closures-a-practical-approach)
 * 📜 [Understanding JavaScript: Closures — Alexander Kondov](https://hackernoon.com/understanding-javascript-closures-4188edf5ea1b)
 * 📜 [How to use JavaScript closures with confidence — Léna Faure](https://hackernoon.com/how-to-use-javascript-closures-with-confidence-85cd1f841a6b)
 * 📜 [JavaScript closures by example — tyler](https://howchoo.com/g/mge2mji2mtq/javascript-closures-by-example)

 ### Vídeos

 * 🎥 [Javascript Closure — techsith](https://www.youtube.com/watch?v=71AtaJpJHw0)
 * 🎥 [Closures — Fun Fun Function](https://www.youtube.com/watch?v=CQqwU2Ixu-U)
 * 🎥 [Closures in JavaScript — techsith](https://www.youtube.com/watch?v=-xqJo5VRP4A)
 * 🎥 [JavaScript Closures 101: What is a closure? — JavaScript Tutorials](https://www.youtube.com/watch?v=yiEeiMN2Khs)
 * 🎥 [Closures — freeCodeCamp](https://www.youtube.com/watch?v=1JsJx1x35c0)
 * 🎥 [JavaScript Closures — CodeWorkr](https://www.youtube.com/watch?v=-rLrGAXK8WE)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 22. Funções de alta ordem

### Artigos (inglês)

 * 📜 [Higher-Order Functions — Eloquent JavaScript [Book]](https://eloquentjavascript.net/05_higher_order.html)
 * 📜 [Higher-Order Functions in JavaScript — M. David Green](https://www.sitepoint.com/higher-order-functions-javascript/)
 * 📜 [Higher Order Functions: Using Filter, Map and Reduce for More Maintainable Code — Guido Schmitz](https://medium.freecodecamp.org/higher-order-functions-in-javascript-d9101f9cf528)
 * 📜 [First-class and Higher Order Functions: Effective Functional JavaScript — Hugo Di Francesco](https://hackernoon.com/effective-functional-javascript-first-class-and-higher-order-functions-713fde8df50a)
 * 📜 [Higher Order Functions in JavaScript — John Hannah](https://www.lullabot.com/articles/higher-order-functions-in-javascript)
 * 📜 [Higher-order Functions — Richard Bovell](http://javascriptissexy.com/tag/higher-order-functions/)
 * 📜 [Higher Order Functions in JavaScript — Zsolt Nagy](http://www.zsoltnagy.eu/higher-order-functions-in-javascript/)
 * 📜 [Fun With Higher Order Functions In JavaScript — Derick](https://derickbailey.com/2015/10/21/fun-with-higher-order-functions-in-javascript/)
 * 📜 [Just a reminder on how to use high order functions — Pedro Filho](https://github.com/pedroapfilho/high-order-functions)
 * 📜 [How to use JavaScript closures with confidence — Léna Faure](https://hackernoon.com/how-to-use-javascript-closures-with-confidence-85cd1f841a6b)
 * 📜 [JavaScript closures by example — tyler](https://howchoo.com/g/mge2mji2mtq/javascript-closures-by-example)

 ### Vídeos

 * 🎥 [JavaScript Higher Order Functions & Arrays — Traversy Media](https://www.youtube.com/watch?v=rRgD1yVwIvE)
 * 🎥 [Higher Order Functions — Fun Fun Function](https://www.youtube.com/watch?v=BMUiFMZr7vk)
 * 🎥 [Higher Order Functions in Javascript — Raja Yogan](https://www.youtube.com/watch?v=dTlpYnmBW9I)
 * 🎥 [Higher Order Iterators in JavaScript — Fun Fun Function](https://www.youtube.com/watch?v=GYRMNp1SKXA)
 * 🎥 [Higher Order Functions in JavaScript — The Coding Train](https://www.youtube.com/watch?v=H4awPsyugS0)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 23. Recursão

### Artigos (inglês)

 * 📜 [Recursion in JavaScript — Kevin Ennis](https://medium.freecodecamp.org/recursion-in-javascript-1608032c7a1f)
 * 📜 [Understanding Recursion in JavaScript — Zak Frisch](https://medium.com/@zfrisch/understanding-recursion-in-javascript-992e96449e03)
 * 📜 [Learn and Understand Recursion in JavaScript — Brandon Morelli](https://codeburst.io/learn-and-understand-recursion-in-javascript-b588218e87ea)
 * 📜 [Recursion in Functional JavaScript — M. David Green](https://www.sitepoint.com/recursion-functional-javascript/)
 * 📜 [Programming with JS: Recursion — Alexander Kondov](https://hackernoon.com/programming-with-js-recursion-31371e2bf808)
 * 📜 [Anonymous Recursion in JavaScript — simo](https://dev.to/simov/anonymous-recursion-in-javascript)
 * 📜 [Recursion, iteration and tail calls in JS — loverajoel](http://www.jstips.co/en/javascript/recursion-iteration-and-tail-calls-in-js/)
 * 📜 [Understanding Recursion in JavaScript with Confidence — Jay](https://www.thecodingdelight.com/understanding-recursion-javascript/)

 ### Vídeos

 * 🎥 [Recursion In JavaScript — techsith](https://www.youtube.com/watch?v=VtG0WAUvq2w)
 * 🎥 [Recursion — Fun Fun Function](https://www.youtube.com/watch?v=k7-N8R0-KY4)
 * 🎥 [Recursion and Recursive Functions — Hexlet](https://www.youtube.com/watch?v=vLhHyGTkjCs)
 * 🎥 [Recursion: Recursion() - JS Monthly — Lucas da Costa](https://www.youtube.com/watch?v=kGXVsd8pBLw)
 * 🎥 [Recursive Function in JavaScript — kudvenkat](https://www.youtube.com/watch?v=uyjsR9eNTIw)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 24. Collections

### Artigos (inglês)

 * 📜 [ES6 In Depth: Collections — Jason Orendorff](https://hacks.mozilla.org/2015/06/es6-in-depth-collections/)
 * 📜 [ES6 Collections: Using Map, Set, WeakMap, WeakSet — Kyle Pennell](https://www.sitepoint.com/es6-collections-map-set-weakmap-weakset/)
 * 📜 [ES6 WeakMaps, Sets, and WeakSets in Depth — Nicolás Bevacqua](https://ponyfoo.com/articles/es6-weakmaps-sets-and-weaksets-in-depth)
 * 📜 [Introduction to Sets in JavaScript — Alligator.io](https://alligator.io/js/sets-introduction/)
 * 📜 [Introduction to Maps in JavaScript — Alligator.io](https://alligator.io/js/maps-introduction/)
 * 📜 [Map, Set, WeakMap and WeakSet — JavaScript.Info](https://javascript.info/map-set-weakmap-weakset)
 * 📜 [Maps in ES6 - A Quick Guide — Ben Mildren](https://dev.to/mildrenben/maps-in-es6---a-quick-guide-35pk)
 * 📜 [ES6 — Set vs Array — What and when? — Maya Shavin](https://medium.com/front-end-hacking/es6-set-vs-array-what-and-when-efc055655e1a)
 * 📜 [ES6 — Map vs Object — What and when? — Maya Shavin](https://medium.com/front-end-hacking/es6-map-vs-object-what-and-when-b80621932373)
 * 📜 [ES6: Working with Sets in JavaScript — Dead Code Rising](http://www.deadcoderising.com/es6-working-with-sets-in-javascript/)
 * 📜 [Array vs Set vs Map vs Object — Real-time use cases in Javascript (ES6/ES7) — Rajesh Babu](https://codeburst.io/array-vs-set-vs-map-vs-object-real-time-use-cases-in-javascript-es6-47ee3295329b)
 * 📜 [How to create an array of unique values in JavaScript using Sets — Claire Parker-Jones](https://dev.to/claireparker/how-to-create-an-array-of-unique-values-in-javascript-using-sets-5dg6)
 * 📜 [What You Should Know About ES6 Maps — Just Chris](https://hackernoon.com/what-you-should-know-about-es6-maps-dc66af6b9a1e)
 * 📜 [ES6 Maps in Depth — Nicolás Bevacqua](https://ponyfoo.com/articles/es6-maps-in-depth)


 ### Vídeos

 * 🎥 [JavaScript ES6 / ES2015 Set, Map, WeakSet and WeakMap — Traversy Media](https://www.youtube.com/watch?v=ycohYSx5h9w)
 * 🎥 [The Differences between ES6 Maps and Sets — Steve Griffith](https://www.youtube.com/watch?v=m4abICrldQI)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 25. Promises

### Artigos (inglês)

 * 📜 [Promise — MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
 * 📜 [JavaScript Promises for Dummies ― Jecelyn Yeen](https://scotch.io/tutorials/javascript-promises-for-dummies)
 * 📜 [Understanding promises in JavaScript — Gokul N K](https://hackernoon.com/understanding-promises-in-javascript-13d99df067c1)
 * 📜 [Master the JavaScript Interview: What is a Promise? — Eric Elliott](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e77261)
 * 📜 [An Overview of JavaScript Promises — Sandeep Panda](https://www.sitepoint.com/overview-javascript-promises/)
 * 📜 [How to use Promises in JavaScript — Prashant Ram](https://medium.freecodecamp.org/promises-in-javascript-explained-277b98850de)
 * 📜 [Implementing Promises In JavaScript — Maciej Cieslar](https://medium.freecodecamp.org/how-to-implement-promises-in-javascript-1ce2680a7f51)
 * 📜 [JavaScript: Promises explained with simple real life analogies — Shruti Kapoor](https://codeburst.io/javascript-promises-explained-with-simple-real-life-analogies-dd6908092138)
 * 📜 [Promises for Asynchronous Programming — Exploring JS](http://exploringjs.com/es6/ch_promises.html)
 * 📜 [JavaScript Promises Explained By Gambling At A Casino — Kevin Kononenko](https://blog.codeanalogies.com/2018/08/26/javascript-promises-explained-by-gambling-at-a-casino/)
 * 📜 [ES6 Promises: Patterns and Anti-Patterns — Bobby Brennan](https://medium.com/datafire-io/es6-promises-patterns-and-anti-patterns-bbb21a5d0918)
 * 📜 [A Simple Guide to ES6 Promises — Brandon Morelli](https://codeburst.io/a-simple-guide-to-es6-promises-d71bacd2e13a)
 * 📜 [The ES6 Promises — Manoj Singh Negi](https://codeburst.io/the-es6-promises-87a979ab27e4)
 * 📜 [ES6 Promises in Depth — Nicolás Bevacqua](https://ponyfoo.com/articles/es6-promises-in-depth)

 ### Vídeos

 * 🎥 [Let's Learn ES6 - Promises — Ryan Christiani](https://www.youtube.com/watch?v=vQ3MoXnKfuQ)
 * 🎥 [JavaScript ES6 / ES2015 Promises — Traversy Media](https://www.youtube.com/watch?v=XJEHuBZQ5dU)
 * 🎥 [Promises — Fun Fun Function](https://www.youtube.com/watch?v=2d7s3spWAzo)
 * 🎥 [Error Handling Promises in JavaScript — Fun Fun Function](https://www.youtube.com/watch?v=f8IgdnYIwOU)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 26. async/await

### Artigos (português)

 * 📜 [Entendendo o async e o await em JavaScript — Wendell Adriel](https://tableless.com.br/entendendo-o-async-e-o-await-em-javascript/)
 * 📜 [Async Await, JS assincronamente síncrono — FELIPE N. MOURA](https://braziljs.org/blog/async-await-js-assincronamente-sincrono/)

### Artigos (inglês)

 * 📜 [async/await — JavaScript.Info](https://javascript.info/async-await)
 * 📜 [Understanding async/await in Javascript — Gokul N K](https://hackernoon.com/understanding-async-await-in-javascript-1d81bb079b2c)
 * 📜 [Asynchronous Programming — Eloquent JavaScript](https://eloquentjavascript.net/11_async.html)
 * 📜 [Exploring Async/Await Functions in JavaScript — Alligator.io](https://alligator.io/js/async-functions/)
 * 📜 [Asynchronous Javascript using async/await — Joy Warugu](https://scotch.io/tutorials/asynchronous-javascript-using-async-await)
 * 📜 [Modern Asynchronous JavaScript with async/await — Flavio Copes](https://flaviocopes.com/javascript-async-await/)
 * 📜 [Asynchronous JavaScript: From Callback Hell to Async and Await — Demir Selmanovic](https://www.toptal.com/javascript/asynchronous-javascript-async-await-tutorial)
 * 📜 [Javascript — ES8 Introducing async/await Functions — Ben Garrison](https://medium.com/@_bengarrison/javascript-es8-introducing-async-await-functions-7a471ec7de8a)
 * 📜 [How to escape async/await hell — Aditya Agarwal](https://medium.freecodecamp.org/avoiding-the-async-await-hell-c77a0fb71c4c)
 * 📜 [Understanding JavaScript’s async await — Nicolás Bevacqua](https://ponyfoo.com/articles/understanding-javascript-async-await)
 * 📜 [JavaScript Async/Await: Serial, Parallel and Complex Flow — TechBrij](https://techbrij.com/javascript-async-await-parallel-sequence)
 * 📜 [Asynchronous Programming — Exploring JS](http://exploringjs.com/es6/ch_async.html)
 * 📜 [From JavaScript Promises to Async/Await: why bother? — Chris Nwamba](https://blog.pusher.com/promises-async-await/)
 * 📜 [Flow Control in Modern JS: Callbacks to Promises to Async/Await — Craig Buckler](https://www.sitepoint.com/flow-control-callbacks-promises-async-await/)
 * 📜 [JavaScript: Promises and Why Async/Await Wins the Battle — Nick Parsons](https://dzone.com/articles/javascript-promises-and-why-asyncawait-wins-the-ba)

 ### Vídeos

 * 🎥 [Async + Await — Wes Bos](https://www.youtube.com/watch?v=9YkUCxvaLEk)
 * 🎥 [Asynchrony: Under the Hood — Shelley Vohr](https://www.youtube.com/watch?v=SrNQS8J67zc)
 * 🎥 [async/await in JavaScript - What, Why and How — Fun Fun Function](https://www.youtube.com/watch?v=568g8hxJJp4&index=3&list=PL0zVEGEvSaeHJppaRLrqjeTPnCH6)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 27. Estrutura dos dados

### Artigos (inglês)

 * 📜 [Data Structures in JavaScript — Thon Ly](https://medium.com/siliconwat/data-structures-in-javascript-1b9aed0ea17c)
 * 📜 [Algorithms and Data Structures in JavaScript — Oleksii Trekhleb](https://itnext.io/algorithms-and-data-structures-in-javascript-a71548f902cb)
 * 📜 [Data Structures: Objects and Arrays ― Chris Nwamba](https://scotch.io/courses/10-need-to-know-javascript-concepts/data-structures-objects-and-arrays)
 * 📜 [Data structures in JavaScript — Benoit Vallon](http://blog.benoitvallon.com/data-structures-in-javascript/data-structures-in-javascript/)
 * 📜 [Playing with Data Structures in Javascript — Anish K.](https://blog.cloudboost.io/playing-with-data-structures-in-javascript-stack-a55ebe50f29d)
 * 📜 [The Little Guide of Queue in JavaScript — Germán Cutraro](https://hackernoon.com/the-little-guide-of-queue-in-javascript-4f67e79260d9)
 * 📜 [All algorithms writing with JavaScript in the book 'Algorithms Fourth Edition'](https://github.com/barretlee/algorithms)
 * 📜 [Collection of classic computer science paradigms in JavaScript](https://github.com/nzakas/computer-science-in-javascript)
 * 📜 [All the things you didn't know you wanted to know about data structures](https://github.com/jamiebuilds/itsy-bitsy-data-structures)

 ### Vídeos

 * 🎥 [Algorithms in JavaScript — Seth Koch](https://www.youtube.com/watch?v=PylQlISSH8U&list=PLujX4CIdBGCa-65N3uN8CDbUMrYsHBrz-)
 * 🎥 [Algorithms In Javascript | Ace Your Interview — Eduonix Learning Solutions](https://www.youtube.com/watch?v=H_EBPZgiAas&list=PLDmvslp_VR0zYUSth_8O69p4_cmvZEgLa)
 * 🎥 [Data Structures and Algorithms in JavaScript — freeCodeCamp](https://www.youtube.com/watch?v=Gj5qBheGOEo&list=PLWKjhJtqVAbkso-IbgiiP48n-O-JQA9PJ)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 28. Expensive Operation e Big O Notation

### Artigos (inglês)

 * 📜 [Big O Notation in Javascript — César Antón Dorantes](https://medium.com/cesars-tech-insights/big-o-notation-javascript-25c79f50b19b)
 * 📜 [Time Complexity/Big O Notation — Tim Roberts](https://medium.com/javascript-scene/time-complexity-big-o-notation-1a4310c3ee4b)
 * 📜 [Big O in JavaScript — Gabriela Medina](https://medium.com/@gmedina229/big-o-in-javascript-36ff67766051)
 * 📜 [Big O Search Algorithms in JavaScript — Bradley Braithwaite](http://www.bradoncode.com/blog/2012/04/big-o-algorithm-examples-in-javascript.html)
 * 📜 [Time Complexity Analysis in JavaScript — Jennifer Bland](https://www.jenniferbland.com/time-complexity-analysis-in-javascript/)
 * 📜 [Algorithms in plain English: time complexity and Big-O Notation — Michael Olorunnisola](https://medium.freecodecamp.org/time-is-complex-but-priceless-f0abd015063c)

### Vídeos

 * 🎥 [JavaScript: Intro to Big O Notation and Function Runtime — Eric Traub](https://www.youtube.com/watch?v=HgA5VOFan5E)
 * 🎥 [Essential Big O for JavaScript Developers — Dave Smith](https://www.youtube.com/watch?v=KatlvCFHPRo)
 * 🎥 [Big O Notation - Time Complexity Analysis — WebTunings](https://www.youtube.com/watch?v=ALl86xJiTD8)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 29. Algoritmos

### Artigos (inglês)

 * 📜 [Data Structures and Algorithms using ES6](https://github.com/Crizstian/data-structure-and-algorithms-with-ES6)
 * 📜 [Algorithms and data structures implemented in JavaScript with explanations and links to further readings](https://github.com/trekhleb/javascript-algorithms)
 * 📜 [JS: Interview Algorithm](http://www.thatjsdude.com/interview/js1.html)
 * 📜 [Algorithms in JavaScript — Thon Ly](https://medium.com/siliconwat/algorithms-in-javascript-b0bed68f4038)
 * 📜 [JavaScript Objects, Square Brackets and Algorithms — Dmitri Grabov](https://medium.freecodecamp.org/javascript-objects-square-brackets-and-algorithms-e9a2916dc158)
 * 📜 [Atwood's Law applied to CS101 - Classic algorithms and data structures implemented in JavaScript](https://github.com/felipernb/algorithms.js)
 * 📜 [Data Structures and Algorithms library in JavaScript](https://github.com/yangshun/lago)
 * 📜 [Collection of computer science algorithms and data structures written in JavaScript](https://github.com/idosela/algorithms-in-javascript)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 30. Herança, Polimorfismo e Reutilização de Código

### Artigos (inglês)

 * 📜 [Class inheritance, super — JavaScript.Info](https://javascript.info/class-inheritance)
 * 📜 [Inheritance in JavaScript — MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Inheritance)
 * 📜 [Inheritance in JavaScript — Rupesh Mishra](https://hackernoon.com/inheritance-in-javascript-21d2b82ffa6f)
 * 📜 [Simple Inheritance with JavaScript — David Catuhe](https://www.sitepoint.com/simple-inheritance-javascript/)
 * 📜 [JavaScript — Inheritance, delegation patterns and Object linking — NC Patro](https://codeburst.io/javascript-inheritance-25fe61ab9f85)
 * 📜 [Object Oriented JavaScript: Polymorphism with examples — Knoldus Blogs](https://blog.knoldus.com/object-oriented-javascript-polymorphism-with-examples/)
 * 📜 [Program Like Proteus — A beginner’s guide to polymorphism in Javascript — Sam Galson](https://medium.com/yld-engineering-blog/program-like-proteus-a-beginners-guide-to-polymorphism-in-javascript-867bea7c8be2)
 * 📜 [Object-oriented JavaScript: A Deep Dive into ES6 Classes — Jeff Mott](https://www.sitepoint.com/object-oriented-javascript-deep-dive-es6-classes/)

  ### Vídeos

 * 🎥 [Inheritance in JavaScript — kudvenkat](https://www.youtube.com/watch?v=yXlFR81tDBM)
 * 🎥 [JavaScript ES6 Classes and Inheritance — Traversy Media](https://www.youtube.com/watch?v=RBLIm5LMrmc)
 * 🎥 [Polymorphism in JavaScript — kudvenkat](https://www.youtube.com/watch?v=zdovG9cuEBA)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 31. Padrões de design

### Artigos (inglês)

 * 📜 [4 JavaScript Design Patterns You Should Know — Devan Patel](https://scotch.io/bar-talk/4-javascript-design-patterns-you-should-know)
 * 📜 [JavaScript Design Patterns – Beginner's Guide to Mobile Web Development — Soumyajit Pathak](https://medium.com/beginners-guide-to-mobile-web-development/javascript-design-patterns-25f0faaaa15)
 * 📜 [JavaScript Design Patterns — Akash Pal](https://medium.com/front-end-hacking/javascript-design-patterns-ed9d4c144c81)
 * 📜 [Javascript Design Patterns: What They Are & How To Use Them — Patrick Simpson](https://seesparkbox.com/foundry/javascript_design_patterns)
 * 📜 [All the 23 (GoF) design patterns implemented in Javascript — Felipe Beline](https://github.com/fbeline/Design-Patterns-JS)
 * 📜 [Learning JavaScript Design Patterns — Addy Osmani ](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)

  ### Vídeos

 * 🎥 [JavaScript Design Patterns — Udacity](https://www.udacity.com/course/javascript-design-patterns--ud989)

 **[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 32. Aplicações parciais, Currying, Compose e Pipe

### Artigos (inglês)

 * 📜 [Use function composition in JavaScript — Rémi](https://www.codementor.io/michelre/use-function-composition-in-javascript-gkmxos5mj)
 * 📜 [Currying in JavaScript ES6 — Adam Bene](https://blog.benestudio.co/currying-in-javascript-es6-540d2ad09400)
 * 📜 [Composition and Currying Elegance in JavaScript — Pragyan Das](https://medium.com/@pragyan88/writing-middleware-composition-and-currying-elegance-in-javascript-8b15c98a541b)
 * 📜 [Functional JavaScript: Function Composition For Every Day Use — Joel Thoms](https://hackernoon.com/javascript-functional-composition-for-every-day-use-22421ef65a10)
 * 📜 [Functional Composition: compose() and pipe() — Anton Paras](https://medium.com/@acparas/what-i-learned-today-july-2-2017-ab9a46dbf85f)
 * 📜 [Why The Hipsters Compose Everything: Functional Composing In JavaScript — A. Sharif](http://busypeoples.github.io/post/functional-composing-javascript/)
 * 📜 [A Gentle Introduction to Functional JavaScript pt III: Functions for making functions — James Sinclair](https://jrsinclair.com/articles/2016/gentle-introduction-to-functional-javascript-functions/)
 * 📜 [Curry And Compose (why you should be using something like ramda in your code) — jsanchesleao](https://jsleao.wordpress.com/2015/02/22/curry-and-compose-why-you-should-be-using-something-like-ramda-in-your-code/)
 * 📜 [Function Composition in JavaScript with Pipe — Andy Van Slaars](https://vanslaars.io/post/create-pipe-function/)
 * 📜 [Practical Functional JavaScript with Ramda — Andrew D'Amelio, Yuri Takhteyev](https://developer.telerik.com/featured/practical-functional-javascript-ramda/)
 * 📜 [The beauty in Partial Application, Currying, and Function Composition — Joel Thoms](https://hackernoon.com/the-beauty-in-partial-application-currying-and-function-composition-d885bdf0d574)
 * 📜 [Curry or Partial Application? — Eric Elliott](https://medium.com/javascript-scene/curry-or-partial-application-8150044c78b8)
 * 📜 [Partial Application in JavaScript — Ben Alman](http://benalman.com/news/2012/09/partial-application-in-javascript/)
 * 📜 [Partial Application of Functions — Functional Reactive Ninja](https://hackernoon.com/partial-application-of-functions-dbe7d9b80760)
 * 📜 [Currying vs Partial Application — Deepak Gupta](https://codeburst.io/javascript-currying-vs-partial-application-4db5b2442be8)
 * 📜 [Partial Application in ECMAScript 2015 — Ragan Wald](http://raganwald.com/2015/04/01/partial-application.html)
 * 📜 [Functional Composition in Javascript — Joe Cortopassi](https://joecortopassi.com/articles/functional-composition-in-javascript/)
 * 📜 [So You Want to be a Functional Programmer pt. I — Charles Scalfani](https://medium.com/@cscalfani/so-you-want-to-be-a-functional-programmer-part-1-1f15e387e536)
 * 📜 [So You Want to be a Functional Programmer pt. II — Charles Scalfani](https://medium.com/@cscalfani/so-you-want-to-be-a-functional-programmer-part-2-7005682cec4a)
 * 📜 [So You Want to be a Functional Programmer pt. III — Charles Scalfani](https://medium.com/@cscalfani/so-you-want-to-be-a-functional-programmer-part-3-1b0fd14eb1a7)
 * 📜 [So You Want to be a Functional Programmer pt. IV — Charles Scalfani](https://medium.com/@cscalfani/so-you-want-to-be-a-functional-programmer-part-4-18fbe3ea9e49)
 * 📜 [So You Want to be a Functional Programmer pt. V — Charles Scalfani](https://medium.com/@cscalfani/so-you-want-to-be-a-functional-programmer-part-5-c70adc9cf56a)
 * 📜 [Functional-Light JavaScript Chapter 3: Managing Function Inputs — Kyle Simpson](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch3.md)

  ### Vídeos

 * 🎥 [Compose vs Pipe: Functional Programming in JavaScript — Chyld Studios](https://www.youtube.com/watch?v=Wl2ejJOqHUU)
 * 🎥 [JavaScript Functional Programing: Compose — Theodore Anderson](https://www.youtube.com/watch?v=jigHxo9YR30)
 * 🎥 [Function Composition - Functional JavaScript — NWCalvank](https://www.youtube.com/watch?v=mth5WpEc4Qs)
 * 🎥 [JavaScript Function Composition Explained — Theodore Anderson](https://www.youtube.com/watch?v=Uam37AlzPYw)
 * 🎥 [Let's code with function composition — Fun Fun Function](https://www.youtube.com/watch?v=VGB9HbL1GHk)
 * 🎥 [Partial Application vs. Currying — NWCalvank](https://www.youtube.com/watch?v=DzLkRsUN2vE)
 * 🎥 [JavaScript Partial Application — Theodore Anderson](https://www.youtube.com/watch?v=jkebgHEcvac)

**[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---

## 33. Código limpo (clean)

### Artigos (inglês)

 * 📜 [Clean Code concepts adapted for JavaScript — Ryan McDermott](https://github.com/ryanmcdermott/clean-code-javascript)
 * 📜 [JavaScript Clean Coding Best Practices — András Tóth](https://blog.risingstack.com/javascript-clean-coding-best-practices-node-js-at-scale/)
 * 📜 [Function parameters in JavaScript Clean Code — Kevin Peters](https://medium.com/@kevin_peters/function-parameters-in-javascript-clean-code-4caac109159b)
 * 📜 [Clean Code JavaScript — Sarah Drasner](https://css-tricks.com/clean-code-javascript/)
 * 📜 [Keeping your code clean — Samuel James](https://codeburst.io/keeping-your-code-clean-d30bcffd1a10)
 * 📜 [Best Practices for Using Modern JavaScript Syntax — M. David Green](https://www.sitepoint.com/modern-javascript-best-practices/)
 
 ### Artigos (português)
 
* 📜 [Conceitos de Código Limpo adaptados em JavaScript - Felipe Augusto](https://github.com/felipe-augusto/clean-code-javascript)

 **[⬆ Voltar ao topo](#tabela-de-conteúdos)**

---
 -->
