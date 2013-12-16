webappvraptorbasica
===================

Código-fonte básico para uma aplicação web em Java usando o VRaptor da Caelum. 
O gerenciamento de dependências nesse projeto é feito com o maven.
A classe principal do VRaptor é br.com.caelum.vraptor.VRaptor, e no web.xml ele não é configurado como servlet, mas sim como um filter com seu filter-mapping para URLs. Dêem uma olhada no web.xml pra ver como ficou.
Com o VRaptor configurado, foi criado uma classe chamada NegocioController e para o VRaptor utilizá-lo foi inserido a anotação @Resource na declaração da classe.
Essa classe, "NegocioController", possui um método chamado "funcionalidade". Ele é chamado quando usamos um URL no padrão http://servidor:porta/webappvraptorbasica/negocio/funcionalidade . 
O sufixo Controller é omitido da classe, e para apresentarmos uma página ao usuário, criamos em WEB-INF a pasta "jsp" e dentro dela a pasta "negocio", que corresponde à classe NegocioController mas sem sufixo, e dentro dela a página "funcionalidade.jsp", que corresponde ao seu método "funcionalidade".
Acredito que com essas instruções básicas é possivel começar JÁ com o VRaptor.