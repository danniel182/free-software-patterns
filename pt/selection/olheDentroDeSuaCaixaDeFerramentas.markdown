# Olhe dentro de sua caixa de ferramentas

**Inten��o:** Selecione um projeto FLOSS para contribuir baseado em tecnologias que voc� j� conhe�a ou usa em seu ambiente de trabalho.
Por exemplo, se voc� tem uma boa experi�ncia em programa��o com uma linguagem de programa��o espec�fica, escolha um projeto escrito nessa linguagem para contribuir.

## Motiva��o

Voc� est� disposto a contribuir em um projeto FLOSS sem ter que aprender uma nova liguagem de programa��o ou ter que introduzir uma tecnologia desconhecida em seu ambiente de trabalho.
Possa ser o caso que voc� e seu time s�o bem produtivos com certas tecnologias como Java e MySQL. Ou voc� est� trabalhando com outros desenvolvedores em projetos existentes e todos eles est�o usando C#.

## Problema

Como voc� vai encontrar um projeto FLOOS para contribuir, dando uma ou mais restri��es tecnol�gicas?

## For�as

* _Auto-confian�a_. Suas abilidades de programa��o em certas tecnologias fazem voc� se sentir confiante para superar as barreiras iniciais e possivelmente realizar melhores contribui��es para o projeto.

* _Voc� est� procurando um projeto a ser incorporado a uma solu��o existente_.
Por exemplo, voc� pode estar procurando por uma biblioteca para ser usada em uma aplica��o existente. Nesse caso, voc� precisa que a biblioteca esteja escrita na mesma linguagem de programa��o da aplica��o.

* _Voc� n�o quer ou n�o tem tempo para aprender coisas novas_.
Sua empresa tem que adicionar alguma nova funcionalidade baseada em um projeto existente, mas n�o disp�e do tempo necess�rio para se familiarizar com tecnologias e ferramentas novas e desconhecidas.

* _Barreiras organizacionais_. Sua organiza��o tem uma pol�tica estrita para aprovar qualquer tecnologia nova antes dessa ser introduzida, e voc� preferiria evitar o problema.

* _A ado��o de uma nova tecnologia pode impor custos proibitivos_.
Por exemplo, adotar uma linguagem de programa��o interpretada para o desenvolvimento de software incorporado exigir� a adi��o de capacidade de armazenamento extra nos dispositivos para realizar a instala��o do interpretador da liguagem.

## Solu��o

Procure por projetos que combinem com o seu crit�rio para tecnologia aceit�vel.
Tecnologias aceit�veis s�o aquelas que te s�o familiares, que s�o aprovadas por sua organiza��o ou colegas de trabalho, ou que se integrem de forma agrad�vel ao seu ambiente existente.

Se seu crit�rio inclui uma linguagem de programa��o espec�fica voc� deve come�ar procurando por projetos em reposit�rios linguagem-espec�fica. Por exemplo, a maiorias de projetos em Perl, Ruby e Python est�o listados em [CPAN](http://www.cpan.org/), [Rubygems](http://rubygems.org/) e [PyPI](http://pypi.python.org/), suas respectivas comunidades de reposit�rio.

Algums vezes seu crit�rio n�o ser� a linguagem de programa��o, mas outras partes de uma arquitetura de aplica��o, como o sistema da base de dados.
Por exemplo, voc� quer verificar se o novo sistema de gerenciamento de conte�do que voc� est� avaliando suporta o sistema de base de dados relacional aprovado pela sua organiza��o. 
Voc� pode pesquisar projetos em [Freecode](http://freecode.com/) (antes Freshmeat), o qual � um cat�logo do Linux, Unix e software de plataforma cruzada, a maioria deles de c�digo aberto. Voc� pode filtrar a lista de projetos por linguagem de programa��o e por tags, que s�o atribu�das pelos usu�rios. Algumas tags se referem a tecnoligias espec�ficas suportadas ou usadas pelo projeto, como o sistema de base de dados ou uma biblioteca de software espec�fica.
Um servi�o similar � o [Ohloh](http://www.ohloh.net/).
Voc� pode utiliz�-lo, por exemplo, para procurar por [sistemas de gerenciamento de conte�do escritos em PHP com suporte para bancos de dados MySQL](http://www.ohloh.net/tags/cms/php/mysql).

## Trade-Offs

**Pr�s:** 

* A curva de aprendizado para se engajar em um projeto � possivelmente minimizada desde que voc� j� lide com tecnologias e ferramentas conhecidas.

* Seu ambiente est� provavelmente configurado para o projeto, ou pelo menos voc� sabe como instalar as depend�ncias.

* Voc� pode fazer contribui��es com melhor qualidade t�cnica desde que voc� esteja familiarizado com as tecnologias.

* Voc� pode ser bem sucedido, ganhando reputa��o ou at� mesmo um emprego (empresas buscando programadores com habilidades espec�ficas podem encontrar contrata��es em potencial examinando c�digos de softwares de c�digo aberto).  

**Contras:** 

* Quando voc� limita sua escolha pelo crit�rio da tecnologia, voc� possivelmente exclui projetos que poderiam ser melhor encaixados em termos de funcionalidade.

* Se voc� sempre ater a tecnologias conhecidas, voc� provavelmente tem problemas em aprender novas ferramentas que podem se mostrar mais �teis em determinados contextos. Por exemplo, voc� pode acabar desenvolvendo aplica��es WEB em COBOL, embora existam importantes bibliotecas para programa��o web que est�o dispon�veis para outras linguagens.

## L�gica

Se voc� selecionou um projeto FLOSS que utiliza tecnologia aceit�vel, voc� pode se concentrar em outros problemas de projeto -- por exemplo, entender os recursos implementados ou se sentir confort�vel com o processo de desenvolvimento.

Al�m disso, voc� provavelmente vai prover melhores contribui��es t�cnicas ao projeto. Quando codificando, voc� talvez aplique seu conhecimento sobre linguagens de programa��o, armadilhas a serem evitadas, tecnologias e ferramentas suportadas, diretrizes que devem ser seguidas, etc.
Voc� tamb�m deve enontrar e consertar bugs mais facilmente, ajudando na documenta��o t�cnica, etc.

## Usos conhecidos

De volta a 2006, n�s come�amos a trabalhar em um projeto de pesquisa de transforma��o de modelo chamado TEMA. Nesse tempo, a maioria das tecnologias de software para transforma��o de modelo eram em java, mas desenvolvedores envolvidos no projeto preferiam Ruby. Ele procurou por projetos de transorma��o de modelo em Ruby e achou o [RMOF](http://rubyforge.org/projects/rmof/). O projeto acabou contribuindo uma quantidade significativa de c�digo ao projeto RMOF.

Um dos autores estava provurando por um editor de texto estens�vel que suportasse seu trabalho di�rio. Al�m disso, ele n�o queria gastar muito tempo aprendendo como escrever novas extenss�es -- o editor deveria dar suporte ao trabalho, n�o para evitar que esse fosse feito. Vim e Emacs, editores de texto tradicionais, n�o eram boas op��es, porque Vim usa sua pr�pria linguagem de script, e Emacs usa uma variante do Lisp, o qual o autor n�o est� familiarizado. O autor acabou escolhendo um editor escrito em Python (com extens�es tamb�m escritas nessa linguagem) e come�ou a contribuir em extens�es existentes que proviam a maoria das caracter�sticas que ele necessitava para suportar seu fluxo de trabalho.

As chances de que voc� e seus colegas de trabalho j� tenham usado esse padr�o muitas vezes � alta.
Por exemplo, pode ser uma framework web em PHP que voc� escolheu porque voc� domina programa��o em PHP, ou uma biblioteca em java que voc� escolheu porque integra bem com outras bibliotecas que voc� esteja usando.
Esse � um padr�o muito comum na pr�tica.

## Padr�es relacionados

As vezes, familiaridade com o software � mais importante do que dominar a linguagem de programa��o ou outras tecnologias. Nesse caso, voc� pode preferir por [Andar em um terreno familiar](link://selection/WalkOnFamiliarGround). 

Se, por outro lado, funcionalidade � mais importante do que familiaridade, voc� sempre pode [Explorar um Admir�vel Mundo Novo](link://selection/ExploreABraveNewWorld).

Contudo, voc� pode descobir que projetos que melhor combinam com as funcionalidades desejadas usam tecnologia que voc� n�o est� familiarizado.


## O que vem depois

Depois de escolher um projeto usando crit�rio baseado em tecnologia, voc� provavelmente deveria [Fazer uma instala��o Simulada](link://involvement/DoAMockInstallation) pra reafirmar sua certeza de que a tecnologia est� sob controle.
