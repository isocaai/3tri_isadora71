<!DOCTYPE html>
<!--Idioma do projeto=lingua portuguesa-->
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!--Título para o Terceiro trimestre-->
    <title>Redes Sociais</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!--Vamos dividir conteúdo em três partes: cabeçalho, usando a tag <header>;
    Conteúdo principal, usando a tag <main>;
    Rodapé, usando a tag <footer>.
    O código ficará da seguinte forma:-->
    <header>
        <!--No cabeçalho da página, incluiremos um título <h1> chamado Relatório das redes sociais.-->
        <h1>Relatório das redes sociais</h1><!--h1-Texto grande-->
        <!--Para isso, utilizaremos a tag <nav>, que cria um menu de navegação-->
        <nav>
            <!--E a tag <a>, que cria links de navegação-->
            <a href="index.html">Mundo</a>
            <a href="#">Minha escola</a>
        </nav>
    </header>
    <!--Agora, trabalharemos na tag <main>, criando uma estrutura para conseguir posicionar nossos gráficos. Começaremos incluindo nessa tag
uma classe chamada graficos-section (seção de gráficos).
Dentro da tag <main>, criaremos uma seção que terá um id graficos-container e uma classe também chamada graficos-conteiner-->
    <main class="graficos-section">
        <section id="graficos-container" class="graficos-container">
        <!--crie os gráficos aqui-->          
        </section>
    </main>
    <!--Por fim, vamos modificar o rodapé.
    Adiciona-se apenas uma tag de parágrafo (footer) que informa quem está desenvolvendo a página.-->
    <footer>
        <p>Desenvolvido por: Digite aqui o seu nome</p>
    </footer>
    <script type="module" src="graficos/informacoesglobais.js"></script>    
</body>
</html>


</body>
</html>

i/*Abra seu projeto e crie um arquivo com nome: style.css
Cole o código logo abaixo. */


/*Esta parte indica a fonte que você vai usar no seu projeto, para conseguí-la, siga os passoa abaixo::after
Entre no endereço abaixo
https://fonts.google.com/
Pesquise a fonte - nunito sans
Clique sobre a primeira fonte encontrada
Em seguida clique em - Get fonte
Depois em – Get embed code
Selecione a opção - @import
Copie tudo (somente) dentro da tag – Style
 */
 @import url('https://fonts.googleapis.com/css2?family=Nunito+Sans:ital,opsz,wght@0,6..12,200..1000;1,6..12,200..1000&display=swap');


 /*O código abaixo indica as cores que iremos utilizar no projeto
 Para isso:
 Entre no seguinte endereço https://colorhunt.co/
 Procure uma paleta de seu agrado e digite os códigos hexadecimais das cores.
 */
 :root {
     --bg-color: #222831;
     --primary-color: #DDDDDD;
     --secondary-color: #F05454;
     --font: "Nunito Sans", sans-serif;
 }
 /*Agora vamos estilizar o body
 */
 body {
     /*Esse comando vai mudar a cor de fundo */
     background-color: var(--bg-color);
     /*IMPORTANTE: ACRESCENTAR NO HTML APÓS A LINHA TITLE, ACRESCENTAR O COMANDO QUE VAI CHAMAR O CSS
     <link rel="stylesheet" href="style.css"> */
     /*O comando abaixo indicará a cor de texto a ser usado no projeto*/
     color: var(--primary-color);
     /*O comando abaixo indicará a fonte a ser usado no projeto*/
     font: var(--font);
     /*Para usar toda a disposição da tela que temos*/
     height: 100vh;
     /*Para deixar sem margem*/
     margin: 0;
 }
 /*Agora vamos estilizar o header*/
 header {
    /*Esse comando vai mudar a cor de fundo */
    background-color: var(--primary-color);
    /*Para alinhar o texto ao centro*/
    text-align: center;
     /*Para o background ocupar todo o espaço da tela*/
     padding: 1px;
}
/*Agora vamos estilizar o h1, que está dentro do header*/
h1 {
    /*tamanho da fonte*/
    font-size: 2 rem;
    /*cor da letra*/
    color: var(--bg-color);
    /*Peso da fonte*/
    font-weight: 700;


}
/*Agora vamos estilizar o Nav*/
nav {
    /*Posicionamento dos elementos*/
    display: flex;
    /*Alinhando os elementos*/
    justify-content: center;
    /*Peso da fonte*/
    font-weight: 400;
}
nav a {
    /*Texto simples, sem sublinhado negrito etc*/
    text-decoration: none;
    color: var(--bg-color);
    /*Margem superior, esquerda, direita, inferior, entre os elementos nesta ordem*/
    margin: 0 2rem 1rem 0rem;
    font-size: 1.2rem;
}
/*Para sabaer que se trata de um link, quando passar o mouse algo muda*/
nav a:hover {
    /*aparece o underline*/
    text-decoration: underline;
    /*aumenta um pouco o tamanho da letra*/
    transform: escale(0.90);
    /*altera a velocidade*/
    transition: transform 0.1s;
}


.graficos-container {
    margin: 5rem;
}


.graficos-container__texto {
    font-size: 1.3rem;
    text-align: center;
    padding: 2rem;
    border: var(--secondary-color) solid 2px;
}


span {
    font-weight: bold;
    color: var(--secondary-color);
}






/*Agora vamos estilizar o Footer*/
footer {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: var(--primary-color);
    color: var(--bg-color);
    /*largura*/
    width: 100%;
    /*altura*/
    height: 3rem;
    /*margem superior*/
    margin-top: 2rem;
}

