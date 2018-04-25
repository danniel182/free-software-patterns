# First Contact
Você faz parte de uma equipe que desenvolve um sistema de software chamado proDoc, que apóia médicos em suas atividades diárias.
Os principais requisitos funcionais dizem respeito a (i)manter os prontuários dos pacientes e (ii)manter o controle do dinheiro a ser pago pelos pacientes e pelos planos de saúde. A legislação de cuidados de saúde na Suíça é bastante complicada e muda regularmente, portanto, há poucos concorrentes para se preocupar. No entanto, uma nova empresa recém-adquirida, adquiriu  uma quota de mercado considerável com um produto concorrente chamado XDoctor. Os recursos de venda do XDoctor possui independência de plataforma e sua integração com a Internet. O sistema oferece um cliente de e-mail incorporado e um navegador da web. O XDoctor também explora a internet para o processamento de transações com os seguros de saúde.

Para garantir sua posição no mercado, sua empresa comprou o XDoctor e agora quer recuperar o máximo possível do negócio. Em particular, eles querem elevar a funcionalidade da Internet do XDoctor para reutilizá-la no proDoc. Você é solicitado a fazer uma primeira avaliação e desenvolver um plano sobre como mesclar os dois produtos em um só. No início, há muito pouco conhecimento sobre os detalhes técnicos do produto concorrente. Da equipe de desenvolvimento original de quatro pessoas, apenas uma se juntou à sua empresa. Seu nome é Dave e ele trouxe uma caixa grande para o seu escritório contendo muito papel (a documentação?) E dois CDs. O primeiro é o disco de instalação do XDoctor contendo um instalador para Windows, MacOS e Linux. O outro contém cerca de 500.000 linhas de código Java e outras 10.000 linhas de código C. Olhando meio desesperadamente para esta caixa em sua mesa, você está se perguntando "Onde é que eu começo?"

## Forces
É surpreendente a frequência com que os projetos de reengenharia começam. Isso não só acontece depois de uma fusão de duas empresas, mas também encontramos projetos nos quais bibliotecas de código foram obtidas de empresas que mais tarde faliram,ou em que equipes de manutenção concluem seu projeto deixando um código muito valioso, mas incompreensível. É claro que a pergunta óbvia a ser feita é "Onde eu começo?". Acontece que essa é uma das questões cruciais a serem respondidas durante um projeto de reengenharia, e é por isso que dedicamos um capítulo inteiro à sua resposta.

Todos os padrões neste grupo podem ser aplicados aos estágios iniciais de um projeto de reengenharia: você está enfrentando um sistema completamente novo para você e, em alguns dias, deve determinar se algo pode ser feito com ele e apresentar um plano de como proceder. No entanto, fazer essa avaliação inicial é difícil, porque você precisa rapidamente de resultados precisos, considerando os efeitos de longo prazo de suas decisões. Para lidar com o conflito inerente entre efeitos rápidos, precisos e de longo prazo, os padrões neste grupo devem resolver as seguintes potências.

* Os sistemas legados são grandes e complexos.
A escala é sempre um problema quando lidamos com sistemas legados. Durante o projeto FAMOOS, enfrentamos sistemas que variam entre 500.000 linhas de C ++ e 2,5 milhões de linhas de Ada.
No entanto, há muito o que uma única equipe de reengenharia pode fazer e, quando o sistema legado é grande demais ou complexo demais, você não pode fazer o trabalho de uma só vez.
Consequentemente, divida o sistema em partes gerenciáveis, onde uma peça gerenciável é uma que você pode manipular com uma única equipe de reengenharia.

O quanto uma única equipe pode gerenciar varia com o objetivo do projeto de reengenharia, o estado do sistema original, a experiência e as habilidades de sua equipe e a cultura de sua organização. Nossas equipes consistiam de três a cinco pessoas e podiam lidar entrem  500.000 e um milhão de linhas de código. No entanto, esses números certamente terão que ser adaptados para o projeto de reengenharia que você está enfrentando. Como regra geral, suponha que uma única equipe possa refazer o código que puder escrever do zero. Melhore suas estimativas durante o projeto de reengenharia, mantendo registros de quanto sua equipe realmente fez a reengenharia.

Se você precisar dividir o código, fique o mais próximo possível da estrutura atual do sistema e da organização da equipe de manutenção. Depois de ter uma boa compreensão da estrutura do sistema, considere as alternativas mais adequadas para a meta do projeto.

* O tempo é escasso.
Perder tempo no início de um projeto tem consequências graves mais tarde. Isso é especialmente relevante durante a engenharia reversa, porque você se sente incerto e, em seguida, é tentador iniciar uma atividade que o manterá ocupado por algum tempo, em vez de abordar a raiz do problema. Consequentemente, considere o tempo como seu recurso mais precioso. Portanto, adie todas as atividades demoradas até mais tarde e use os primeiros dias do projeto para avaliar a viabilidade dos objetivos do projeto. Todos os padrões deste grupo destinam-se a identificar rapidamente as oportunidades e os riscos do seu projeto e, como tal, ajudarão você a definir a direção geral do projeto.

* As primeiras impressões são perigosas.
Tomar decisões importantes com base em conhecimento incompleto implica que há uma chance de você tomar a decisão errada. Não há como evitar esse risco durante o primeiro contato com o sistema, mas você pode minimizar o impacto se verificar sempre suas fontes.

* As pessoas têm agendas diferentes.
Normalmente, você se juntará a um grupo de pessoas onde vários membros terão muita experiência com o sistema para serem reprojetados. Talvez os membros da equipe de desenvolvimento original ainda estejam disponíveis ou talvez a equipe de reengenharia inclua pessoas que mantiveram o sistema por algum tempo. Pelo menos haverá usuários finais e gerentes que acreditam o suficiente neste sistema para solicitar um projeto de reengenharia. Você deve complementar a equipe com suas habilidades de reengenharia e experiência, portanto, você deve saber com quem está lidando.

Normalmente, seus novos colegas se dividem em três categorias. A primeira categoria são os fiéis, as pessoas que acreditam que a reengenharia é necessária e que você é capaz de (ajudá-los) fazê-lo. A segunda é a categoria dos céticos, que acreditam que todo esse negócio de reengenharia é apenas uma perda de tempo porque querem proteger seus empregos ou porque acham que todo o projeto deve começar do zero. A terceira categoria é a categoria dos "sitters", que não têm uma opinião forte sobre se essa reengenharia vai compensar, então eles apenas esperam e vêem o que acontece. Consequentemente, a fim de tornar o projeto um sucesso, você deve continuar convencendo os fiéis, ganhar crédito com os "sitters" e ter cuidado com os céticps.

## Visão geral
Perder tempo é o maior risco quando você tem seu primeiro contato com um sistema, portanto esses padrões devem ser aplicados durante um curto período de tempo, digamos uma semana. Após essa semana, você deve compreender os principais problemas e, com base nesse plano de conhecimento, realizar outras atividades ou, quando necessário, cancelar o projeto.

Os padrões "ChatWithTheMaintainers" e "InterviewDuringDemo" ajudarão você a se familiarizar com as pessoas envolvidas. Como regra geral, passe quatro dias para coletar informações e use o último dia da semana para compilar todas essas informações em um primeiro plano de projeto. Não há uma ordem restrita sobre aplicar os padrões, embora a ordem sugerida pela sequência no livro seja típica. No entanto, muitas vezes nos encontramos combinando fragmentos desses padrões por causa da necessidade de checar duplamente. Por exemplo, durante uma segunda reunião com os mantenedores, geralmente começamos com um "InterviewDuringDemo", mas fazemos perguntas sobre o que aprendemos em "ReadAllTheCodeInOneHour" e "SkimTheDocumentation". Além disso, após uma entrevista, verificamos rapidamente o código-fonte e a documentação para confirmar o que foi dito

Em certas situações, percebemos que alguns padrões não são aplicáveis devido à falta de recursos. Por exemplo, se todos os mantenedores tiverem saído da empresa, você não poderá usar o "ChatWithTheMaintainers". Além disso, alguns sistemas não possuem uma interface de usuário externa e, portanto, é inútil tentar um "InterviewDuringDemo" com um usuário final. Isso não é necessariamente um problema, porque alguns desses padrões podem ser irrelevantes para sua meta de projeto. No entanto, a ausência de recursos é um risco extra para o projeto e deve ser registrado como tal no primeiro plano do projeto.

## Qual o proximo

Depois de ter as informações necessárias, é hora de compilar o primeiro plano do projeto. Esse plano é muito semelhante aos planos que você normalmente usa ao lançar um projeto e, portanto, os modelos de documento padrão usados na sua empresa devem ser usados. Quando necessário, dobre as regras para incluir pelo menos os seguintes itens.

* Escopo do Projeto
Prepare uma breve descrição (meia página) do projeto, incluindo seu contexto, seus objetivos e os critérios que serão usados para verificar se você atingiu essas metas. "InvolveTheUsers" e "AgreeOnMaxims" para gravar essa parte do plano.

* Oportunidades
Identifique os fatores que você espera que contribuam para atingir as metas do projeto. Listar os itens que você descobriu durante o primeiro contato, como a disponibilidade de mantenedores qualificados e usuários avançados, a legibilidade do código-fonte ou a presença de documentação atualizada.

* Riscos
Considere elementos que podem causar problemas durante o curso do projeto. Listar os itens que você não encontrou ou onde a qualidade era inferior, como bibliotecas de código ausentes ou a ausência de suítes de teste. Se possível, inclua uma avaliação da probabilidade (improvável, possível, provável) e do impacto (alto, moderado, baixo) para cada risco. Atenção especial deve ser dada aos riscos críticos, ou seja, aqueles que são possíveis / prováveis e têm um impacto moderado / alto ou aqueles que são prováveis, mas têm um impacto baixo.

* Decisão ir / não-ir.
Em algum momento você terá que decidir se o projeto deve ser continuado ou cancelado. Use as oportunidades e os riscos acima para argumentar essa decisão.

* Atividades.
(No caso de uma decisão "ir") Prepare uma visão geral do próximo período, explicando como você pretende atingir a meta do projeto. Em uma visão de olho de peixe, as atividades de curto prazo são explicadas com detalhes consideráveis, enquanto para as atividades posteriores um esboço é suficiente. Muito provavelmente, as atividades de curto prazo corresponderão aos padrões descritos em \ charef {Compreensão Inicial} {InitialUnderstanding}. Para as atividades posteriores, verifique os capítulos subseqüentes.

A lista de atividades deve explorar as oportunidades e reduzir os riscos (críticos). Por exemplo, se você listar a presença de documentação atualizada como uma oportunidade e a ausência de um conjunto de testes como um risco crítico, planeje uma atividade que criará um conjunto de testes com base na documentação.
