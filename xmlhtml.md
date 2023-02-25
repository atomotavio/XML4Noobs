<h1>🆚 XML vs HTML</h1>

<p>Primeiro, antes que pareça, não existe uma competição entre essas linguagens de marcação, até porque seus propósitos são diferentes, porém, elas compartilham caracteristicas semelhantes.</p>
<p>A primeira e provavelmente mais óbvia, é o fato de ambas utilizarem tags em sua estrutura. Além disso, se você se lembra do capítulo anterior e da ISO que define a SGML, deve imaginar que algumas de suas semelhanças podem ter relação com o fato de ambas seguirem essas especificações, mas para além de estarem de acordo com a norma, são as mais famosas linguagens que a seguem.</p>
<p>Mas e sobre suas diferenças? Enquanto o XML é uma linguagem de marcação criada para representar dados, o HTML é uma linguagem de marcação que define a aparência e as ações em uma página web.</p>

<h3>Exemplo de um documento HTML</h3>

~~~~html

<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="utf-8" />
        <meta name="description" content="a descrição do seu site em no máximo 90 caracteres">
        <meta name="keywords" content="escreva palavras-chaves curtas, máximo 150 caracteres">
        <title>Título do Documento</title>
    </head>
    <body>
    <!-- Aqui fica a página que será visível para todos, onde pode-se inserir
    textos, imagens, links para outras páginas, etc, geralmente usa-se: -->

    <div>
        Tag para criar-se uma 'caixa', um bloco, mais utilizada com "Cascading Style Sheets
         (Folhas de Estilo em Cascata)
    </div>

    <span>Tag para modificação de uma parte do texto da página</span>

    <img src="endereço_de_uma_imagem.jpg" />

    <a href="http://www.wikipedia.org">Wikipedia, A Enciclopédia Livre</a>
    </body>
</html>

~~~~

*Exemplo retirado do wikipedia*

[Aprenda mais sobre HTML](https://github.com/sorenhe4rt/HTML4Noobs)

[Próxima sessão ➡️](estrutura.md)