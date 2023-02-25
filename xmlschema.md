<h1>🔎 XML Schema</h1>

<p>Assim como o DTD é utilizada para definição de regras de validação ("esquemas") em documentos no formato XML. Sua diferença está em ser uma linguagem baseada no formato XML, inclusive foi a primeira linguagem de esquema para XML a obter o status de recomendação por parte do W3C. Ela é uma alternativa ao DTD, já que sua sintaxe não é baseada no formato XML.</p>
<p>O arquivo que contém as definições na linguagem XML Schema é chamado de XSD (XML Schema Definition)</p>
<p>Ela surgiu para resolver os principais problemas encontrados no DTD, pois nele não existe um conjunto amplo de tipos (todos os dados são interpretados como texto), trazendo efeitos indesejáveis. Também não suportam espaços de nomes (namespace), forçam que os elementos sempre apareçam na ordem especificada etc.</p>

<h2>Estrutura básica de um XML Schema</p>
<p>Em sua essência é um documento XML. Isso é, deve obedecer as mesmas regras que um documento XML. Os elementos são declarados utilizando-se a tag “element”, já os atributos se parecem muito com as declarações de elementos.</p>

<h3>Exemplo de um documento XML Schema</h3>

~~~xml

<xsd:element name="cliente">
 <xsd:complexType>
  <xsd:sequence>
   <xsd:element name="nome" type="xsd:string"/>
   <xsd:element name="endereco" type="xsd:string"/>
   <xsd:element name="cep" type="xsd:integer"/>
  </xsd:sequence>
 </xsd:complexType>
</xsd:element>

~~~

*Exemplo retirado do Wikipedia*

<p>Nosso objetivo não é aprofundar no XML Schema e demonstrar a criação de um na prática, apenas informar sobre sua existência e importância.</p>

[Próxima sessão ➡️](bibliografia.md)