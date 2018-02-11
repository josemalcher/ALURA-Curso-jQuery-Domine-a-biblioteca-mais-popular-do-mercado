# Curso jQuery: Domine a biblioteca mais popular do mercado - Alura

https://josemalcher.net/kanban/public/task/242/c1b8680b9e2b4305daf46fb0f202491ea8b958010a14999aebf4e6238976



---

## <a name="indice">Índice</a>

- [1.Introdução ao jQuery, suas vantagens e a função seletora](#parte1)   
- [2.Escutando eventos com jQuery](#parte2)   
- [3.Criando o GameOver com eventos](#parte3)   
- [4.Reiniciando nosso jogo](#parte4)   
- [5.Funções que auxiliam os estilos](#parte5)   
- [6.Criando e manipulando elementos com jQuery](#parte6)   


---

## <a name="parte1">1.Introdução ao jQuery, suas vantagens e a função seletora</a>

### Introdução ao jQuery

Para ampliar as possibilidades de interação de nossos usuários com nossas páginas, recorremos a recursos avançados do CSS3, inclusive do HTML5, mas que muitas vezes não são suficientes. Este é o caso de quando queremos, por exemplo, copiar a informação digitada pelo usuário em outro elemento de nossa página, ou até mesmo fazer uma validação antes de enviar um formulário. Para atender casos como este, e outros ainda mais complexos, programamos em JavaScript, uma linguagem dinâmica compreendida pelo navegador.
Mas nos dias de hoje, sabemos que nossas páginas são acessadas por usuários de diversos dispositivos diferentes, passando pelo usuário comum de desktop até mesmo a um usuário que possuí um celular rodando um sistema operacional antigo. Esta variedade de dispositivos traz também uma variedade de navegadores.

![javascript nos navegadores](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/sem_jquery_navegadores1.png?raw=true)

Esta variedade que tornou o desenvolvimento do Javascript algo mais complexo, já que existem pequenas diferenças no modo com que o JavaScript funciona em cada navegador, fazendo com que um código que é completamente funcional em um determinado navegador, deixe de funcionar em outro.

![versões javascript nos navegadores](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/sem_jquery_navegadores.png?raw=true)


### Para o resgate: o framework jQuery

Neste cenário, que devemos garantir que nosso código JavaScript rode nos mais diversos navegadores, que entra o famoso framework jQuery. O jQuery é uma biblioteca que possuí várias funções de uso bastante comum no dia a dia do desenvolvedor JavaScript. O jQuery nos garante que suas funções irão funcionar nos mais diversos browsers, nos poupando de nos preocuparmos se o nosso código JavaScript irá funcionar em determinado navegador.
Ele age como um "tradutor", no sentido mais amplo da palavra, tornando um código JavaScript que era incompatível com certos navegadores em um código JavaScript funcional na grande parte deles:

![jquery](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/com_jquery.png?raw=true)

### Vantagens do jQuery

Além da grande vantagem de compatibilidade entre navegadores que o jQuery traz quando utilizamos suas funções, ele também tem um outro grande benefício, que ele deixa claro no seu logo.

Write less, Do more. Ou em português: escreva menos, faça mais. A segunda grande vantagem de utilizar o jQuery em seus projetos é o ganho de produtividade do desenvolvedor. Graças às suas funções sucintas, quando utilizamos o jQuery podemos reduzir muito o tamanho dos nossos códigos JavaScript, como podemos ver no seguinte exemplo:

![codigo javascript](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/codigo_sem_jquery_1.png?raw=true)

Este pedaço de código JavaScrit seleciona todos os parágrafos da página, itera por eles, e troca seu texto para "novo texto". Utilizando o jQuery, conseguimos realizar a mesma funcionalidade com muito menos código, veja:

![codigo com jquery](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/codigo_com_jquery_1.png?raw=true)

Como diz o lema do jQuery, conseguimos escrever muito menos quando estamos utilizando-o.
Um exemplo que combina tanto a vantagem da compatibilidade com a da produtividade é o seguinte:

![codigo javascript](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/codigo_sem_jquery_2.png?raw=true)

Neste código, temos de escrever bastante JavaScript para que o nosso evento de click seja detectado tanto nos Internet Explorer's antigos quantos nos browsers atuais, por isso ele faz a verificação com o if do começo. Este mesmo código, utilizando do jQuery ficaria assim:

![codigo jquery](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/codigo_com_jquery_2.png?raw=true)

Reduziu-se muito a quantidade de código escrito e manteve-se a compatibilidade com os mais diversos navegadores!

O grande foco deste treinamento é te ensinar a trabalhar com as mais diversas funções da biblioteca do jQuery, tornando-o um desenvolvedor mais ágil e mais bem preparado em como lidar com as diversas diferenças dos navegadores.


### Colocando o jQuery no projeto

Versões do jQuery

Agora que já entendemos as vantagens do jQuery e por que ele é um framework tão famoso, vamos discutir um pouco sobre as suas versões.
Para utilizar o jQuery em nosso projeto, primeiro precisamos baixá-lo. O jQuery pode ser baixado em seu site oficial, o jquery.com. 

Ao acessar esta página, nos encontraremos com uma grande quantidade links, cada um correspondendo a uma versão diferente do jQuery. 

O jQuery lançou recentemente sua nova versão, a versão 3, que trouxe mais rapidez em suas funções e reduziu o seu tamanho. Além destas melhorias, ele também trouxe uma nova versão do jQuery, a slim version, que hoje é disponibilizada como alternativa à versão tradicional do jQuery.

Esta versão slim, como a própria tradução indica, é uma versão mais magra do jQuery, mais leve. Ela não possuí as funções de AJAX, nem de animações, tornando-o mais leve, sendo uma boa opção para desenvolvedores que não vão precisar destas funcionalidades.

Uma outra distinção a se fazer é entre as versões de desenvolvimento e de produção. As versões de produção têm o código minificado e reduzido, tornando-o mais compacto, para onerar menos a banda do usuário quando ele fizer o download do jQuery. Normalmente ela é utilizada quando finalizamos o projeto e vamos colocá-la no servidor de produção.

Já a versão de desenvolvimento é uma versão que mostra o código como completo do jQuery, permitindo ao desenvolvedor ver como uma ou outra função do jQuery foi implementada, permitindo-o debbugar em caso de algum comportamento inesperado.

Neste treinamento, utilizaremos a versão normal do jQuery, a versão 3.1.0 de desenvolvimento, já que queremos aprender o máximo de funções possíveis, inclusive sobre AJAX e animações. Não se preocupe em baixá-la, pois ela já foi disponibilizada para você na pasta do projeto que você fará o download.

#### O projeto AluraTyper

Para praticar o conhecimento que iremos adquirir de jQuery, iremos desenvolver a aplicação AluraTyper. O AluraTyper é um jogo que tem como objetivo medir a velocidade de digitação de seus usuários, e salvar seu recordes em um placar. Esta aplicação parece simples, mas irá envolver quase toda a biblioteca de funções do jQuery, nos fazendo passar desde o básico de manipulação de elementos até requisições assíncronas com AJAX.

Depois que você fizer o download do projeto, abra-o no seu editor de textos e você deve ver a seguinte estrutura:
```
alura-typer/
├── public
│   ├── css
│   ├── fonts
│   ├── img
│   ├── js
│   │   ├── jquery.js
│   └── principal.html
└── servidor
```
Por enquanto vamos ignorar a pasta servidor e vamos no focar apenas na pasta public.

#### Iniciando o projeto: HTML base

Nosso primeiro passo é escrever um HTML inicial para nossa aplicação, então vamos começar editando o arquivo principal.html, para que ele contenha o título da nossa aplicação, uma frase , e uma <ul> que conterá o número de caracteres e de palavras da frase:

```html
<body>
    <h1>Alura Typer</h1>
    <p class="frase">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>

    <ul class="informacoes">
        <li>19 palavras</li>
        <li>15 segundos</li>
    </ul>
</body>
```

Adicionamos algumas classes para poder manipular estes elementos posteriormente.
Nosso objetivo inicial é que o nosso contador de palavras seja atualizado de acordo com a frase que está no HTML. Por exemplo, para a frase: "Alura: Cursos online de tecnologia que reinventam sua carreira.", ele deve mostrar 9 palavras. Para isso , vamos ter que começar a utilizar o JavaScript com jQuery.

### Primeiros passos com jQuery

#### Começando a trabalhar com Javacript: Importando scripts

Nosso primeiro passo é criar um arquivo JavaScript que conterá nosso código. Crie o arquivo main.js dentro da pasta /js:
```
alura-typer/
├── public
│   ├── css
│   ├── fonts
│   ├── img
│   ├── js
│   │   ├── main.js
│   │   └── jquery.js
```
Devemos agora importá-lo, utilizando a tag <script> no final da tag <body>, no arquivo principal.html:

```html
<--! Resto do código HTML -->
    <script src="js/main.js"></script>

</body>
</html>
```

Repare que importamos o script com o caminho js/main.js, já que ele está dentro da pasta /js.
Como o foco do treinamento é trabalhar com as funções do jQuery, vamos importar o jquery.js:

```html
<--! Resto do código HTML -->
    <script src="js/jquery.js"></script>
    <script src="js/main.js"></script>

</body>
</html>
```

Repare que importamos o jQuery acima do main.js, já que queremos utilizar a funções do jQuery dentro dele. É muito importante prestar atenção na ordem de importação dos seus scripts .js, para evitarmos bugs no nosso projeto.

#### Pegando a frase: A função seletora jQuery!

Para contarmos quantas palavras nossa frase tem, temos que ter acesso a ela dentro do nosso main.js. Precisamos selecionar o elemento do HTML dentro do JavaScript, e para isto nós vamos utilizar a função seletora do jQuery: A própria função jQuery().

Como o nosso parágrafo tem a classe frase (<p class="frase">...</p>), nós vamos utilizar esse seletor CSS na nossa função jQuery():

```javascript
//main.js
jQuery(".frase");
```

Mas precisamos salvar o elemento selecionado em uma variável:

```javascript
//main.js
var frase = jQuery(".frase");
```

Se você imprimir com um console.log(frase), você verá que conseguimos selecionar perfeitamente o elemento HTML, porém o que pode estar estranho aos seus olhos é que utilizamos a função jQuery(). É muito mais comum quando estudamos pela internet ver elementos sendo selecionados através do atalho para a função jQuery, representado pelo símbolo $. O $() é um atalho que nos economiza de escrever jQuery() toda vez que precisamos selecionar um elemento.

Como o jQuery se trata de produtividade, vamos a partir de agora utilizar a função $() para selecionar elementos!

Trocando no nosso código anterior:
```javascript
//main.js
var frase = $(".frase");
console.log(frase);
```

Vemos que o código continua funcionando igualmente.

#### Acessando o conteúdo de texto: função .text()

Mas o que estamos interessados é no conteúdo textual da tag <p>, ou seja o que está escrito de fato na frase.

Para conseguir acessar o texto da frase, vamos utilizar a função .text() do jQuery, que nos retorna o conteúdo de texto do elemento em formato de string, veja:

```javascript
//main.js
var frase = $(".frase").text();
console.log(frase);
// Retorno:
Lorem ipsum dolor sit amet, consectetur adipiscing...
```

Agora estamos salvando na variável o conteúdo em si da tag <p>, uma string com a frase que queremos contar o número de palavras!

#### Contando as palavras

Com a seguinte frase de exemplo: Alura: Cursos de tecnologia.

Sabemos que ela tem 4 palavras, pois conseguimos mentalmente diferenciar que cada palavra é separada por um espaço, e por isso conseguimos contá-las. Vamos adotar uma estratégia similar no código JavaScript para fazer a contagem. Quebraremos a nossa frase pelos espaços dela, e em seguida vamos contar as palavras restantes.

Primeiro, para quebrar uma string em espaços, vamos utilizar a conhecida função .split() do JavaScript tradicional, que nos retorna um array com as palavras separadas. Como queremos separar pelo espaço em branco(" "), vamos passar ele como parâmetro na função split:

```javascript
//main.js
var frase = $(".frase").text();
var numPalavras = frase.split(" ");
console.log(numPalavras);
// Retorno:
["Alura:", "Cursos", "de", "tecnologia"]
```

Como a variável numPalavras é um array, podemos nos aproveitar da propriedade .length dos arrays para nos dizer o tamanho do array, que é o mesmo do tamanho da frase recém dividida:

```javascript
//main.js
var frase = $(".frase").text();
var numPalavras = frase.split(" ").length;
console.log(numPalavras);
// Retorno:
4
```

#### Editando o número de palavras

Agora que conseguimos pegar o número de palavras da frase a ser digitada, precisamos alterar o indicador de palavras para que ele seja atualizado com este número. O primeiro passo é conseguir selecionar o elemento HTML que contém esta informação, para isso vamos envolver o número do indicador com um tag span, para que fique mais fácil acessá-lo:

```html
<!-- Restante do código HTML -->
    <ul class="informacoes">
        <li><span id="tamanho-frase">19</span> palavras</li>
        <li>15 segundos</li>
    </ul>
<!-- Restante do código HTML -->
```

E vamos selecionar essa tag span no main.js, utilizando a função $:

```javascript
//main.js
var frase = $(".frase").text();
var numPalavras = frase.split(" ").length;

var tamanhoFrase = $("#tamanho-frase");
```

Note que, como queremos selecionar através do id do elemento, utilizamos o seletor de id do CSS, a tralha (#).

Com o elemento selecionado, precisamos alterar o seu valor de texto para que ele contenha o número de palavras da frase, que está na variável numPalavras. Para isto vamos utilizar a função .text() do jQuery novamente, só que dessa vez vamos passar um parâmetro para ela, dizendo que queremos modificar o valor de texto do atributo:

```javascript
//main.js
var frase = $(".frase").text();
var numPalavras = frase.split(" ").length;

var tamanhoFrase = $("#tamanho-frase");
tamanhoFrase.text(numPalavras);
```

Ao reiniciar sua página, você deve notar que nosso indicador atualizou-se para o valor de palavras da frase! Conseguimos fazer a contagem automática de palavras.

Você pode notar que a função .text() do jQuery tem dois comportamentos, o primeiro , quando passamos sem nenhum parâmetro, nos retorna o valor de texto do elemento, e o segundo, quando passamos com um parâmetro, altera o valor de texto do elemento!

Diversas funções do jQuery tem essa característica, de variar o seu comportamento conforme os parâmetros passados, e você vai ver que este de retornar/alterar valor é um bastante comum. Vamos estudar várias outras como essa aqui no curso.

### Mãos na massa: Download inicial do projeto

Download do projeto e pré-requisitos: 
https://s3.amazonaws.com/caelum-online-public/jquery-alura-typer/stages/alura-typer-inicial.zip 

Para este curso precisamos fazer o download prévio do nosso projeto, que podemos baixar AQUI.
Você deve deszipar o arquivo baixado e encontrar uma estrutura como está:
```
alura-typer/
├── public
│   ├── css
│   │   └── estilos.css
│   ├── fonts
│   ├── img
│   ├── js
│   │   └── jquery.js
│   └── principal.html
└── servidor
```
Neste projeto também precisamos de um editor de textos para ser o nosso ambiente de desenvolvimento, eu recomendo o Atom , mas você pode usar outra opção de sua prefêrencia, como o Sublime Text 3 ou o Visual Studio Code (Win/Mac/Linux).

Também precisamos de um navegador para visualizar o resultado de nosso código, é recomendado o uso do Google Chrome.

Abra a pasta alura-typer/ no seu editor e o principal.html em seu navegador e vamos dar início ao desenvolvimento!


### Mãos na massa: Contando as palavras da frase e atualizando o seu contador

Agora podemos começar o desenvolvimento da página principal.html, o primeiro passo é escrever um HTML inicial, com o título da nossa aplicação, uma frase , e uma <ul> que conterá o número de caracteres e de palavras da frase, e algumas classes para manipular os elementos mais adiante:

```html
<body>
    <h1>Alura Typer</h1>
    <p class="frase">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>

    <ul class="informacoes">
        <li>19 palavras</li>
        <li>15 segundos</li>
    </ul>
</body>
```

Para atualizar os contadores de acordo com a frase que está no HTML, teremos que começar a utilizar o Javascript com jQuery. Então vamos criar um arquivo que conterá nosso código, o arquivo main.js dentro da pasta public/js, e vamos importá-lo na página principal.html, como último elemento da tag <body>. 

Vamos aproveitar para importar o jQuery também, como queremos usar as suas dentro no main.js, vamos importá-lo como primeiro script:

```html
<--! Resto do código HTML -->
    <script src="js/jquery.js"></script>
    <script src="js/main.js"></script>

</body>
</html>
```

No main.js, vamos acessar a frase utilizando o atalho para a função jQuery, acessando-a através da classe do seu elemento:
```javascript
$(".frase");
```

Vamos acessar o seu conteúdo, o seu texto, através da função text() e guardá-lo em uma variável:

```javascript
var frase = $(".frase").text();
```

Sabemos que as palavras são separadas por um espaço em branco, então vamos quebrar a frase onde houver espaços, utilizando a função split():
```javascript
var frase = $(".frase").text();
frase.split(" ");
```
O retorno dessa função é um array com as palavras separadas, então se acessarmos o seu tamanho (length), temos o número de palavras da frase. Vamos guardar esse resultado em uma variável também:

```javascript
var frase = $(".frase").text();
var numPalavras = frase.split(" ").length;
```

Já conseguimos contar a quantidade de palavras, mas ainda falta atualizar o contador no HTML. Primeiramente devemos selecionar o elemento HTML que contém a contagem de palavras. Como queremos somente o número, vamos envolvê-lo em um span e colocar um id nele:

```html
<!-- Página principal.html -->
<!-- Restante do código HTML -->
    <ul class="informacoes">
        <li><span id="tamanho-frase">19</span> palavras</li>
        <li>15 segundos</li>
    </ul>
<!-- Restante do código HTML -->
``` 

Agora, no main.js, vamos selecionar essa tag span, e modificar o seu conteúdo, passando o número de palavras por parâmetro para a função text():
```javascript
var frase = $(".frase").text();
var numPalavras = frase.split(" ").length;

var tamanhoFrase = $("#tamanho-frase");
tamanhoFrase.text(numPalavras);
```

Ou seja, a função .text() tem dois comportamentos, o primeiro , quando utilizamos-a sem nenhum parâmetro, nos é retornado o valor de texto do elemento, e o segundo, quando passamos um parâmetro para a função, ela altera o valor de texto do elemento!

Ao reiniciar sua página, você deve notar que nosso indicador atualizou-se para o valor de palavras da frase! Conseguimos fazer a contagem automática de palavras.

### Para saber mais: As antigas versões do jQuery

Sobre a compatibilidade das versões:

http://jquery.com/browser-support/

Vimos que uma das principais vantagens do jQuery é a compatibilidade com os diversos navegadores que ele oferece. Na teoria, se visitarmos a página de compatibilidade do jquery ele diz que só suporta as duas últimas versões de cada navegador.

Ná prática, sabemos que não é bem assim e que é bem provável que o jQuery funcione bem na maioria dos navegadores recentes, mesmo que não estejam nas últimas duas versões. E mesmo assim, se visitarmos o gráfico dos browsers mais usados, vemos que a grande maioria dos usuários já está nas últimas versões do Browser:

![jquery cmpatibilidade](https://github.com/josemalcher/ALURA-Curso-jQuery-Domine-a-biblioteca-mais-popular-do-mercado/blob/master/img_git/suporte_jquery_navegadores.png?raw=true)

Mas e se precisarmos dar suporte ao IE 8 e versões antigas?

Se você está desenvolvendo algum tipo de sistema que deve atender ao máximo de usuários possíveis, talvez seja bom você utilizar uma versão especial do jQuery: a versão 1.12.
Esta versão em específica do jQuery ficou muito famosa, e recebe updates até hoje. Ela é focada para dar suporte aos navegadores antigos, como Internet Explorer 6-8, Opera 12.1x ou Safari 5.1+.

Então caso você seu website tenha um público de usuários que notadamente não atualiza seus softwares, como os usuários da China que ainda tem boa parte de seus usuários utilizando o Windows XP, é interessante você utilizar esta versão do jQuery, pois ela é focada em dar suporte maior aos browers antigos. Talvez algumas das funções que aprendemos aqui neste treinamento não sejam válidas no jQuery 1.12, mas um rápida consulta a documentação do jQuery resolverá suas dúvidas :) .




[Voltar ao Índice](#indice)

---

## <a name="parte2">2.Escutando eventos com jQuery</a>


[Voltar ao Índice](#indice)

---

## <a name="parte3">3.Criando o GameOver com eventos</a>


[Voltar ao Índice](#indice)

---

## <a name="parte4">4.Reiniciando nosso jogo</a>


[Voltar ao Índice](#indice)

---

## <a name="parte5">5.Funções que auxiliam os estilos</a>


[Voltar ao Índice](#indice)

---

## <a name="parte6">6.Criando e manipulando elementos com jQuery</a>


[Voltar ao Índice](#indice)

---

