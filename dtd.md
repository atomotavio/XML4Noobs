<h1>🔗 DTD</h1>

<p>Para entender o DTD, precisamos primeiro entender o por quê de ele existir, e seu papel dentro (ou fora) do documento XML.</p>
<p>Por mais bonito e legível que o XML possa ser para nós humanos, máquinas são objetos burros e é sempre necessário falar o óbvio para elas. Por mais que você estruture o XML corretamente, é necessário dizer ao computador a quem o atributo ou elemento pertencem, se aquele atributo ou elemento é opcional, quantas vezes eles podem aparecer etc.</p>
<p>Para isso, foi então criado o DTD, que literalmente é uma definição de tipo de documento (Document Type Definition). Ele é responsável por definir uma gramática para válidar documentos, isto é, um conjunto de regras que definem a estrutura do documento.</p>
<p>Vale lembrar que o DTD é apenas uma das formas de validação do XML, no próximo capítulo inclusive veremos mais uma delas, e provavelmente a mais comum, o XML Schema</p>

Numa DTD são definidos:

* Os elementos contidos no documento;
* Os atributos dos elementos;
* As entidades;
* As hierarquias e ordens desses elementos;
* Descrição dos atributos e elementos que podem aparecer no documento.

**Lembrando que a validação compara um documento em particular com uma DTD correspondente, ou seja, para cada XML é necessário que se escreva uma DTD, que pode ser tanto um documento externo, como estar incorporado a um documento XML**

**O documento precisa estar bem formatado para ser validado.**

A DTD vai conter:

* Declarações dos tipos de elementos;
* Declarações de listas de atributos;
* Declarações de entidades;
* Declarações de notação.

<h3>Exemplo de XML com DTD internamente</h3>

~~~xml

 <?xml version="1.0"?>
<!DOCTYPE note [
<!ELEMENT note (to,from,heading,body)>
<!ELEMENT to (#PCDATA)>
<!ELEMENT from (#PCDATA)>
<!ELEMENT heading (#PCDATA)>
<!ELEMENT body (#PCDATA)>
]>
<note>
<to>Tove</to>
<from>Jani</from>
<heading>Reminder</heading>
<body>Don't forget me this weekend</body>
</note> 

~~~

<h3>Exemplo de um XML com referência a um DTD externo e seu respectivo DTD</h3>

~~~~xml

 <?xml version="1.0"?>
<!DOCTYPE note SYSTEM "note.dtd">
<note>
  <to>Tove</to>
  <from>Jani</from>
  <heading>Reminder</heading>
  <body>Don't forget me this weekend!</body>
</note> 

~~~~

~~~~xml


<!ELEMENT note (to,from,heading,body)>
<!ELEMENT to (#PCDATA)>
<!ELEMENT from (#PCDATA)>
<!ELEMENT heading (#PCDATA)>
<!ELEMENT body (#PCDATA)> 

~~~~

*Exemplos retirado da W3Schools*

<p>Nosso objetivo não é aprofundar no DTD e demonstrar a criação de um na prática, apenas informar sobre sua existência e importância.</p>


[Próxima sessão ➡️](xmlschema.md)