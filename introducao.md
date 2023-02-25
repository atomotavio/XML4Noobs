<h1>📣 Introdução ao XML</h1>

<h2>O que é XML?</H2>

<p>eXtensible Markup Language, é uma linguagem de marcação de dados que provê um formato para descrever dados estruturados. Ele é um texto -em formato unicode, com tags de marcação (markup tags) e outras informações.</p>
<p>Ele foi construido baseado em uma norma ISO que define o SGML (Standard Generalized Markup Language), ela define as declarações/sintaxe das linguagens de marcação.</p>
<p>A linguagem XML tem sido adotada como padrão para representação de dados e troca de informações nas mais diferentes áreas.</p>
<p>XML representa dados de forma muito mais legível para nós, quando comparamos com outros formatos (ex: arquivo “.csv”, arquivo JSON, tabelas relacionais). Ou seja: as próprias tags já são capazes de explicar o significado do conteúdo dos dados que representam. Normalmente, basta “bater o olho” em um arquivo XML para entender o seu significado.</p>

<h3>Exemplo de documento XML</h3>

~~~xml

<?xml version="1.0">
<filmes>
    <filme id="1">
        <titulo>O XML veste prada</titulo>
        <resumo>O filme mostra a elegância da XML na representação de dados estruturados e semi estruturados.</resumo>
        <genero>Aventura</genero>
        <genero>Documentário</genero>
        <elenco>
            <ator>Mark UPlanguage</ator>
            <ator>Mary well-Formed</ator>
            <ator>Sedna D. Atabase</ator>
        </elenco>
    </filme>
</filmes>

~~~

*Exemplo retirado do blog DevMedia*

[Próxima sessão ➡️](xmlhtml.md)