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

Nosso primeiro passo é escrever um HTML inicial para nossa aplicação, então vamos começar editando o arquivo principal.html, para que ele contenha o título da nossa aplicação, uma frase , e uma "ul" que conterá o número de caracteres e de palavras da frase:

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
Devemos agora importá-lo, utilizando a tag "script" no final da tag "body", no arquivo principal.html:

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

Como o nosso parágrafo tem a classe frase ("p class="frase""..."/p"), nós vamos utilizar esse seletor CSS na nossa função jQuery():

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

Mas o que estamos interessados é no conteúdo textual da tag "p", ou seja o que está escrito de fato na frase.

Para conseguir acessar o texto da frase, vamos utilizar a função .text() do jQuery, que nos retorna o conteúdo de texto do elemento em formato de string, veja:

```javascript
//main.js
var frase = $(".frase").text();
console.log(frase);
// Retorno:
Lorem ipsum dolor sit amet, consectetur adipiscing...
```

Agora estamos salvando na variável o conteúdo em si da tag "p", uma string com a frase que queremos contar o número de palavras!

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

Agora podemos começar o desenvolvimento da página principal.html, o primeiro passo é escrever um HTML inicial, com o título da nossa aplicação, uma frase , e uma "ul" que conterá o número de caracteres e de palavras da frase, e algumas classes para manipular os elementos mais adiante:

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

Para atualizar os contadores de acordo com a frase que está no HTML, teremos que começar a utilizar o Javascript com jQuery. Então vamos criar um arquivo que conterá nosso código, o arquivo main.js dentro da pasta public/js, e vamos importá-lo na página principal.html, como último elemento da tag "body". 

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

### Eventos do jQuery

Sejam bem-vindos a mais um capítulo do treinamento de jQuery. Nós já implementamos corretamente o contador de palavras da frase a ser digitada e o próximo passo é disponibilizarmos um campo na página para o usuário poder digitar nele, para começarmos a ter uma interatividade com o jogo, já que atualmente nosso jogo somente conta as palavras.

Vamos colocar um textarea para o usuário digitar a frase e dois contadores, um para contar quantos caracteres o usuário digitou, e outro para contar quantas palavras foram digitadas.
Então, na página principal.html, logo após a ul de informações, colocamos o textarea:
```html
<textarea class="campo-digitacao" rows="8" cols ="40"></textarea>
```

E logo abaixo, criamos uma ul (semelhante à que já temos) com duas lis, cada uma representando um contador:

```html
<ul>
    <li><span id="contador-caracteres">0</span> caracteres</li>
    <li><span id="contador-palavras">0</span> palavras</li>
</ul>
```

### Trabalhando com eventos

O usuário já consegue digitar a frase no campo específico, mas os contadores permanecem zerados. Podemos fazer com que os contadores sejam atualizados toda vez que o usuário clicar no textarea, contando assim os caracteres e palavras já digitados e atualizando os respectivos spans.

Para fazer isso, temos que entender os famosos eventos do JavaScript. Como vocês já sabem, o JavaScript possui uma série de eventos, como um evento para click, double click, scroll, entre outras interatividades, e o jQuery nos facilita muito a escutar os eventos JavaScript dos nossos elementos.

Para comprovar isso, vamos utilizá-lo no caso acima, para atualizar os contadores toda vez que o usuário clicar no textarea. Vamos passo a passo. Primeiramente, no main.js, se queremos detectar um evento de clique no campo, primeiro devemos selecioná-lo:

```javascript
var campo = $(".campo-digitacao");
```

Agora, quando o campo for clicado, temos que "fazer alguma coisa". Essa ação de "quando o campo for..." faz referência à função on do jQuery, e como queremos o evento do clique no campo, passamos "click" para a função:

```javascript
var campo = $(".campo-digitacao");
campo.on("click");
```

E para "fazer algo" quando o campo for clicado, passamos um segundo parâmetro para a função on, passamos uma função, a já conhecida função anônima:

```javascript
var campo = $(".campo-digitacao");
campo.on("click", function() {

});
```

Dentro da função anônima, iremos implementar o que queremos que aconteça quando clicarem no campo. Toda vez que clicarem no campo, essa função será chamada. Para comprovar isso, podemos imprimir uma mensagem no console do navegador toda vez que o campo for clicado, para isso colocamos um console.log dentro da função:

```javascript
var campo = $(".campo-digitacao");
campo.on("click", function() {
    console.log("Cliquei no campo");
});
```

Atualizamos a página, abrimos o console do navegador e vemos que toda vez que clicamos no campo, a mensagem "Cliquei no campo" é exibida. Com isso, podemos partir para o nosso objetivo, que é contar as palavras. Nós já vimos anteriormente que uma boa maneira de contarmos as palavras, é pegar o conteúdo do campo, fazer um split nele no espaço e pegar o seu tamanho. Podemos utilizar essa mesma tática aqui, mas como pegar o valor do textarea?

No caso do textarea, o seu conteúdo não estará na propriedade text e sim no value, ou val, que é como o jQuery o chama:

```javascript
var campo = $(".campo-digitacao");
campo.on("click", function() {
    console.log(campo.val());
});
```

Agora toda vez que clicamos no campo, o seu conteúdo é impresso no console. Lembrando que o val nos dá acesso ao que está dentro de uma tag de input, como as tags input e textarea; já o text nos dá acesso ao que está dentro de uma tag de texto, como p, span e h1.

#### Contando os caracteres e as palavras digitadas
Agora que já sabemos como o val funciona (que é o conteúdo da nossa frase), podemos fazer o split nele e contar as palavras:

```javascript
var campo = $(".campo-digitacao");
campo.on("click", function() {
    var conteudo = campo.val();
    var qtdPalavras = conteudo.split(" ").length;
});
```

Para testar, vamos imprimir a quantidade de palavras para ver se estamos contando corretamente:
```javascript
var campo = $(".campo-digitacao");
campo.on("click", function() {
    var conteudo = campo.val();
    var qtdPalavras = conteudo.split(" ").length;
    console.log(qtdPalavras);
});
```

Aparentemente está funcionando, a cada clique no campo, é impresso a quantidade de palavras nele escritas. Mas não basta só contar as palavras, temos que atualizar o seu contador, ou seja, temos que selecionar o span e alterar o seu text, atribuindo a quantidade de palavras a ele:

```javascript
var campo = $(".campo-digitacao");
campo.on("click", function() {
    var conteudo = campo.val();
    var qtdPalavras = conteudo.split(" ").length;

    $("#contador-palavras").text(qtdPalavras);
});
```

Podemos escrever a frase, e a cada clique o contador é atualizado corretamente! Ótimo, agora só falta contar os caracteres, que é mais fácil ainda, é só pegarmos o conteúdo do campo, e o seu tamanho (length) será a quantidade de caracteres. Sabendo disso, podemos também atualizar o seu contador:

```javascript
var campo = $(".campo-digitacao");
campo.on("click", function() {
    var conteudo = campo.val();

    var qtdPalavras = conteudo.split(" ").length;
    $("#contador-palavras").text(qtdPalavras);

    var qtdCaracteres = conteudo.length;
    $("#contador-caracteres").text(qtdCaracteres);
});
```

#### O evento input

Pronto, só que para atualizar os contadores, estamos tendo sempre que clicar dentro do campo, o que não é nada legal, o ideal é que o contador seja atualizado enquanto o usuário digita. E para isso existe um evento específico de quando digitamos, colocamos dados em um campo, que é o evento input:

```javascript
var campo = $(".campo-digitacao");
campo.on("input", function() {
    var conteudo = campo.val();

    var qtdPalavras = conteudo.split(" ").length;
    $("#contador-palavras").text(qtdPalavras);

    var qtdCaracteres = conteudo.length;
    $("#contador-caracteres").text(qtdCaracteres);
});
```

Repare que agora, enquanto digitamos, o campo vai sendo atualizado, e era justamente isso que queríamos.

#### Separando através de Regexp

A contagem tanto das palavras quanto dos caracteres aparentemente está funcionando, mas se olharmos atentamente podemos reparar que se apagarmos alguma frase escrita, o contador de palavras ainda conta uma, além disso, se dermos vários espaços, o contador conta como se cada espaço equivalesse a uma palavra. Isso tem relação com o modo que estamos contando as palavras, fazendo um split em um espaço vazio.
Para contar mais precisamente temos que utilizar uma expressão regular no lugar do espaço vazio, uma expressão regular que busca qualquer caractere, exceto espaço vazio, essa expressão é /\S+/:

```javascript
var campo = $(".campo-digitacao");
campo.on("input", function() {
    var conteudo = campo.val();

    var qtdPalavras = conteudo.split(/\S+/).length;
    $("#contador-palavras").text(qtdPalavras);

    var qtdCaracteres = conteudo.length;
    $("#contador-caracteres").text(qtdCaracteres);
});
```

Agora os espaços não são mais considerados como palavras, mas a contagem sempre mostra a quantidade de palavras mais uma, para resolver isso vamos subtrair um do length do conteúdo:

```javascript
var campo = $(".campo-digitacao");
campo.on("input", function() {
    var conteudo = campo.val();

    var qtdPalavras = conteudo.split(/\S+/).length - 1;
    $("#contador-palavras").text(qtdPalavras);

    var qtdCaracteres = conteudo.length;
    $("#contador-caracteres").text(qtdCaracteres);
});
```

#### Mãos na massa: Contando através de eventos

Contando através de eventos

Vamos adicionar uma textarea à nossa página e começar a trabalhar com eventos. Mãos à obra :)

1) Abra o arquivo public/principal.html e adicione uma textara e um ul, logo após a ul de informações:
```html
<textarea class="campo-digitacao" rows="8" cols ="40"></textarea>

<ul>
    <li><span id="contador-caracteres">0</span> caracteres</li>
    <li><span id="contador-palavras">0</span> palavras</li>
</ul>
```

2) Vamos adicionar um evento ao nosso campo-digitacao. Abra o arquivo public/js/main.js e coloque no final:
```javascript
var campo = $(".campo-digitacao");
campo.on("input", function() {


});
```

Selecionamos o campo pelo nome da classe e já associamos o evento input com ele.

3) Dentro da função anônima do evento recupere o valor (val()) do campo, conta as palavras usando a função split(..) e imprime no console.
```javascript
var conteudo = campo.val();
var qtdPalavras = conteudo.split(/\S+/).length - 1;
$("#contador-palavras").text(qtdPalavras);

```

Você já pode testar esse código no navegador. O contador de palavras deve mostrar a quantidade de palavras.

4) Logo após do $("#contador-palavras") atualize também o contador de caracteres: 

```javascript
var qtdCaracteres = conteudo.length;
$("#contador-caracteres").text(qtdCaracteres);
```

5) Salve e teste o seu código no navegador:


#### Mãos na massa: Contando através de eventos
 
Segue o código completo do arquivo main.js:
```javascript
var frase = $(".frase").text();
var numPalavras  = frase.split(" ").length;
var tamanhoFrase = $("#tamanho-frase");

tamanhoFrase.text(numPalavras);


var campo = $(".campo-digitacao");
campo.on("input", function() {
    var conteudo = campo.val();
    var qtdPalavras = conteudo.split(/\S+/).length - 1;
    console.log(qtdPalavras);
    $("#contador-palavras").text(qtdPalavras);

    var qtdCaracteres = conteudo.length;
    $("#contador-caracteres").text(qtdCaracteres);

});

```



[Voltar ao Índice](#indice)

---

## <a name="parte3">3.Criando o GameOver com eventos</a>

### Game Over com eventos

Nosso jogo está começando a criar forma, mas está faltando algo característico de todo jogo, o Game Over. Nós temos um tempo limite para o usuário digitar a frase, então ele deve decrescer, e quando o mesmo zerar, o usuário perde o jogo, não conseguindo mais digitar no campo. Vamos começar?

#### Contagem regressiva para digitação

Assim que o usuário clicar no campo de digitação, a contagem regressiva deve iniciar, então primeiramente devemos detectar essa ação do usuário "entrar no campo". Será que podemos usar o evento click? Clicando no campo, nós entramos nele, ok. Mas será que essa é a única maneira? Não, podemos entrar no campo utilizando a tecla TAB também.

Pensando nisso, há um evento específico para quando entramos dentro de um campo, que é o evento focus, que é quando o campo ganha o foco para ser utilizado. Logo, no main.js, podemos começar a implementar o nosso código:
```javascript
campo.on("focus", function() {
});
```

Se queremos que o tempo decresça, temos que saber o seu valor. Para isso, na página principal.html, vamos envolver o tempo em uma tag "span", e colocar o id tempo-digitacao:
```html
<ul class="informacoes">
    <li><span id="tamanho-frase">5</span> palavras</li>
    <li><span id="tempo-digitacao">10</span> segundos</li>
</ul>
```

Voltando ao main.js, vamos pegar o conteúdo do span e salvá-lo em uma variável:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
});
```

Feito isso, temos que implementar a lógica. A cada segundo que se passar, temos que subtrair 1 do nosso tempo restante. Para tal, vamos utilizar a função setInterval do JavaScript, que faz com que uma determinada ação (passada como primeiro parâmetro) seja executada em um intervalo de tempo (passado como segundo parâmetro, no nosso caso, 1 segundo, ou 1000 milissegundos):

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
    setInterval(function() {

    }, 1000);
});
```

Dentro o setInterval podemos subtrair 1 do nosso tempo restante a cada segundo que passe, logo:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
    setInterval(function() {
        tempoRestante--;
    }, 1000);
});
```

Falta agora atualizarmos o contador com o tempo restante, bem semelhante ao que já fizemos anteriormente:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
    setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
    }, 1000);
});
```

Perfeito, nosso tempo já está decrescendo, só que o mesmo ainda não influencia em nada no jogo, já que o usuário consegue ficar digitando mesmo com o tempo zerado. Vamos então desabilitar o campo para que o usuário não consiga mais digitar nada quando o tempo zerar.

A textarea possui um atributo disabled, que faz com que não consigamos digitar nada na mesma (justamente o que queremos). Então o que queremos é que quando o tempo chegar a 0, o JavaScript vai e "coloca" o atributo disabled na textarea. Como queremos adicionar um atributo, o jQuery nos auxilia disponibilizando a função attr.

Essa função funciona de maneira semelhante à função text, podendo pegar o valor de um atributo, ou modificá-lo. Por exemplo, para pegar o valor do atributo rows do nosso campo, fazemos:

```javascript
var campo = $(".campo-digitacao");
campo.attr("rows");
```

E para modificar o mesmo, passamos mais um parâmetro para a função, que é o novo valor do atributo, por exemplo:

```javascript
var campo = $(".campo-digitacao");
campo.attr("rows", 500);
```

Só que o atributo disabled não tem nenhum valor, só queremos colocá-lo na tag. Nesse caso, nós temos que informar isso passando o valor true (verdadeiro) para a função, assim estaremos "habilitando" o atributo:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
    setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        campo.attr("disabled", true);
    }, 1000);
});
```

Como queremos desabilitar o campo somente quando o tempo chegar a 0, vamos envolver essa linha em uma condição if:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
    setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if (tempoRestante < 1) {
            campo.attr("disabled", true);
        }
    }, 1000);
});
```

Testamos e vemos que assim que o tempo chega a 0, o campo é travado, perfeito! Mas ainda temos um bug, porque o tempo continua decrescendo depois do 0, ou seja, ele fica negativo. Temos que fazer com que a função setInterval pare quando o tempo for 0, mas como?
Para isso, existe a função clearInterval, que recebe o id do setInterval como parâmetro. Vamos colocá-la dentro do nosso if:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
    setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if (tempoRestante < 1) {
            campo.attr("disabled", true);
            clearInterval(id);
        }
    }, 1000);
});
```

Mas atualmente não temos acesso a essa id da função setInterval, como consegui-lo? Toda função setInterval retorna o seu próprio id, logo basta guardarmos esse id em uma variável e passá-lo para a função clearInterval:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.on("focus", function() {
    var cronometroID = setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if (tempoRestante < 1) {
            campo.attr("disabled", true);
            clearInterval(cronometroID);
        }
    }, 1000);
});
```

Podemos testar mais uma vez, e ver que agora tudo funciona como o esperado. Será?
#### Escutando um evento uma única vez

O que acontece se entrarmos vários vezes no nosso campo? Repare que toda vez que entramos no campo, o tempo decresce mais rápido, chegando até a ficar negativo! Isso acontece porque toda vez que o campo é focado, a nossa lógica é executada. O ideal seria que esse código só seja executado uma única vez.

O problema é que a função on fica escutando o evento o tempo todo, e para que ela funcione somente na primeira vez, existe a função one, que funciona exatamente como a função on, só que só escuta o evento uma única vez:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.one("focus", function() {
    var cronometroID = setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if (tempoRestante < 1) {
            campo.attr("disabled", true);
            clearInterval(cronometroID);
        }
    }, 1000);
});
```

### Mãos na massa: Game over

Implementando a lógica de Game Over
Assim que o usuário clicar no campo de digitação, deve começar a contagem regressiva do jogo. Como apresentado no video, vamos implementar essa funcionalidade:

1) Abra o arquivo principal.html e envolva o tempo em uma tag "span", colocando o id tempo-digitacao. Adicione o elemento span apenas dentro da segunda li:
```html
<ul class="informacoes">
    <li><span id="tamanho-frase">5</span> palavras</li>
    <li><span id="tempo-digitacao">10</span> segundos</li>
</ul>
```

Repare que usamos a ul com a classe informacoes.
2) Abra o arquivo main.js e acrescente no final o código para selecionar o elemento span:
var tempoRestante = $("#tempo-digitacao").text();
3) Ainda no main.js adicione logo depois da variável tempoRestante o evento blur que fica associando com o nosso campo:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.one("focus", function() {
    //aqui vem mais
});
```

Repare que já usamos a função one que garante que o evento será associado apenas uma vez.
4) Dentro da função anônima usa o setInterval para diminiur o tempoRestante a cada segundo:
```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.one("focus", function() {
    var cronometroID = setInterval(function() {
        tempoRestante--;
        //aqui vem mais
    }, 1000);
});
```

Perceba que a função setInterval devolve uma id (cronometroID).
5) Agora só falta atualizar o tempo-digitacao no DOM e verificar se o tempo já esgotou. Lembra-se de desabilitar o campo através da função attr e de limpar o intervalo (clearInterval): 
```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.one("focus", function() {
    var cronometroID = setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if (tempoRestante < 1) {
            campo.attr("disabled", true);
            clearInterval(cronometroID);
        }
    }, 1000);
});
```

6) Pronto, salve tudo e teste no seu navegador!


### Mãos na massa: Game over
 
Implementando cada mais funcionalidades o nosso código também cresceu. No próximo capítulo vamos organizar o nosso código melhor!
```javascript
var frase = $(".frase").text();
var numPalavras  = frase.split(" ").length;
var tamanhoFrase = $("#tamanho-frase");

tamanhoFrase.text(numPalavras);


var campo = $(".campo-digitacao");
campo.on("input", function() {
    var conteudo = campo.val();
    var qtdPalavras = conteudo.split(/\S+/).length - 1;
    console.log(qtdPalavras);
    $("#contador-palavras").text(qtdPalavras);

    var qtdCaracteres = conteudo.length;
    $("#contador-caracteres").text(qtdCaracteres);

});

var tempoRestante = $("#tempo-digitacao").text();
campo.one("focus", function() {
    var cronometroID = setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if (tempoRestante < 1) {
            campo.attr("disabled", true);
            clearInterval(cronometroID);
        }
    }, 1000);
});
```

[Voltar ao Índice](#indice)

---

## <a name="parte4">4.Reiniciando nosso jogo</a>

### Código atal
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Alura Typer</title>
</head>

<body>
    <h1>Alura Typer</h1>
    <p class="frase">Esta frase tem varias e varias palavras. Esta frase tem varias e varias palavras</p>
    <ul class="informacoes">
        <li>
            <span id="tamanho-frase">5</span> palavras</li>
        <li><span id="tempo-digitacao">10</span> segundos</li>
    </ul>

    <textarea class="campo-digitacao" rows="8" cols="40"></textarea>
    <button id="botao-reiniciar">Reiniciar Jogo</button>

    <ul>
        <li>
            <span id="contador-caracteres">0</span> caracteres</li>
        <li><span id="contador-palavras">0</span> palavras</li>
    </ul>

    <script src="js/jquery-3.3.1.min.js"></script>
    <script src="js/main.js"></script>
</body>

</html>
```

```javascript
var tempoInicial = $("#tempo-digitacao").text();
var campo = $(".campo-digitacao");

//$(document).readyState(function(){
$(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();
    $("#botao-reiniciar").click(reinicializaJogo) ;
});

function atualizaTamanhoFrase() {
    var frase = $(".frase").text();
    var numPalavras = frase.split(" ").length;
    var tamanhoFrase = $("#tamanho-frase");
    tamanhoFrase.text(numPalavras);
}

function inicializaContadores() {
    campo.on("input", function () {
        var conteudo = campo.val();

        var qtdPalavras = conteudo.split(/\S+/).length - 1;
        $("#contador-palavras").text(qtdPalavras);

        var qtdCaracteres = conteudo.length;
        $("#contador-caracteres").text(qtdCaracteres);
    });
}

function inicializaCronometro() {
    var tempoRestante = $("#tempo-digitacao").text();
    campo.one("focus", function () {
        var cronometroID = setInterval(function () {
            tempoRestante--;
            //console.log(tempoRestante);
            $("#tempo-digitacao").text(tempoRestante);
            if (tempoRestante < 1) {
                campo.attr("disabled", true);
                clearInterval(cronometroID);
            }
        }, 1000);
    });
}

/* $("#botao-reiniciar").on("click", function(){
    console.log("BOão Clicado");
}); */
/* 
$("#botao-reiniciar").click(function () {
    //console.log("Botão clicando com .click()");
}); */
function reinicializaJogo() {
    campo.attr("disabled", false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
    $("#tempo-digitacao").text(tempoInicial);
    inicializaCronometro();
}

```

### Reiniciando o jogo

Queremos dar a opção do nosso usuário reiniciar o nosso jogo sem ter que recarregar a página, e para isto vamos implementar um pequeno botão, que ao ser clicado, vai zerar os nosso campos e contadores, permitindo o usuário iniciar uma nova rodada no jogo.

Como primeiro passo, vamos adicionar um "button" no nosso HTML, abaixo da "textarea":
```html
<!-- Restante do HTML -->

<textarea class="campo-digitacao" rows="8" cols="40"></textarea>
<button id="botao-reiniciar">Reiniciar Jogo</button>

<!-- Restante do HTML -->
```

Agora precisamos atrelar um evento de click neste botão recém criado. Até agora , vimos como fazer isto através da função on("click",function(){...}) do jQuery, porém vamos aprender um novo modo de ter acesso a este evento.

#### Um atalho para função on("click"), a shorthand click()

Os eventos do Javascript que são mais comuns, como o click, blur( evento de sair de um campo), dblclick(Clique duplo) tem funções próprias no jQuery, que são funções de atalho, evitando precisar chamar a função on() e chamando diretamente a função do próprio evento.
Veja no exemplo abaixo, aonde capturamos o evento de click em um título e exibimos uma mensagem no console como resposta:
```javascript
var titulo = $("#titulo");
titulo.on("click",function(){
    console.log("Titulo foi clicado!");
});
```

Poderíamos executar este mesmo evento e ação com a função de atalho click():

```javascript
var titulo = $("#titulo");
titulo.click(function(){
    console.log("Titulo foi clicado!");
});
```

Podemos ser mais sucintos ainda e escrever tudo em uma linha só:

```javascript
$("#titulo").click(function(){
    console.log("Titulo foi clicado!");
});
```

Como o jQuery é uma grande ajuda na produtividade, ele disponibiliza algumas dessas funções de atalho, que são mais curtas e simples para agilizar a vida do programador.
Vamos atrelar um evento de click no nosso botão com está nova função:

```javascript
//main.js

$("#botao-reiniciar").click(function(){
    console.log("Reiniciando o jogo...");
});
```

#### Reiniciando o jogo: tratando do campo

Agora que estamos detectando o evento de click no botão reiniciar, vamos começar a retornar o jogo para estado inicial, como se o usuário estivesse acabado de entrar na página. O primeiro passo é habilitarmos o campo novamente, pois quando colocamos o atributo disabled nele na hora do Game Over impedimos o usuário de digitar.
Para removê-lo, vamos nos aproveitar da função .attr() do jQuery:
```javascript
//main.js

$("#botao-reiniciar").click(function(){
    campo.attr("disabled", false);
});
```

A função .attr() nos permite colocar, retirar ou modificar valores de atributos de elementos HTML.

Agora com o campo digitável, precisamos zera-lo, pois ele ainda contêm os resquicíos da ultima jogada do nosso usuário. Queremos que o conteúdo da "textarea" seja zerado, fique vazio.

Sabemos que para manipular o conteúdo de um elemento de input do usuário, como a "textarea", temos que utilizar a função .val(), e como queremos que ela fique vazia , faremos assim:
```javascript
//main.js

$("#botao-reiniciar").click(function(){
    campo.attr("disabled", false);
    campo.val("");
});
```

Colocando o conteúdo(.val()) do campo como vazio(""), ele ficará zerado.
Agora nosso campo está limpo e pode ser digitado novamente.

#### Reiniciando o jogo: zerando os contadores

Nosso próximo passo é retornar os contadores para seu estado inicial, ou seja, com zero palavras.

Este é mais fácil, basta selecionar os dois contadores e substituir o texto dos "span" por 0.

```javascript
//main.js

$("#botao-reiniciar").click(function(){
    campo.attr("disabled", false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
});
```

Com os contadores zerados, fica faltando apenas ajustar o tempo inicial!

#### Reiniciando o jogo: restaurando o tempo inicial

Para obtermos o tempo inicial, temos que guarda-lo numa variável assim que iniciamos a aplicação, pois como alteramos o valor do tempo depois, acabamos perdendo-o. Vamos criar uma variável chamada tempoInicial e capturar o valor assim que o script foi carregado:

```javascript
//main.js
var tempoInicial = $("#tempo-digitacao").text();

// Resto do código
```

Agora que temos o valor do tempo inicial, podemos reatribui-lo ao marcador de tempo quando clicarmos no botão de reiniciar:

```javascript
//main.js

$("#botao-reiniciar").click(function(){
    campo.attr("disabled", false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
    $("#tempo-digitacao").text(tempoInicial);
});
```

Agora o tempo inicial é restaurado corretamente.

#### Reiniciando o jogo: atrelando o evento de focus ao campo

Nosso botão reiniciar está quase funcionando completamente, ele já zera os campos e contadores, e restaura o tempo inicial! No entanto, ao testar o botão, percebemos que o jogo não será reinicializado.

O problema é que o evento input do campo foi associando apenas uma vez (one) pelo nosso código. Para resolver bastaria reatrelar um novo evento de focus ao campo, que fará o trabalho do cronômetro. O nosso evento de focus deve ser atribuído novamente com a função one do jQuery, pois como vimos só queremos que ele seja executado uma única vez.
Para fazer isto, poderíamos simplesmente copiar e colar o código que implementa o cronometro. Lembrando do código que você já escreveu:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.one("focus",function(){
    var cronometroID = setInterval(function(){
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if(tempoRestante < 1){
            campo.attr("disabled", true);
            clearInterval(cronometroID);
        }
    },1000);
});
```

Poderíamos usar esse código dentro da função de click() do botão reiniciar, porém isto seria uma má prática de programação, pois estaríamos colando código repetido em dois lugares diferentes!

Sabemos que podemos reaproveitar este pedaço de código caso ele estivesse mais modularizado e organizado em funções. Como nosso código está crescendo muito, agora é uma boa hora de fazer esta separação de responsabilidades.

### Organizando o nosso código em funções

Vamos separar cada bloco de código em uma função com um nome bem semântico, que especifique o que aquele bloco de código fará. Vamos começar pelo topo do arquivo main.js, aonde temos este bloco de código:

```javascript
var frase = $(".frase").text();
var numPalavras  = frase.split(" ").length;
var tamanhoFrase = $("#tamanho-frase");
tamanhoFrase.text(numPalavras);
```

Vemos que ele é responsável por atualizar o tamanho da frase, logo vamos envolvê-lo numa função de mesmo nome:

```javascript
function atualizaTamanhoFrase() {
    var frase = $(".frase").text();
    var numPalavras  = frase.split(" ").length;
    var tamanhoFrase = $("#tamanho-frase");
    tamanhoFrase.text(numPalavras);
}
```

Continuando a olhar o arquivo main.js, vemos o trecho abaixo:
```javascript
var campo = $(".campo-digitacao");
campo.on("input",function(){
    var conteudo = campo.val();

    var qtdPalavras = conteudo.split(/\S+/).length;
    $("#contador-palavras").text(qtdPalavras);

    var qtdCaracteres = conteudo.length;
    $("#contador-caracteres").text(qtdCaracteres);
});
```

Claramente aqui temos outro bloco de função, já que este pedaço de código é inteiramente responsável por inicializar os contadores de palavras e caracteres. Vamos deixar a variável campo em separada no topo do main.js, pois ela é utilizada em vários locais e vamos envolver este bloco em uma função:

```javascript
//var campo fica no topo da página
function inicializaContadores() {
    campo.on("input",function(){
        var conteudo = campo.val();

        var qtdPalavras = conteudo.split(/\S+/).length;
        $("#contador-palavras").text(qtdPalavras);

        var qtdCaracteres = conteudo.length;
        $("#contador-caracteres").text(qtdCaracteres);
    });
}
```

Continuando a olhar o main.js vamos encontrar mais um bloco que já precisamos que se tornasse uma função, o bloco que inicializa o cronometro para marcar o tempo:

```javascript
var tempoRestante = $("#tempo-digitacao").text();
campo.one("focus", function() {
    var cronometroID = setInterval(function() {
        tempoRestante--;
        $("#tempo-digitacao").text(tempoRestante);
        if (tempoRestante < 1) {
            campo.attr("disabled", true);
            clearInterval(cronometroID);
        }
    }, 1000);
});
```

Vamos envolvê-lo em uma função:
```javascript
function inicializaCronometro() {
    var tempoRestante = $("#tempo-digitacao").text();
    campo.one("focus", function() {
        var cronometroID = setInterval(function() {
            tempoRestante--;
            $("#tempo-digitacao").text(tempoRestante);
            if (tempoRestante < 1) {
                campo.attr("disabled", true);
                clearInterval(cronometroID);
            }
        }, 1000);
    });
}
```

Por último o nosso código recém escrito, que tem como função reiniciar o nosso jogo. Vamos separar a função seletora da função de reiniciar e também separa-lo em uma função com nome semântico:

```javascript
$("#botao-reiniciar").click(reiniciaJogo);
function reiniciaJogo(){
    campo.attr("disabled",false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
    $("#tempo-digitacao").text(tempoInicial);
}
```

Agora sim nosso código está bem mais organizado e modularizado, com blocos de função com responsabilidades bem definidas.
Podemos agora chamar a função inicializaCronometro dentro da reiniciaJogo, já que agora são código reaproveitáveis:
```javascript
$("#botao-reiniciar").click(reiniciaJogo);
function reiniciaJogo(){
    campo.attr("disabled",false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
    $("#tempo-digitacao").text(tempoInicial);
    // Adicionamos aqui \/
    inicializaCronometro();
}
```

Graças a nossa separação podemos fazer o reuso de uma mesma função em diversos pedaços do código.

#### Código organizado...mas funcionando?

Conseguimos separar nosso código em diversas funções, com nomes bem claros que especificam suas funcionalidades, porém se você abrir a página, verá que o nosso jogo Alura Typer não está mais funcionando como deveria! Ele não conta palavras, os eventos não são atribuídos e tudo que foi feito até agora parou de funcionar.

Como agora todo nosso código está isolado dentro de funções, precisamos que alguém invoque estas funções para que elas sejam executadas! Afinal nossos eventos só serão atrelados aos elementos HTML quando nossas funções forem chamadas!

Para fazer isto, vamos utilizar uma função do jQuery que aguarda a página ser carregada e depois executa seu conteúdo: a função $(document).ready()
Sabemos que para que o Javascript manipule uma página com segurança ele deve aguardar todos os seus elementos serem carregados, e é exatamente ai que a função $(document).ready() vai entrar. Vamos coloca-la no nosso código e assim que a página for carregada ela irá executar nossas funções para nós:

```javascript
//main.js
$(document).ready(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();
    $("#botao-reiniciar").click(reiniciaJogo);
});
```

#### Vamo aproveitar e atrelar o evento quando da função iniciar dentro dela também.

Como está é uma função bastante utilizada do jQuery, ela também tem um atalho , que é a função chamada deste modo : $(function() { ... }); . Quando passamos uma função dentro da função $() , estamos na verdade utilizando a função $(document).ready(). Como é mais prático utilizar este segundo modo, vamos alterar nosso código:

```javascript
//main.js
$(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();
    $("#botao-reiniciar").click(reiniciaJogo);
});
```

Conferindo a organização
Depois de separada e organizado, nosso código deve deste modo:

```javascript
//main.js
var tempoInicial = $("#tempo-digitacao").text();
var campo = $("#campo-digitacao");

$(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();
    $("#botao-reiniciar").click(reiniciaJogo);
});

function atualizaTamanhoFrase(){
    ...
}
function inicializaContadores(){
    ...
}
function inicializaCronometro(){
    ...
}
function reiniciaJogo(){
    ...
}
```

Apesar deste pequeno trabalho inicial de organizar o código, daqui pra frente mantê-lo será muito mais fácil, pois agora podemos usar e abusar de nossas funções para reaproveitar bastante as funcionalidades.

E nossa função de reiniciar funciona corretamente, fazendo com que nosso usuário possa jogar o AluraTyper repetidas vezes sem precisar apelar para o botão F5!


### Mãos na massa: Botão para reinicializar o jogo

####Criando o botão reiniciar

1) Como primeiro passo, adicione um "button" na página principal.html, logo abaixo da "textarea":
```html
<button id="botao-reiniciar">Reiniciar Jogo</button>
```

2) No arquivo main.js atrele o evento de click com no nosso botão. Dentro da função do evento reative o o campo pela função attr:
```javascript
$("#botao-reiniciar").click(function(){
    campo.attr("disabled", false);
    //aqui vem mais
});
```
3) Ainda na função do evento reinicie o campo, o contador-palavras e o contador-caracteres:
```javascript
$("#botao-reiniciar").click(function(){
    campo.attr("disabled", false);
    //inicializando os campos
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
});
```
4) Falta ainda reinicializar o tempo inicial. Vamos guardar o tempoInicial em uma variável auxiliar. No início do arquivo main.js, logo após tamanhoFrase.text(numPalavras); adicione:
```javascript
var tempoInicial = $("#tempo-digitacao").text();
```
5) Agora use esssa variável dentro da função do evento click do nosso botão:
```javascript
$("#botao-reiniciar").click(function(){
    campo.attr("disabled", false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");

    $("#tempo-digitacao").text(tempoInicial); //novo

});
```

Isso faz que o tempo inicial volte ao elemento tempo-digitacao.

6) Salve tudo e teste no navegador. O botão já deve reinicializar os valores. 
No entanto ainda não está 100%. Qual é o problema?.

### Mãos na massa: Organizando o código

Objetivo desse exercício é separar cada bloco de código em uma função e resolver o problema de reinicialização do jogo. Muito cuidado nesse exercício para realmente usar o mesmo código dentro das funções.

1) Envolva as variáveis frase, numPalavras e a inicicialização da tamanhoFrase dentro de uma função atualizaTamanhoFrase:
```javascript
function atualizaTamanhoFrase() {
    var frase = $(".frase").text();
    var numPalavras  = frase.split(" ").length;
    var tamanhoFrase = $("#tamanho-frase");
    tamanhoFrase.text(numPalavras);
}
```

2) Envolva o evento input do campo dentro de uma função inicializaContadores:
```javascript
function inicializaContadores() {
    campo.on("input", function() {
        var conteudo = campo.val();

        var qtdPalavras = conteudo.split(/\S+/).length - 1;
        $("#contador-palavras").text(qtdPalavras);

        var qtdCaracteres = conteudo.length;
        $("#contador-caracteres").text(qtdCaracteres);

    });
}
```

Cuidado, repare que a inicialização da variável campo não ficou nessa função!
3) Agora envolva a variável tempoRestante junto com o evento focus do campo dentro de uma função inicializaCronometro:
```javascript
function inicializaCronometro() {
    var tempoRestante = $("#tempo-digitacao").text();
    campo.one("focus", function() {
        var cronometroID = setInterval(function() {
            tempoRestante--;
            $("#tempo-digitacao").text(tempoRestante);
            if (tempoRestante < 1) {
                campo.attr("disabled", true);
                clearInterval(cronometroID);
            }
        }, 1000);
    });
}
```

4) O nosso nosso botão para reiniciar vai receber na função click o nome da função:

```javascript
$("#botao-reiniciar").click(reiniciaJogo);
```
Todo o código que estava dentro da função do evento click deve estar dentro da função reiniciaJogo:
```javascript
function reiniciaJogo(){
    campo.attr("disabled",false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
    $("#tempo-digitacao").text(tempoInicial);
    inicializaCronometro(); //novo
}
```

Repare que já estamos chamando a função inicializaCronometro dentro da função reiniciaJogo. 

5) Como agora todo nosso código está isolado dentro de funções, precisamos que alguém invoque estas funções para que elas sejam executadas! nções forem chamadas!
Para fazer isto, vamos utilizar uma função do jQuery que aguarda a página ser carregada e depois executa seu conteúdo: a função $(document).ready()
Para tal, adicione no ínicio da página logo após da declaração das variaveis já existentes:
```javascript
//as duas vars já devem existir
var campo = $(".campo-digitacao");
var tempoInicial = $("#tempo-digitacao").text();

//nova funcao
$(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();
    $("#botao-reiniciar").click(reiniciaJogo);
});

//outras funções omitidas
```
6) Salve e teste o seu código! 

Objetivo desse exercício foi organizar o nosso código em funções para deixar mais claro e mais reutilizável.
A refatoração valeu a pena no nosso código mas foi algo mais difícil de acompanhar, por isso estamos colocando o código do arquivo main.js para sua comparação:
```javascript
var campo = $(".campo-digitacao");
var tempoInicial = $("#tempo-digitacao").text();

$(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();
    $("#botao-reiniciar").click(reiniciaJogo);
});


function atualizaTamanhoFrase() {

    var frase = $(".frase").text();
    var numPalavras  = frase.split(" ").length;
    var tamanhoFrase = $("#tamanho-frase");
    tamanhoFrase.text(numPalavras);
}

function inicializaContadores() {

    campo.on("input", function() {
        var conteudo = campo.val();

        var qtdPalavras = conteudo.split(/\S+/).length - 1;
        $("#contador-palavras").text(qtdPalavras);

        var qtdCaracteres = conteudo.length;
        $("#contador-caracteres").text(qtdCaracteres);

    });
}

function inicializaCronometro() {

    var tempoRestante = $("#tempo-digitacao").text();
    campo.one("focus", function() {
        var cronometroID = setInterval(function() {
            tempoRestante--;
            $("#tempo-digitacao").text(tempoRestante);
            if (tempoRestante < 1) {
                campo.attr("disabled", true);
                clearInterval(cronometroID);
            }
        }, 1000);
    });
}

$("#botao-reiniciar").click(reiniciaJogo);

function reiniciaJogo(){
    campo.attr("disabled", false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");

    $("#tempo-digitacao").text(tempoInicial);
    inicializaCronometro();
}
```

### (Opcional) Desabilitando o botão na hora certa
O nosso botão reiniciar funciona corretamente, porém ele fica habilitado enquanto o usuário está jogando e o tempo passando, e caso ele clique no botão, o cronômetro irá tentar reiniciar e acontecerá um bug! Faça o teste aí.

Para resolver isto, podemos desabilitar o botão de reiniciar caso o usuário dê início ao jogo e o crônometro comece a descer, depois, ao fim do jogo, podemos reabilitar o botão novamente para o usuário poder reiniciá-lo.

Para desabilitar o botão, basta adicionar o atributo disabled nele, algo que já sabemos fazer. Dentro da função inicializaCronometro, no evento de focus:
```javascript
function inicializaCronometro() {
    var tempoRestante = $("#tempo-digitacao").text();
    campo.one("focus", function() {
        // Adicione aqui
        $("#botao-reiniciar").attr("disabled",true);
        ...
}
```

Assim quando o usuário começar a digitar o botão será desabilitado. Para reabilitá-lo ao fim do jogo vamos remover o atributo disabled na função inicializaCronometro, dentro do if que determina o fim do jogo:
```javascript
function inicializaCronometro() {
    ...
            if (tempoRestante < 1) {
                campo.attr("disabled", true);
                clearInterval(cronometroID);
                //Adicione aqui
                $("#botao-reiniciar").attr("disabled", false);
            }
    ...
}
```

Pronto, este é um modo de não deixar nossos usuários reiniciar o jogo no meio de uma digitação.



[Voltar ao Índice](#indice)

---

## <a name="parte5">5.Funções que auxiliam os estilos</a>

### Estilizando o jogo

O visual do nosso jogo ainda está bastante simples. Se formos olhar a versão completa do jogo:
 
Iremos perceber alguns detalhes, como botões estilizados, campo de digitação com o fundo cinza quando o mesmo estiver desabilitado, entre outros. Mas não estamos mexendo com CSS ainda, então é justamente isso que faremos aqui neste capítulo, utilizar o CSS para estilizar o nosso jogo.

Utilizaremos uma framework já pronta, pois o foco deste treinamento não é CSS, mas estilizaremos alguns pontos do nosso jogo com o auxílio do JavaScript, e obviamente do jQuery.

Adicionando alguns estilos ao nosso jogo

Dentro da pasta do projeto, public/css/libs, temos o arquivo materialize.min.css. O Materialize é uma framework front-end, assim como o Bootstrap, e nos auxiliará a estilizar o nosso jogo, evitando assim uma grande perda de tempo nessa tarefa.

Então vamos importá-lo na página principal.html, dentro da tag "head":

```html
<head>
    <meta charset="UTF-8">
    <title>Alura Typer</title>
    <link rel="stylesheet" href="css/libs/materialize.min.css">
</head>

```

Abra a página no navegador, e perceba já uma mudança significativa no layout da mesma:
 
Para estilizar ainda mais nossa página, vamos colocar todo o seu conteúdo do body (exceto os scripts) dentro de uma div com a classe container:
```html
<body>
    <div class="container">
        <!-- conteúdo da página aqui -->
    </div>

    <script src="js/jquery.js"></script>
    <script src="js/main.js"></script>
</body>
```

Com isso a nossa página fica alinhada no centro. Vamos centralizar também os contadores, o título e a frase, para isso adicionamos a classe center neles, mais precisamente nas duas uls da nossa página, no h1 e no p.

Após isso, vamos aumentar a altura do campo, alinhar a frase à esquerda, e aumentar as suas fontes. Coloque esse código dentro do arquivo public/css/estilos.css:
```css
.campo-digitacao {
    font-size: 20px;
    height: 130px;
}

.frase {
    font-size: 20px;
    text-align: left;
}
```

Por fim, não podemos esquecer de importar esse arquivo na página principal.html:
```html
<head>
    <meta charset="UTF-8">
    <title>Alura Typer</title>
    <link rel="stylesheet" href="css/libs/materialize.min.css">
    <link rel="stylesheet" href="css/estilos.css">
</head>
 
 ```

#### CSS com jQuery

Um outro ponto que podemos melhorar é o campo de digitação ficar com o fundo cinza quando o mesmo estiver desabilitado, quando o tempo se esgotar, para ficar bem claro para o usuário que ele não pode digitar no campo. E aí é que o jQuery nos auxilia, ele pode alterar o estilo de qualquer elemento.

No main.js, quando o tempo for menos que 1 (dentro da função inicializaCronometro), alteramos o CSS do campo utilizando a função css do jQuery, passando por parâmetro a propriedade CSS queremos modificar e o seu valor, separados por vírgula:
```javascript
if (tempoRestante < 1) {
    campo.attr("disabled", true);
    clearInterval(cronometroID);
    campo.css("background-color", "lightgray"); //novo
}
```

Agora ficou bem mais claro que o usuário não pode digitar, já que o jogo foi finalizado.

#### Alterando o CSS no JavaScript?

Mas se o designer do jogo decidir que não quer mais que a cor do fundo fique cinza, e sim azul, teremos que procurar no main.js onde estamos modificando o background-color do elemento e alterá-lo.

Nós sabemos que não é certo mexer com o estilo de uma página, de seus elementos, no JavaScript. Se queremos estilizar, logo devemos mexer nos arquivos .css. Então, o que podemos fazer é, ao invés de mexer diretamente com o CSS no JavaScript, adicionar uma classe. E no arquivo CSS nós estilizamos o campo através dessa classe.

Logo, no arquivo estilos.css, adicionamos:
```css
.campo-desativado {
    background-color: lightgray;
}
```

E no main.js, quando o tempo se esgotar, adicionamos essa classe campo-desativado no campo, através da função addClass:

```javascript
if (tempoRestante < 1) {
    campo.attr("disabled", true);
    clearInterval(cronometroID);
    campo.addClass("campo-desativado");
}
```


#### Adicionando ícones

O que está faltando agora no nosso jogo para realmente ficar parecido com o Alura Typer pronto são os ícones e botões coloridos que estão nele. Você pode ver como utilizar esses ícones aqui, no site no Materialize.
O primeiro passo é importar a fonte de ícones, nós podemos copiar o link que está no site, ou utilizar a fonte que já está no projeto, dentro da pasta public/css/libs. Vamos então importá-la dentro da tag "head", na página principal.html:
```html
<head>
    <meta charset="UTF-8">
    <title>Alura Typer</title>
    <link rel="stylesheet" href="css/libs/materialize.min.css">
    <link rel="stylesheet" href="css/libs/google-fonts.css">
    <link rel="stylesheet" href="css/estilos.css">
</head>
```

Agora, para utilizar os ícones, temos que adicionar uma tag "i" com as classes small (referente ao tamanho do ícone, há também os tamanhos tiny, small, medium e large) e material-icons. Dentro da tag nós colocamos o nome do ícone que queremos (a lista se encontra no site). Os ícones que utilizaremos para o contador do tamanho da frase e para o cronômetro são o description e query_builder, respectivamente.
Além disso, vamos deixar o nosso ul centraliado. Logo, nossa ul de informações ficará assim:

```html
<ul class="informacoes center">
    <li>
        <i class="small material-icons">description</i>
        <span id="tamanho-frase">5</span> palavras
    </li>
    <li>
        <i class="small material-icons">query_builder</i>
        <span id="tempo-digitacao">10</span> segundos
    </li>
</ul>
```

Falta deixar os ícones alinhados com o seu respectivo texto, para isso vamos adicionar a classe icones às duas tags "i" e adicionar o seguinte código no estilos.css:
```css
.icones {
    vertical-align: middle;
}
```

Para sua comparação segue o ul completo:
```html
<ul class="informacoes center">
    <li>
        <i class="small material-icons icones">description</i>
        <span id="tamanho-frase">5</span> palavras
    </li>
    <li>
        <i class="small material-icons icones">query_builder</i>
        <span id="tempo-digitacao">10</span> segundos
    </li>
</ul>
```

#### Botão de reinício de jogo mais agradável

O próximo passo agora é modificar o layout do botão de reinício de jogo. Para isso, o Materialize também nos auxilia, na página Buttons há uma série do opções para utilizarmos. Vamos utilizar o Floating, então vamos substituir o código do botão atual pelo código disponibilizado no site:
```html
<a class="btn-floating btn-large waves-effect waves-light red">
    <i class="material-icons">add</i>
</a>
```
Para terminar, vamos colocar o id do nosso antigo botão (botao-reiniciar) na tag "a" e utilizar um ícone mais expressivo, o restore:
```html
<a id="botao-reiniciar" class="btn-floating btn-large waves-effect waves-light red">
    <i class="material-icons">restore</i>
</a>
```

Como iremos ter mais botões futuramente, vamos colocar o nosso botão atual dentro de uma div com a classe botoes:
```html
<div class="botoes">
    <a id="botao-reiniciar" class="btn-floating btn-large waves-effect waves-light red">
        <i class="material-icons">restore</i>
    </a>
</div>
```


#### Adicionando e removendo classes facilmente de um elemento

Quando clicamos no botão, conseguimos digitar novamente no campo, mas o fundo do mesmo não fica branco, podendo deixar o usuário em dúvida se o jogo realmente foi reiniciado. Vamos deixar isso bem claro, deixando o fundo do campo em branco assim que o jogo for reiniciado.

Para deixar o fundo do campo cinza, nós adicionamos a classe campo-desativado no campo, assim que o tempo se esgotar. E no CSS nós pintamos o fundo do campo que contiver esta classe. Então para remover o fundo, basta nós removermos a classe do campo quando o jogo for reiniciado.

Assim como o jQuery possui a função addClass, ele também possui a removeClass, logo, no main.js, adicionamos:

```javascript
function reiniciaJogo() {
    campo.attr("disabled", false);
    campo.val("");
    $("#contador-palavras").text(0);
    $("#contador-caracteres").text(0);
    $("#tempo-digitacao").text(tempoInicial);
    inicializaCronometro();
    campo.removeClass("campo-desativado");
}
```

Essa ação de adicionar e remover classes se tornou uma tarefa tão comum, que o jQuery criou uma função específica para isso, a toggleClass. Ela funciona da seguinte maneira, se no momento que a função for chamada, o elemento possuir a classe, ela será removida. Mas se o elemento não possuir a classe, ela será adicionada. Exatamente o que precisamos!

Então vamos utilizar esta função no lugar de ambas as funções, addClass e removeClass:
```javascript
function reiniciaJogo() {
    campo.attr("disabled", false);
    campo.val("");
    $("#contador-palavras").text(0);
    $("#contador-caracteres").text(0);
    $("#tempo-digitacao").text(tempoInicial);
    inicializaCronometro();
    campo.toggleClass("campo-desativado");
}
```

E dentro da função inicializaCronometro():
```javascript
if (tempoRestante < 1) {
    campo.attr("disabled", true);
    clearInterval(cronometroID);
    campo.toggleClass("campo-desativado");
}
```

#### Marcação da borda

O nosso aplicativo Alura Typer já está ganhando forma mas ainda há pontos a melhorar. Algo que ainda falta é uma verificação visual se o usuário realmente acerta o texto a digitar. Queremos que o jogador perceba facilmente onde errou no texto.

A nossa ideia é a seguinte: enquanto o jogador acerta as letras mostraremos uma borda verde no campo de digitação. Assim que errou uma letra alteraremos a borda para a cor vermelha. Assim o jogador percebe na hora que errou algo, ok?

#### Evento input
Para comparar o texto digitado com a frase proposta devemos associar o evento input que ao nosso elemento campo. Já aprendemos isso nas aulas anteriores, basta usar a função on do jquery.

Dentro do main.js, ainda solto e fora de qualquer outra função vamos pegar a frase pelo seletor de classe do elemento e adicionar o evento ao campo:
```javascript
var frase = $(".frase").text();
campo.on("input", function() {
    console.log(frase);
});
```

Ao testar no navegador já deveria aparecer a frase completa enquanto estamos escrevendo.

Dentro da função anônima vamos capturar o texto digitado, basta usar a função val() do campo:
```javascript
var frase = $(".frase").text();
campo.on("input", function() {
    var digitado = campo.val();
    console.log(frase);
    console.log(digitado);
});
```

#### Comparando o texto digitado

Agora já sabemos qual é a frase e o que o jogador digitou. Falta verificar se o texto digitado realmente faz parte da frase para saber se o jogador errou ou não.
Repare que não podemos usar a condição digitado == frase pois isso verificaria sempre a frase inteira com o valor digitado. Mesmo se o jogador tenha escrito apenas uma palavra, o jogo consideraria errado pois estaria comparando com a frase inteira, mesmo que o jogador esteja no caminho certo e não tenha errado nada ainda. 
Então para saber se o jogador está certo ou não, vamos pegar apenas a parte inicial da frase que possui a mesma quantidade do valor digitado. Isso pode ser feito pela função substr (sub-string):

```javascript
var comparavel = frase.substr(0 , digitado.length);
```

A função substr devolve uma outra string com o tamanho definido nos parâmetros. O primeiro parâmetro é o inicio, aqui 0, ou seja, sempre a partir do primeiro char. O segundo define o fim que é justamente o tamanho do valor digitado. 

Assim podemos realmente comparar o valor digitado com a substring correta da frase:
```javascript
if(digitado == comparavel) {
    console.log("Está certo");
} else {
    console.log("Está errado");
}
```

Agora tudo dentro do evento:
```javascript
var frase = $(".frase").text();
campo.on("input", function() {
    var digitado = campo.val();
    var comparavel = frase.substr(0 , digitado.length);

    if(digitado == comparavel) {
        console.log("Está certo");
    } else {
        console.log("Está errado");
    }
});
```


#### Melhorando o feedback

Ótimo, já está funcionando mas apenas olhando no console percebemos se erramos ou acertamos. Vamos melhorar agora o feedback para o usuário mostrando uma borda verde ou vermelha, respectivamente.

O primeiro passo é adicionar duas classes que representam a borda verde ou vermelha no nosso arquivo estilo.css:
```css
.borda-verde {
    border: 3px solid green;
}

.borda-vermelha {
    border: 3px solid red;
}
```

Agora só falta adicionar a classe programaticamente no evento dentro do nosso if:
```javascript
var frase = $(".frase").text();
campo.on("input", function() {
    var digitado = campo.val();
    var comparavel = frase.substr(0 , digitado.length);

    if(digitado == comparavel) {
        campo.addClass("borda-verde");
    } else {
        campo.addClass("borda-vermelha");
    }
});
```

#### Removendo a classe

Ao testar já aparece a borda verde como esperado e se errarmos se torna vermelha, mas ainda tem um probleminha. Se corrigimos o texto digitado, a borda não volta para a cor verde, e sim continua vermelha. Isto é pois sempre adicionarmos a classe no campo. Uma vez adicionado ela continua lá e consequentemente continua vermelho ou verde, dependendo da última classe adicionada.

Para resolver basta remover a outra classe dentro do if:
```javascript
var frase = $(".frase").text();
campo.on("input", function() {
    var digitado = campo.val();
    var comparavel = frase.substr(0 , digitado.length);

    if(digitado == comparavel) {
        campo.addClass("borda-verde");
        campo.removeClass("borda-vermelha");
    } else {
        campo.addClass("borda-vermelha");
        campo.removeClass("borda-verde");
    }
});
```

Novamente vamos testar no navegador e a troca de cores funciona perfeitamente.

#### Encapsulando o código

Vamos seguir as boas práticas e isolar o código JavaScript dentro de uma função para não ficar solto dentro do arquivo main.js. Chamaremos a função de inicializaMarcadores
```javascript
function inicializaMarcadores() {
    var frase = $(".frase").text();
    campo.on("input", function() {
        var digitado = campo.val();
        var comparavel = frase.substr(0 , digitado.length);

        if(digitado == comparavel) {
            campo.addClass("borda-verde");
            campo.removeClass("borda-vermelha");
        } else {
            campo.addClass("borda-vermelha");
            campo.removeClass("borda-verde");
        }
    });
}
```

E assim podemos adicionar essa função inicializaMarcadores na função que é chamada ao carregar a página:
```javascript
$(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();
    inicializaMarcadores(); //novo
    $("#botao-reiniciar").click(reiniciaJogo);
});
```

#### Inicializando sem cor

A marcação da borda já funciona mas ainda podemos melhorar um detalhe. Ao jogar e reinicializar o jogo através de nosso botão, percebemos que a borda continua pintada e não volta ao estado inicial. Faz todo sentido começar com uma borda preta, e a cor vir apenas quando realmente começamos a digitar. 
Para reiniciar o jogo corretamente basta remover as classe de borda do campo na função reiniciaJogo:
```javascript
function reiniciaJogo(){
    campo.attr("disabled",false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
    $("#tempo-digitacao").text(tempoInicial);
    inicializaCronometro();
    campo.toggleClass("campo-desativado");

    campo.removeClass("borda-vermelha"); //novo
    campo.removeClass("borda-verde"); //novo
}
```

### O que é CSS?

HTML é usado para estruturar conteúdos da página, o CSS para formatar conteúdos estruturados.
CSS é uma linguagem para estilos que define o layout de documentos HTML. Por exemplo, CSS controla fontes, cores, margens, linhas, alturas, larguras, imagens de fundo, posicionamentos e muito mais. 


### Mãos na massa: Aplicando CSS

#### Melhorando o visual
O visual do nosso jogo ainda está bastante simples razão suficiente para aplicar um CSS, não? Como você viu no video usaremos o framework Materialize para estilizar a página que auxilia muito nessa tarefa. 
Para tal:

1) Abra o arquivo principal.html e adicione dentro do <head> logo abaixo da tag <title>:

```html
<link rel="stylesheet" href="css/libs/materialize.min.css">
```
Recarregue a página dentro do navegador e repare a diferença. Para sua comparação o <head> inteiro ficou como:
```html
<head>
    <meta charset="UTF-8">
    <title>Alura Typer</title>
    <link rel="stylesheet" href="css/libs/materialize.min.css"> <!-- novo -->
</head>
```

Obs: O arquivo materialize.min.css já está dentro da pasta public/css/libs do seu projeto.

2) Agora, na mesma página principal.html, coloque todo o conteúdo do body (exceto os scripts) dentro de uma div com a classe container. Adicione apenas o div:
```html
<body>
    <div class="container">
        <!-- conteúdo da página aqui -->
    </div>

    <script src="js/jquery.js"></script>
    <script src="js/main.js"></script>
</body>
```

Novamente, recarregue a página no navegador para ver a diferença

3) Após isso, vamos aumentar a altura do campo, alinhar a frase à esquerda, e aumentar as suas fontes. Abre o arquivo public/css/estilos.css e coloque esse código abaixo:
```css
.campo-digitacao {
    font-size: 20px;
    height: 130px;
}

.frase {
    font-size: 20px;
    text-align: left;
}
```
4) No arquivo principal.html importe o estilo.css dentro da tag <head>:
```html
<head>
    <meta charset="UTF-8">
    <title>Alura Typer</title>
    <link rel="stylesheet" href="css/libs/materialize.min.css"> 
    <link rel="stylesheet" href="css/estilos.css"> <!-- novo -->
</head>
```

5) Para deixar mais claro que o jogo terminou, deixe o campo de digitação cinza quando o tempo esgotar. Dentro do arquivo public/css/estilo.css adiciona uma nova clase:
```css
.campo-desativado {
    background-color: lightgray;
}
```

6) No arquivo main.js, quando o tempo se esgotar, devemos adicionar essa classe campo-desativado ao campo usando jQuery. Quando o usuário clicar no botão reiniciar, o campo deveria ser reativado. Para não espalhar as funções addClass e removeClass do jQuery, vamos aproveitar a função toggleClass que ativa e desativa respectivamente.
Abra o arquivo main.js e procure a função inicializaCronometro:
```javascript
//dentro do arquivo main.js, dentro da função inicializaCronometro

//dentro desse if adicione apenas a linha com toggleClass
if (tempoRestante < 1) {
    campo.attr("disabled", true);
    clearInterval(cronometroID);
    campo.toggleClass("campo-desativado"); //novo
}
//Adicione a mesma funcionalidade no final da função reiniciaJogo:
function reiniciaJogo() {
    //código omitido e não alterado
    campo.toggleClass("campo-desativado"); //novo
}
```
7) Salve os arquivo e teste no navegador. Após o tempo esgotar, o campo de digitação deve ficar cinza. Ao reiniciar volta a ser ativado.
 

#### Mãos na massa: Usando ícones
O próximo passo é usar os ícones e colorir mais a página. Vamos aproveitar o framework materialize para essa tarefa.
1) O primeiro passo é importar a fonte de ícones. Abra a página principal.html e adicione na tag "head" mais um estilo:
```html
<head>
    <meta charset="UTF-8">
    <title>Alura Typer</title>
    <link rel="stylesheet" href="css/libs/materialize.min.css">
    <link rel="stylesheet" href="css/libs/google-fonts.css"> <!-- novo --> 
    <link rel="stylesheet" href="css/estilos.css"> 
</head>
```

2) Agora podemos aproveitar os ícones do framework Materialize. Vamos mostrar um ícone para o item palavras e tempo. No mesmo arquivo principal.html procure a tag ul que possui a classe informacoes. Nele adicione a classe center, e em cada elemento li uma nova tag para carregar o ícone:
```html
<ul class="informacoes center">
    <li>
        <i class="small material-icons icones">description</i>
        <span id="tamanho-frase">5</span> palavras
    </li>
    <li>
        <i class="small material-icons icones">query_builder</i>
        <span id="tempo-digitacao">10</span> segundos
    </li>
</ul>
```
Obs: Você pode ver como utilizar esses ícones no site do Materialize.
3) Repare que usamos a classe icones dentro da tag i. Essa classe não existe e deve ser adicionado no nosso arquivo estilos.css para centralizar o texto com os ícones.
Adicione no arquivo estilos.css a classe seguinte:
```css
.icones {
    vertical-align: middle;
}
```
4) Recarregue a página no navegador. O resultado deve ser parecido com a imagem abaixo:
 

#### Mãos na massa: Verificando a digitação

Como apresentado no video vamos marcar a borda do campo de digitação para sinalizar se o usuário errou ou acertou.
1) No arquivo main.js adicione uma nova função inicializaMarcadores. Nela já recupera a frase através do jQuery e associe o evento input com o campo:
```javascript
function inicializaMarcadores() {

    var frase = $(".frase").text();
    campo.on("input", function() {
        //aqui vem mais
    });
}
```
2) Dentro da função anônima do evento pegue o valor do campo e gere uma substring baseado no tamanho dele. Guarde o substring dentro de uma nova variável:
```javascript
var digitado = campo.val();
var comparavel = frase.substr(0 , digitado.length);
```
3) Logo após da variável comparavel teste se ela é igual ao texto digitado. Se for igual, adicione a classe borda-verde e remove borda-vermelha. No bloco else faça o inverso:
```javascript
if(digitado == comparavel) {
    campo.addClass("borda-verde");
    campo.removeClass("borda-vermelha");
} else {
    campo.addClass("borda-vermelha");
    campo.removeClass("borda-verde");
}
```
4) Procure a função que é chamada ao carregar a página no início do arquivo main.js. Nela adiciona a chamada da função inicializaMarcadores: 
```javascript
$(function(){
    atualizaTamanhoFrase();
    inicializaContadores();
    inicializaCronometro();

    inicializaMarcadores(); //novo

    $("#botao-reiniciar").click(reiniciaJogo);
});
```
5) As classes borda-verde e borda-vermelha não exisem ainda. Abra o arquivo estilos.css e adicione:
```css
.borda-verde {
    border: 3px solid green;
}

.borda-vermelha {
    border: 3px solid red;
}
```
6) Vamos inicializar o jogo sempre sem marcação da borda. Para isso volte ao arquivo main.js e procure a função reiniciaJogo. No final dela adicione:
```javascript
function reiniciaJogo(){
    campo.attr("disabled",false);
    campo.val("");
    $("#contador-palavras").text("0");
    $("#contador-caracteres").text("0");
    $("#tempo-digitacao").text(tempoInicial);
    inicializaCronometro();
    campo.toggleClass("campo-desativado");

    campo.removeClass("borda-vermelha"); //novo
    campo.removeClass("borda-verde"); //novo
}
```
7) Salve os seus arquivos e teste a marcação da borda!



#### Mãos na massa: Verificando a digitação
 
Para sua comparação segue uma vez o código completo da função inicializaMarcadores:
```javascript
function inicializaMarcadores() {
    var frase = $(".frase").text();
    campo.on("input", function() {
        var digitado = campo.val();
        var comparavel = frase.substr(0 , digitado.length);

        if(digitado == comparavel) {
            campo.addClass("borda-verde");
            campo.removeClass("borda-vermelha");
        } else {
            campo.addClass("borda-vermelha");
            campo.removeClass("borda-verde");
        }
    });
}
```

No nosso projeto foi necessário pegar uma parte da frase para comparar a string com aquilo que foi digitado pelo usuário. Lembrando rapidamente do código:
```javascript
var comparavel = frase.substr(0 , digitado.length);
```
Usamos a função substr para pegar o uma parte da frase, aqui do início (índice 0) até o tamanho da string digitado. Baseado nessa substring comparavel testamos se o conteúdo digitado bate com a frase:
```javascript
if(digitado == comparavel) {
 campo.addClass("borda-verde");
} else {
 campo.addClass("borda-vermelha");
}
```

Como o JavaScript está evoluindo e melhorando já existe uma forma mais fácil de verificar se uma string faz parte da outra string. Se o seu navegador já dar suporte ao ECMA Script 6 você pode simplesmente executar:

```javascript

 var digitouCorreto = frase.startsWith(digitado);
if(digitouCorreto) {
 campo.addClass("borda-verde");
} else {
 campo.addClass("borda-vermelha");
}
```

Ainda mais enxuto:

```javascript
if( frase.startsWith(digitado)) {
 campo.addClass("borda-verde");
} else {
 campo.addClass("borda-vermelha");
}
``` 
A função startsWith devolve true ou false, se a frase começa com o valor digitado ou não. Teste isso agora no console, digitando por exemplo:

```javascript

"ECMA Script 6".startsWith("ECMA")
```
#### Para saber mais: Materialize e Bootstrap
O Materialize é uma framework front-end que auxilia muito a estilizar páginas, evitando assim uma grande perda de tempo nessa tarefa. É útil para quem gostaria de seguir boas práticas no mundo CSS para por exemplo criar uma página responsiva sem entrar em detalhes:

http://materializecss.com/

O Materialize foi criado pela Google e segue o Material Design que é uma linguagem de design desenvolvida pela Google. Material Design é útilizado em vários produtos do Google e também é aplicado nos aplicativos Android.

Outro framework famoso nessa linha é o Bootstrap. Para ser correto o Bootstrap é o framework mais famoso para estilizar páginas:
http://getbootstrap.com/




[Voltar ao Índice](#indice)

---

## <a name="parte6">6.Criando e manipulando elementos com jQuery</a>

### Salvando a pontuação no placar

#### Criando o placar
Neste capítulo queremos que a pontuação do usuário seja salva ao final de cada jogada dele. Para isto, vamos montar um placar: Uma pequena tabela que deve ficar na parte de baixo da nossa aplicação, que salvará o número de palavras digitadas e o nome do usuário a cada jogada dele.

Primeiramente, vamos montar a estrutura HTML necessária para comportar o placar, montando uma "section" e dentro dele colocando uma tabela que terá o nome do usuário e número de palavras digitadas.
```html
<section class="placar">
    <h3>Placar</h3>
    <table>
        <thead>
            <tr>
                <th>Usuário</th>
                <th>No. de palavras</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Usuario Exemplo</td>
                <td>99</td>
            </tr>
        </tbody>
    </table>
</section>
```
Vamos aproveitar e colocar algumas classes da nossa framework frontend para que a tabela tenha algum estilo:
```html
<section class="placar">
    <h3 class="center">Placar</h3>
    <table class="centered bordered">
        <thead>
            <tr>
                <th>Usuário</th>
                <th>No. de palavras</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Usuario Exemplo</td>
                <td>99</td>
            </tr>
        </tbody>
    </table>
</section>
```
Com a estrutura da tabela montada, podemos partir para o Javascript, aonde criaremos a função responsável de inserir no placar. Em seu main.js crie a função inserePlacar:
```javascript
//main.js

function inserePlacar(){
    console.log("Linha inserida no placar");    
}
```

Devemos chamar esta função ao término do nosso jogo, ou seja, quando o tempo chegar a zero. Sabemos exatamente aonde isto acontece, na função inicializaCronometro, em seu if:
```javascript
//main.js
// Restante do código
if(tempoRestante < 1){
    clearInterval(cronometroID);
    campo.attr("disabled",true);
    campo.toggleClass("campo-desativado");
    inserePlacar();
}
```

#### Buscando nos filhos com jQuery

Na função inserePlacar(), precisamos buscar pelo corpo da tabela, que é de fato aonde queremos inserir novas linhas com a pontuação do usuário. Vamos primeiro selecionar a section placar inteira:
```javascript
//main.js

function inserePlacar(){
    var placar = $(".placar");
}
```

Em seguida, queremos obter o tbody que fica dentro da "table", que por sua vez está dentro da "section". Quando queremos buscar filhos de um elemento que já selecionamos previamente, podemos utilizar a função .find() do jQuery, que funciona de modo semelhante a função seletora ($), porém fazendo a busca apenas do filho do elemento:
```javascript
//main.js

function inserePlacar(){
    var placar = $(".placar");
    var corpoTabela = placar.find("tbody");
}
```
A função .find() recebe como parâmetro seletores CSS, e busca em seus filhos algum elemento que atenda aquela busca. Podemos simplificar e fazer tudo em uma linha apenas:
```javascript
//main.js

function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
}
```

#### Criando uma nova linha

Como queremos criar uma nova linha na tabela, com o nome do usuário e o número de palavras, precisamos pegar essas informações:

```javascript
//main.js

function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();
}
```

Com os dados obtidos, vamos dar inicio a criação da nossa linha, que deve ser um "tr" com dois "td" dentro , cada um com uma informação. Vamos começar a criando esta estrutura como uma string:
```javascript
//main.js

function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();

    var linha = "<tr>"+
                    "<td>"+ usuario + "</td>"+
                    "<td>"+ numPalavras + "</td>"+
                "</tr>";
}
```
Repare que concatenamos com pedaços da string com o nossas variáveis, que continham os dados, pois nosso objetivo final é ter algo assim:
```html
<tr>
    <td>Douglas</td>
    <td>99</td>
</tr>
```

#### Adicionando HTML na página com jQuery

Com nossa linha criada, precisamos adicioná-la ao corpo da tabela, e para isto vamos utilizar a função .append() do jQuery. Esta função adiciona a string ou elemento HTML que é passada como parâmetro como último filho do elemento em qual ela for chamada.
Vamos a linha como última filha do tbody:

```javascript
//main.js

function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();

    var linha = "<tr>"+
                    "<td>"+ usuario + "</td>"+
                    "<td>"+ numPalavras + "</td>"+
                "</tr>";

    corpoTabela.append(linha);
}
```

Agora, ao final do jogo, uma nova linha é criada e adicionada ao corpo da tabela, contendo o nome do usuário e número de palavras.
Adicionando como primeiro item

Se quisermos adicionar a nova linha como primeiro item da tabela, devemos utilizar uma função que é prima da função .append(), que é a .prepend(). Ela adiciona a string/HTML passada como primeiro filho do elemento selecionado:
```javascript
//main.js

function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();

    var linha = "<tr>"+
                    "<td>"+ usuario + "</td>"+
                    "<td>"+ numPalavras + "</td>"+
                "</tr>";

    corpoTabela.prepend(linha);
}
```

Assim o placar mais recente do usuário aparece como primeiro item da lista.


### Criando um botão remover

Agora que estamos conseguindo adicionar item a nossa tabela placar, também precisamos dar a opção do usuário de remover alguma das linhas que ele desejar.
Para isto, vamos adicionar um pequeno botão de remover em cada linha da tabela, como uma terceira coluna. Ele será um link representado por um icone de lixeira , que pegaremos do framework que estamos utilizando para estilizar. Vamos adiciona-lo dentro de um "td", como uma nova coluna da tabela:

```html
<tr>
    <td>Padrao</td>
    <td>999</td>
    <td>
        <a href="#">
            <i class="small material-icons">delete</i>
        </a>
    </td>    
</tr>
```
Mas deixando-o estático, ele irá aparecer apenas nas pontuações que já vem no principal.html. Vamos alterar a nossa função inserePlaca() para adicionar um botão de remoção na linha também:
```javascript
function inserePlacar() {
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Douglas"
    var numPalavras = $("#contador-palavras").text();
    var botaoRemover = "<a href='#'><i class='small material-icons'>delete</i></a>" ;

    var linha = "<tr>"+
                    "<td>"+ usuario + "</td>"+
                    "<td>"+ numPalavras + "</td>"+
                    "<td>"+ botaoRemover + "</td>"+
                "</tr>";

    corpoTabela.append(linha);
}
```

Primeiro criamos o botão com uma string, depois adicionamos-o como uma terceira linha da coluna.
Com o botão aparecendo um nossa página tanto nas linhas que já vem no placar quanto as que são criadas no fim do jogo, vamos começar a adicionar um evento de click em nossos botões:
Primeiramente, vamos adicionar uma classe à tag "a":
```html
<a href="#" class="botao-remover">
    <i class="small material-icons">delete</i>
</a>
```

E vamos adicionar um evento de click no main.js:
```javascript
$(".botao-remover").click(function(){
    console.log("Fui clicado");
})
```

#### Prevenindo o salto da tela

Repare que ao clicar no icone de remoção, além de exibir a mensagem no console a página salta para o topo. Isso acontece pois quando clicamos em uma tag "a" ela tem o comportamento de redirecionar para o que estiver em seu atributo href, seja um link ou um ID de um elemento HTML. Neste caso, estamos com o valor de "#" no href, o que faz com que seja redirecionado pro topo da página. Se o href fosse o id de algum elemento, a visualização iria saltar para este elemento.
Este é um comportamento padrão da tag "a", mas neste caso , queremos evita-lo. Conseguimos fazer isto através da função preventDefault(). Vamos alterar nosso evento para receber um parâmetro que permite usa-la:
```javascript
$(".botao-remover").click(function(event){
    event.preventDefault();
    console.log("Fui clicado");
})
```

Experimente clicar no botão agora, você verá que apenas a mensagem é exibida e a tela parou de saltar.
#### Removendo a linha

Agora que estamos detectando o evento de click, partiremos para a remoção da linha. Pare remover um elemento do HTML , podemos utiliza a função com nome semelhante do jQuery, a .remove().

Se no nosso evento de click, utilizarmos ela para remover quem foi clicado, que pode ser acessado através do this:
```javascript
$(".botao-remover").click(event, function(){
    this.remove();
})
```

Vamos obter um erro clássico de quando estamos trabalhando com jQuery. Tentamos utilizar uma função do jQuery em um elemento do HTML. Elementos comuns do HTML não tem acesso as funções do jQuery, precisamos empoderá-los com as funções do objeto jQuery, envolvendo-os com a função jQuery:

```javascript
$(".botao-remover").click(event, function(){
    $(this).remore();
})
```

Deste modo o this (elemento HTML que foi clicado), ganha acesso as várias funções do jQuery, como .text(),.val(), .css() e todas as outras funções do jQuery.
Só que o código acima não resolve nosso problema, se você clicou no botão remover, você vai ver que apenas o icone de lixeira sumiu! O linha com a pontuação do usuário continua lá. Isto acontece pois estamos chamando a função .remove() na tag "a", quem é quem foi clicada!
O que nós desejamos é clicar na tag "a" e remover a linha inteira, que é a "tr"! Só que a "tr" é um elemento acima da tag no HTML , veja:
```html
<tr>
    <td>Padrao</td>
    <td>999</td>
    <td>
        <a href="#">
            <i class="small material-icons">delete</i>
        </a>
    </td>    
</tr>
```

O elemento pai da "a" é uma "td" , e a linha é o elemento dois níveis acima, ou seja , a "tr". Para acessarmos um elemento acima do elemento selecionado com jQuery, um elemento pai, temos a função .parent() do Javascript, veja:

```javascript
$(".botao-remover").click(){
    $(this).parent().remove();
}
```

O elemento $(this).parent() é o "td", como queremos remover a linha inteira, que é o "tr", vamos subir mais um nível da na árvore do HTML utilizando a função .parent() duas vezes:
```javascript
$(".botao-remover").click(){
    $(this).parent().parent().remove();
}
```

Agora sim nossa linha é removida corretamente quando clicamos no tag "a"!

### Adicionando eventos nas linhas do placar

#### Criando uma linha removível

Apesar de já conseguirmos remover uma linha que já vem por padrão no placar, a remoção ainda não funciona para as linhas que são geradas ao término de cada jogo. Isso se dá por que não atrelamos o evento de remoção depois de adicionar a linha ao placar. E nem conseguimos fazer isto, pois a nossa linha é apenas uma string antes de ser adicionada no HTML. Só conseguimos atrelar eventos à elementos!

#### Criando um <tr> dentro do Javascript

Por isso, vamos mudar o modo de criação da linha e vamos criar um elemento HTML, que será nossa linha, dentro do Javascript antes de colocá-la no placar.
Vamos criar uma função chamada novaLinha():
```javascript
function novaLinha(){

}
```

E vamos chamá-la na dentro da função inserePlacar(), no local de criação da linha antiga:
```javascript
function inserePlacar() {
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Douglas"
    var numPalavras = $("#contador-palavras").text();
    var botaoRemover = "<a href='#'><i class='small material-icons'>delete</i></a>" ;

    var linha = novaLinha();

    corpoTabela.append(linha);
}
```

Na função novaLinha() nosso objetivo será criar um elemento HTML em si, não apenas uma string, e para isto vamos utilizar a função jQuery $(), só que ao invés de passarmos um seletor, como fazemos por padrão, vamos passar a tag HTML que queremos criar. Veja:
```javascript
function novaLinha(){
    var linha = $("<tr>");
}
```

Assim a variável linha será de fato um! Como se estivéssemos selecionado no HTML! 

Isso irá nos permitir criar cada elemento da linha individualmente, depois juntá-los, atrelar o evento de remoção e aí sim coloca-lo no HTML.
Vamos criar nossas colunas, primeiro a coluna de usuário, que será um "td" que tem como texto o nome do usuário.
```javascript
function novaLinha(){
    var linha = $("<tr>");
    var colunaUsuario = $("<td>");
}
```

Como não temos o nome do usuário nem o número de palavras nesta função, vamos recebê-los como parâmetros da função e passá-los na inserePlacar():
```javascript
function inserePlacar(){
    ...
    var usuario = "Douglas"
    var numPalavras = $("#contador-palavras").text();
    var botaoRemover = "<a href='#'><i class='small material-icons'>delete</i></a>" ;

    var linha = novaLinha(usuario,numPalavras);
    ...
}

function novaLinha(usuario,palavras){
    var linha = $("<tr>");
    var colunaUsuario = $("<td>");
}
```

Agora com estas informações disponíveis na função novaLinha(), podemos criar as duas colunas com os textos apropriados dentro:
```javascript
function novaLinha(usuario,palavras){
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
}
```

A última parte que temos que montar da nossa linha é o ícone de remoção, que possuí o seguinte HTML:
```html
<td>
    <a href="#">
        <i class="small material-icons">delete</i>
    </a>
</td>
```

Vamos começar a criar estes elementos com jQuery:

```javascript
function novaLinha(usuario,palavras){
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
    var colunaRemover = $("<td>");

    var link = $("<a>").attr("href","#");
    var icone = $("<i>").addClass("small").addClass("material-icons").text("delete");
}
```
Aqui utilizamos diversas funções do jQuery que já conhecemos para montar os elementos iguais a sua estrutura original do HTML.
Agora basta posiciona-los corretamente com a função append():
```javascript
function novaLinha(usuario,palavras){
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
    var colunaRemover = $("<td>");

    var link = $("<a>").attr("href","#");
    var icone = $("<i>").addClass("small").addClass("material-icons").text("delete");

    // Icone dentro do <a>
    link.append(icone);

    // <a> dentro do <td>
    colunaRemover.append(link);

    // Os três <td> dentro do <tr>
    linha.append(colunaUsuario);
    linha.append(colunaPalavras);
    linha.append(colunaRemover);
}
```
Por último, vamos retornar a linha que foi criada pela nossa função:
```javascript
function novaLinha(usuario,palavras){
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
    var colunaRemover = $("<td>");

    var link = $("<a>").attr("href","#");
    var icone = $("<i>").addClass("small").addClass("material-icons").text("delete");

    link.append(icone);

    colunaRemover.append(link);

    linha.append(colunaUsuario);
    linha.append(colunaPalavras);
    linha.append(colunaRemover);

    return linha;
}
```

#### Adicionando o evento de remoção na linha recém criada:
Agora que nossa função inserePlacar() tem acesso a um elemento do HTML, podemos finalmente atrelar o evento de click ao botão que fica dentro da linha. Vamos primeiro exportar nossa função de remoção para uma linha genérica:
```javascript
function removeLinha(event){
    event.preventDefault();
    $(this).parent().parent().remove();
}
```
E chamar a função removeLinha para os botoes que estão dentro das linhas criadas. Como agora temos um elemento HTML, podemos utilizar o .find() para acha-los:

```javascript
function inserePlacar() {
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Douglas"
    var numPalavras = $("#contador-palavras").text();
    var botaoRemover = "<a href='#'><i class='small material-icons'>delete</i></a>" ;

    var linha = novaLinha(usuario,numPalavras);
    linha.find(".botao-remover").click(removeLinha);

    corpoTabela.append(linha);
}
```
Agora nossas linhas geradas pelo jogo podem ser deletadas normalmente! Podemos até mesmo remover as linhas que já vinham por padrão no nosso placar, deixando apenas as que foram geradas pela usuário!

### Organizando o código da aplicação

#### Quebrando o código em diferentes arquivos

Com o aprimoramento do nosso projeto, o nosso main.js cresceu razoavelmente e se continuarmos nesse ritmo, ao final da aplicação teremos um arquivo com mais de 300 linhas de código, o que sabemos que não é uma boa prática.
Vamos dividir um pouco este arquivo, em diversos arquivos .js menores, aonde cada arquivo será responsável por um área de nossa aplicação.

#### As funções do placar

Vamos criar o arquivo placar.js na pasta /js e importá-lo em principal.html:
```html
    <script src="js/jquery.js"></script>
    <script src="js/materialize-min.js"></script>
    <script src="js/main.js"></script>
    <script src="js/placar.js"></script>
```

Mova as funções inserePlacar(), novaLinha() e removeLinha() para o placar.js e teste se sua aplicação continua funcionando como antes.

#### Código separado

Daqui para frente, cada parte do nosso código ficará em um arquivo próprio, melhorando a organização de nossa aplicação!


### Salvando a pontuação do usuário

Para salvar a pontuação do usuário no final de cada jogada dele, precisamos primeiramente criar um placar. Para isso, no final da página principal.html, vamos adicionar uma tabela:
```html
<section class="placar">
    <h3 class="center">Placar</h3>
        <table class="centered bordered">
            <thead>
                <tr>
                    <th>Usuário</th>
                    <th>No. de palavras</th>
                </tr>
            </thead>
        <tbody>
            <tr>
                <td>Usuario Exemplo</td>
                <td>99</td>
            </tr>
        </tbody>
    </table>
</section>
```

Finalizada a estrutura do placar, podemos partir para o código JavaScript. No main.js, vamos criar a função inserePlacar() e acessar o nosso placar:
```javascript
function inserePlacar() {
    var placar = $(".placar");
}
```

Mas devemos inserir a pontuação no tbody, vamos então obtê-lo. Como tbody é um elemento filho do nosso placar, vamos utilizar a função find do jQuery, que funciona de modo semelhante a função seletora ($), porém fazendo a busca apenas do filho do elemento:
```javascript
function inserePlacar() {
    var placar = $(".placar");
    var corpoTabela = placar.find("tbody");
}
```

Vamos simplificar fazendo tudo em uma linha e como queremos criar uma nova linha na tabela, com o nome do usuário e o número de palavras, vamos pegar essas informações:
```javascript
function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();
}
```

Precisamos agora inserir uma linha na tabela com esses dados, mas vamos realizar isso em uma função separada:
```javascript
function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();

    var linha = novaLinha();
}

function novaLinha() {

}
```

Na função novaLinha() precisamos criar um elemento HTML, e para isto vamos utilizar a função jQuery $(), só que ao invés de passarmos um seletor, vamos passar a tag HTML que queremos criar:
```javascript
function novaLinha() {
    var linha = $("<tr>");
}
```

Assim a variável linha será de fato um "tr", como se estivéssemos acabado de selecionar um no HTML. Vamos montar o resto da tabela com as informações do usuário e o placar, mas como não temos essas informações na função, vamos recebê-las por paramêtro:
```javascript
function inserePlacar(){
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();

    var linha = novaLinha(usuario, numPalavras);
}

function novaLinha(usuario, palavras) {
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
}
```

Com tudo pronto, precisamos adicionar os elementos HTML corretamente dentro da linha da tabela, para isso vamos utilizar a função append. Ela adiciona a string ou elemento HTML que é passada como parâmetro como último filho do elemento em qual for chamada:
```javascript
function novaLinha(usuario, palavras) {
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);

    // Os dois <td> dentro do <tr>
    linha.append(colunaUsuario);
    linha.append(colunaPalavras);
}
```

E por último, vamos retornar a linha que foi criada pela nossa função:
```javascript
function novaLinha(usuario, palavras) {
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);

    // Os dois <td> dentro do <tr>
    linha.append(colunaUsuario);
    linha.append(colunaPalavras);

    return linha;
}
```

Com a linha devidamente criada, vamos adicioná-la no corpo da tabela:
```javascript
function inserePlacar() {
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome";
    var numPalavras = $("#contador-palavras").text();

    var linha = novaLinha(usuario, numPalavras);

    corpoTabela.append(linha);
}
```

#### Chamando a inserePlacar
A nossa função insere placar deve ser chamada ao fim de cada jogo, e isto ocorre quando tempo chega a zero, ou seja dentro do if da função inicializaCronometro :
```javascript
function inicializaCronometro() {
    ...
            if (tempoRestante < 1) {
                clearInterval(cronometroID);

                campo.attr("disabled", true);
                campo.toggleClass("campo-desativado");
                // Alteração aqui
                inserePlacar();
            }
    ...
}
```

Mas a função inicializaCronometro já está fazendo muitas coisas, vamos separar a responsabilidade de desabilitar o campo, colocar o fundo cinza e chamar o inserePlacar em uma outra função, a função finalizaJogo:
```javascript
function finalizaJogo() {
    campo.attr("disabled", true);
    campo.toggleClass("campo-desativado");
    inserePlacar();
}
```

E vamos chamar a função finalizaJogo dentro do if na inicializaCronometro substituindo as últimas linhas:
```javascript
function inicializaCronometro() {
    ...
            if (tempoRestante < 1) {
                clearInterval(cronometroID);
                //Alteração aqui
                finalizaJogo();
            }
    ...
}
```

Agora toda ação que deve ser feita ao final de cada jogo pode ser adicionada na função finalizaJogo.

### Mãos na massa: Removendo linhas do placar

Já estamos adicionando linhas no nosso placar, então agora devemos ter a opção de removê-las. Para isto, vamos adicionar um pequeno botão de remoção em cada linha da tabela, ele será um link estilizado pelo Materialize. Vamos adicioná-lo dentro de um "td", como uma nova coluna da tabela, e adicionar um novo "th" para referenciá-lo:
```html
<section class="placar">
    <h3 class="center">Placar</h3>
        <table class="centered bordered">
            <thead>
                <tr>
                    <th>Usuário</th>
                    <th>No. de palavras</th>
                    <th>Remover</th>
                </tr>
            </thead>
        <tbody>
            <tr>
                <td>Usuario Exemplo</td>
                <td>99</td>
                <td>
                    <a href="#">
                        <i class="small material-icons">delete</i>
                    </a>
                </td>
            </tr>
        </tbody>
    </table>
</section>
```

Para esse botão aparecer também nas pontuações que serão adicionadas futuramente, precisamos alterar a nossa função novaLinha() para adicionar o botão de remoção na linha também. No main.js, adicionamos:
```javascript
function novaLinha(usuario,palavras) {
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
    var colunaRemover = $("<td>");

    var link = $("<a>").attr("href","#");
    var icone = $("<i>").addClass("small").addClass("material-icons").text("delete");

    linha.append(colunaUsuario);
    linha.append(colunaPalavras);

    return linha;
}
```

Utilizamos algumas já conhecidas funções do jQuery para montar a sua estrutura semelhante a do HTML. Falta posicionar o ícone dentro do link, o link dentro da coluna, e a coluna dentro da linha:

```javascript
function novaLinha(usuario,palavras) {
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
    var colunaRemover = $("<td>");

    var link = $("<a>").attr("href","#");
    var icone = $("<i>").addClass("small").addClass("material-icons").text("delete");

    // Ícone dentro do <a>
    link.append(icone);

    // <a> dentro do <td>
    colunaRemover.append(link);

    // Os três <td> dentro do <tr>
    linha.append(colunaUsuario);
    linha.append(colunaPalavras);
    linha.append(colunaRemover);

    return linha;
}
```

### Removendo a linha
Agora que o botão de remoção já é adicionado corretamente em cada linha, precisamos fazer com que ele remova a linha quando for clicado. Para isso criamos a função removeLinha():

```javascript
function removeLinha() {

}
```
Se clicarmos no ícone de remoção, iremos perceber que a página salta para o topo. Para remover esse comportamento, vamos utilizar a função preventDefault(). Vamos alterar nosso evento para receber um parâmetro que permita usá-la:
```javascript
function removeLinha(event) {
    event.preventDefault();
}
```
Agora, para remover um elemento do HTML , vamos utilizar a função com nome semelhante do jQuery, a remove():
```javascript
function removeLinha(event) {
    event.preventDefault();
    $(this).remove();
}
```

Como elementos comuns do HTML não têm acesso às funções do jQuery, empoderamo-os com as funções do objeto jQuery, envolvendo-os com a função jQuery.
Agora precisamos chamar a função removeLinha() para o clique de todos os botões que estão dentro das linhas criadas, podendo utilizar o find() para achá-los:
```javascript

function inserePlacar() {
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome"
    var numPalavras = $("#contador-palavras").text();

    var linha = novaLinha(usuario,numPalavras);
    linha.find(".botao-remover").click(removeLinha);

    corpoTabela.append(linha);
}
```

Se clicarmos no ícone da lixeira, veremos que somente a mesma sumiu! Isto acontece pois estamos chamando a função remove() na tag "a", que é quem foi clicada! Para remover a linha inteira, vamos olhar a estrutura HTML, e ver que a tag "tr" é pai do pai da tag "a". Para acessar o pai com o jQuery, utilizamos a função parent(). Logo, vamos chamá-la duas vezes na hora de remover:

```javascript
function removeLinha() {
    event.preventDefault();
    $(this).parent().parent().remove();
}
```

Agora nossas linhas geradas pelo jogo podem ser deletadas normalmente! Podemos até mesmo remover as linhas que já vinham por padrão no nosso placar, deixando apenas as que foram geradas pelo usuário!

### Mãos na massa: Organizando o nosso código

Para organizar melhor o nosso código JavaScript, vamos separar as suas responsabilidades em arquivos diferentes.
O que é referente ao placar do nosso jogo, colocaremos em um outro arquivo, chamado placar.js. Ou seja, moveremos as funções inserePlacar, novaLinha e removeLinha:
```javascript
function inserePlacar() {
    var corpoTabela = $(".placar").find("tbody");
    var usuario = "Seu-nome"
    var numPalavras = $("#contador-palavras").text();

    var linha = novaLinha(usuario, numPalavras);
    linha.find(".botao-remover").click(removeLinha);

    corpoTabela.append(linha);
}

function novaLinha(usuario, palavras) {
    var linha = $("<tr>");
    var colunaUsuario = $("<td>").text(usuario);
    var colunaPalavras = $("<td>").text(palavras);
    var colunaRemover = $("<td>");

    var link = $("<a>").addClass("botao-remover").attr("href", "#");
    var icone = $("<i>").addClass("small").addClass("material-icons").text("delete");

    link.append(icone);

    colunaRemover.append(link);

    linha.append(colunaUsuario);
    linha.append(colunaPalavras);
    linha.append(colunaRemover);

    return linha;
}

function removeLinha() {
    event.preventDefault();
    $(this).parent().parent().remove();
}
```

Daqui para frente, cada parte do nosso código ficará em um arquivo próprio, melhorando a organização da nossa aplicação!

### Projeto Final do Curso 

Você pode fazer o download completo do projeto deste módulo AQUI. 

https://s3.amazonaws.com/caelum-online-public/jquery-alura-typer/stages/jquery-modulo-1-final.zip



[Voltar ao Índice](#indice)

---

