# Olhe dentro de sua caixa de ferramentas

**Intenção:** Selecione um projeto FLOSS para contribuir baseado em tecnologias que você já conheça ou usa em seu ambiente de trabalho.
Por exemplo, se você tem uma boa experiência em programação com uma linguagem de programação específica, escolha um projeto escrito nessa linguagem para contribuir.

## Motivação

Você está disposto a contribuir em um projeto FLOSS sem ter que aprender uma nova liguagem de programação ou ter que introduzir uma tecnologia desconhecida em seu ambiente de trabalho.
Possa ser o caso que você e seu time são bem produtivos com certas tecnologias como Java e MySQL.
Ou você está trabalhando com outros desenvolvedores em projetos existentes e todos eles estão usando C#.

## Problema

Como você vai encontrar um projeto FLOOS para contribuir, dando uma ou mais restrições tecnológicas?

## Forças

* _Auto-confiança_. Suas abilidades de programação em certas tecnologias fazer você se sentir confiante para superar as barreiras iniciais e possivelmente realizar melhores contribuições para o projeto.

* _Você está procurando um projeto a ser incorporado a uma solução existente_.
Por exemplo, você pode estar procurando por uma biblioteca para ser usada em uma aplicação existente. Nesse caso, você precisa que a biblioteca esteja escrita na mesma linguagem de programação da aplicação.

* _Você não quer ou tem tempo para aprender coisas novas_.
Sua compania tem que adicionar nova funcionalidade baseada em um projeto existente, mas não dispõe do tempo necessário para se familiarizar com tecnologias e ferramentas novas e desconhecidas.

* _Barreiras organizacionais_. Sua organização tem uma política estrita para aprovar qualquer tecnologia nova antes dessa ser introduzida, e você preferiria evitar o problema.

* _A adoção de uma nova tecnologia pode impor custos proibitvos_.
Por exemplo, adotar uma linguagem de programação interpretada para o desenvolvimento de software incorporado exigirá a adição de capacidade de armazenamento extra nos dispositivos, para realizar a instalação do interpretador da liguagem.

## Solução

Procure por projetos que combinem com o seu critério para tecnologia aceitável.
Tecnologias aceitáveis são aquelas que te são familiares, que são aprovadas por sua organização ou colegas de trabalho, ou que se integrem de forma agradável ao seu ambiente existente.

Se seu critério inclui uma linguagem de programação específica você deve começar procurando por projetos em repositórios linguagem-específica. Por exemplo, a maiorias de projetos em Perl, Ruby e Python estão listados em [CPAN](http://www.cpan.org/), [Rubygems](http://rubygems.org/) e [PyPI](http://pypi.python.org/), suas respectivas comunidades de repositório.

Algums vezes seu critério não será a linguagem de programação, mas outras partes de uma arquitetura de aplicação, como o sistema da base de dados.
Por exemplo, você quer verificar se o novo sistema de gerenciamento de conteúdo que você está avaliando suporta o sistema de base de dados relacional aprovado pela sua organização. 
Você pode pesquisar projetos em [Freecode](http://freecode.com/) (antes Freshmeat), o qual é um catálogo do Linux, Unis e software de plataforma cruzada, a maioria deles de código aberto. Você pode filtrar a lista de projetos por linguagem de programação e por tags, que são atribuídas pelos usuários. Algumas tags se referem a tecnoligias específicas suportadas ou usadas pelo projeto, como o sistema de base de dados ou uma biblioteca de software específica.
Um serviço similar é o [Ohloh](http://www.ohloh.net/).
Você pode utilizá-lo, por exemplo, para procurar por 
[sistemas de gerenciamento de conteúdo escritos em PHP com suporte para bancos de dados MySQL](http://www.ohloh.net/tags/cms/php/mysql).

## Trade-Offs

**Prós:** 

* A curva de aprendizado para se engajar em um projeto é possivelmente minimizada desde que você já lide com tecnologias e ferramentas conhecidas.

* Seu ambiente está provavelmente configurado para o projeto, ou pelo menos você sabe como instalar as dependências.

* Você pode fazer contribuições com melhor qualidade técnica desde que você esteja familiarizado com as tecnologias.

* Você pode ser bem sucedido, ganhando reputação ou até mesmo um emprego (empresas buscando programadores com habilidades específicas podem encontrar contratações em potencial examinando códigos de softwares de código aberto).  

**Contras:** 

* Quando você limita sua escolha pelo critério da tecnologia, você possivelmente exclui projetos que poderiam ser melhor encaixados em termos de funcionalidade.

* Se você sempreater a tecnologias conhecidas, você provavelmente tem problemas em aprender novas ferramentas que podem se mostrar mais úteis em determinados contextos. Por exemplo, você pode acabar desenvolvendo aplicações WEB em COBOL, embora existam importantes bibliotecas para programação web que estão disponíveis para outras linguagens.

## Lógica

Se você selecionou um projeto FLOSS que utiliza tecnologia aceitável, você pode se concentrar em outros problemas de projeto -- por exemplo, entender os recursos implementados ou se sentir confortável com o processo de desenvolvimento.

Além disso, você provavelmente vai prover melhores contribuições técnicas ao projeto. Quando codificando, você talvez aplique seu conhecimento sobre linguagens de programação, armadilhas a serem evitadas, tecnologias e ferramentas suportadas, diretrizes que devem ser seguidas, etc.
Você também deve enontrar e consertar bugs mais facilmente, ajudando na documentação técnica, etc.

## Usos conhecidos

De volta a 2006, nós começamos a trabalhar em um projeto de pesquisa de transformação de modelo chamado TEMA. Nesse tempo, a maioria ddas tecnologias de software para transformação de modelo era em java, mas desenvolvedores envolvidos no projeto preferiam Ruby. Ele procurou por projetos de transormação de modelo em Ruby e achou [RMOF](http://rubyforge.org/projects/rmof/). O projeto acabou contribuindo uma quantidade significativa de código ao projeto RMOF.

Um dos autores estava provurando por um editor de texto estensível que suportasse seu trabalho diário. Além disso, ele não queria gastar muito tempo aprendendo como escrever novas extenssões -- o editos deveria dar suporte ao trabalho, não para evitar que esse fosse feito. Vim e Emacs, editores de texto tradicionais, não eram boas opções, porque Vim usa sua própria linguagem de script, e Emacs usa uma variante do Lisp, o qual o autor não está familiarizado. O autor acabou escolhendo um editor escrito em Python (com extensões também escritas nessa linguagem) e começou a contribuir em extensões existentes que proviam a maoria das características que ele necessitava para suportar seu fluxo de trabalho.

As chances de que você e seus colegas de trabalho já tenham usado esse padrão muitas vezes é alta.
Por exemplo, pode ser uma framework web em PHP que você escolheu porque você domina programação em PHP, ou uma biblioteca em java que você escolheu porque integra bem com outras bibliotecas que você esteja usando.
Esse é um padrão muito comum na prática.

## Padrões relacionados

As vezes, familiaridade com o software é mais importante do que dominar linguagem de programação ou outras tecnologias. Nesse caso, você pode preferir por [Andar em um terreno familiar](link://selection/WalkOnFamiliarGround). 

Se, por outro lado, funcionalidade é mais importante do que familiaridade, você sempre pode [Explorar um Admirável Mundo Novo](link://selection/ExploreABraveNewWorld).

Contudo, você pode descobir que projetos que melhor combinam com as funcionalidades desejadas usam tecnologia que você não está familiarizado.


## O que vem depois

Depois de escolher um projeto usando critério baseado em tecnologia, você provavelmente deveria [Fazer uma instalação Simulada](link://involvement/DoAMockInstallation) pra reafirmar sua certeza de que a tecnologia está sob controle.
