# Segunda Lista Projeto e Engenharia de Software

## 1. Explique por que o desenvolvimento incremental é o método mais eficaz para o desenvolvimento de sistemas de software de negócios. Por que esse modelo é menos adequado para a engenharia de sistemas de tempo real ?

Em sistemas de tempo real, muito provávelmente não é possível a
realização da implementação e ou validação sem antes a realização
total da etapa de especificação, tornando o desenvolvimento
inevitávelmente sequencial. Já no sistemas de software de negócios
é muito provável que a exigência do tempo de produção seja o menor
possível aliado a uma maior probabilidade de que os requisitos iniciais
do projeto mude antes mesmo do software ser finalizado, sendo
assim, possuir versões intermediárias do software algo vantajoso,
mesmo que não cumprindo totalmente com os requisitos.

## 2. Considere o modelo de processo baseado em reúso da Figura abaixo. Explique por que, nesse processo, é essencial ter duas atividades distintas de engenharia de requisitos

![Processo baseado em Reúso](processo_baseado_em_reúso.png)  

Em um modelo de processo com um foco em reaproveitamento de código como um
desenvolvimento de um framework por exemplo, é comum ter uma etapa durante
o desenvolvimento onde a equipe busca encontrar padrões entre os componentes,
verificar se se criação de novos componentes é algo necessário ou se pode reaproveitar
um componente já criado, nesse tipo de modelo, mitigar qualquer modificação
da arquitetura do software é normalmente tão importante quando gerar o
software que atenda os requisitos. Em desenvolvimento de um framework ter um
passo para analisar a arquitetura ajuda a reduzir o número de breaking changes
que uma nova realise do seu software pode conter.

## 3. Descreva as principais atividades do processo de projeto de software e as saídas dessas atividades  

   ![](modelo_geral_de_processo.png)

   1. __Projeto de arquitetura__. No qual você pode identificar a estrutura geral do sistema, os componentes principais (algumas vezes, chamados subsistemas ou módulos), seus relacionamentos e como eles são distribuídos.  
   _Saída:_ separação de responsabilidades em forma de sistemas Módulos ou subsistemas e a forma como eles se se relacionam.

   1. __Projeto de interface__. No qual você define as interfaces entre os componentes do sistema. Essa especificação de interface deve ser inequívoca. Com uma interface precisa, um componente pode ser usado de maneira que outros componentes não precisam saber como ele é implementado. Uma vez que as especificações de interface são acordadas, os componentes podem ser projetados e desenvolvidos simultaneamente.
   _Saída:_ Interfaces, ou a separação de responsabilidades dentro de um módulo ou subsistemas.

   1. __Projeto de componentes__. no qual você toma cada componente do sistema e projeta seu funcionamento. Pode-se tratar de uma simples declaração da funcionalidade que se espera implementar com o projeto específico para cada programador. Pode, também, ser uma lista de alterações a serem feitas em um componente reusável ou um modelo de projeto detalhado. O modelo de projeto pode ser usado para gerar automaticamente uma implementação.  
   _Saída_: Os detalhes da implementação, a forma como é executada ou realizada a responsabilidade.

   1. __Projeto de banco de dados__. No qual você projeta as estruturas de dados do sistema e como eles devem ser representados em um banco de dados. Novamente, o trabalho aqui depende da existência de um banco de dados a ser reusado ou da criação de um novo banco de dados.  
   _Saída_: A forma como é representado as entidades do sistema e como elas serão armazenadas,
   caso precise.

## 4. Explique por que os sistemas desenvolvidos como protótipos normalmente não devem ser usados como sistemas de produção

Um protótipo possui o objetivo, validar uma ídeia e demonstrar o
funcionamento dela, o autor do protótipo possui a liberdade de não
se preocupar com as boas práticas de desenvolvimento durante a criação do protótipo,
caso opte por essa abordagem, muito provavélmente
inserir novas funcionalidades ou a manutenção dessa aplicação serão
praticamente inviáveis e não é recomendado por em produção, um software com a manutenção e
a inserção de novas features comprometidas.  

## 5. Quais são as vantagens de proporcionar visões estáticas e dinâmicas do processo de software, assim como no Rational Unified Process ?

A vantagem de proporcionar visões estáticas e dinâmicas é que as fases
do processo de desenvolvimento não estão associadas a workflows específicos. Ao menos em princípio, todos os workflows do RUP podem estar
ativos em todas as fases do processo. Nas fases iniciais provavelmente
maiores esforços serão empenhados em workflows, como modelagem de
negócios e requisitos, e, nas fases posteriores, no teste e na implantação.

## 6. Por que métodos como o Processo Unificado (UP) e Espiral não são considerados ágeis? E qual a diferença deles para o Modelo Waterfall ?

**_“Metodologia ágil é uma abordagem para gerenciamento de projetos de alta imprevisibilidade, para construir software de maneira incremental e iterativa, apoiada em trabalho de equipe”._**  
[O rup não é um processo ágil por moamello](https://iblogdomoa.wordpress.com/2011/10/20/o-rup-nao-e-um-processo-agil/)  

Metodologias ágeis se baseando que não há uma sequencia de procedimentos
ótimos para o desenvolvimento de software devido a alta imprevisibilidade.
Portanto uma metodologia com o espiral ou UP não é ágil uma vez que, eles
possuem formulados uma sequencia de passos determinísticos para cada
momento do desenvolvimento. A diferença do UP ou espiral para o Waterfall
a é flexibilidade que existe no espiral e UP, uma vez que não existe uma
óbrigatoriedade de terminar de terminar uma etapa para começar a outra.
Por exemplo não existe a obrigatóriedade de terminar Especificação de software para começar a implementação

Em geral as metodologias ágeis vão justificar seu modelo através da natureza do processo de desenvolvimento, isto é, o processo é empírico, não é definido, no sentido de que não é determinado, compreendido. Portanto não tem uma formulação ou descrição conhecida e daí não pode ser prescritivo, quer dizer, não há como designar passos e tarefas em sequência para realizar um projeto pois não há um caminho ótimo, conhecido de antemão, para executá-lo. Reagimos às mudanças. Nessa situação é ocioso escrever o processo e detalhá-lo definindo um descritivo, a realidade mudará tudo que definirmos.

## 7. Historicamente, a introdução de tecnologia provocou mudanças profundas no mercado de trabalho e, pelo menos temporariamente, deixou muitas pessoas desempregadas. Discuta se a introdução da automação extensiva em processos pode vir a ter as mesmas consequências para os engenheiros de software. Se sua resposta for não, justifique. Se você acha que sim, que vai reduzir as oportunidades de emprego, é ética a resistência passiva ou ativa, pelos engenheiros afetados, à introdução dessa tecnologia ?

Sim ou não ambos estão certos. A figura da automação sem contexto especifico pode proporcionar o bem estar, melhor qualidade de vida, melhor qualidade do trabalho e mais empregos na área de desenvolvimento de software como também pode ser utilizado para nós prejudicar. Um exemplo positivo
podemos citar o desenvolvimento de ferramentas que verificação a qualidade do código
testado com o [codecov](https://codecov.io/) ou outras ferramentas de DevOps que tornaram o trabalho de testar software muito menos repetitivo. Um exemplo
negativo foi a utilização de [inteligencia artificial para a automação de seleção de currículos pode ser sexista](https://olhardigital.com.br/2018/10/10/noticias/inteligencia-artificial-da-amazon-exercitava-preconceito/). (Utilização de engenheiros de software em seleções de empregos na sua respectiva área é uma prática muito comum). Automação de um processo se
dá através das criações de técnicas e tecnologias, a forma como o usuário utiliza ou a finalidade da criação dessas técnicas e tecnologias dizem se automação é ou será prejudicial ou benéfica para um conjunto de indivíduos.
Em uma boa parte das aplicações ela é prejudicial para alguns e benéfica para outros. Em relação a ética, se é ético automatizar ou não é ainda mais complexo definir regras, pois ética em si, varia com tempo, espaço,
cultura, número de pessoas, e diversas outras variáveis desconhecidas, ou seja, ética em si é complexo, aplicar ética, em um processo não causal é
atualmente impossível tomar uma decisão satisfatória baseado em leis físicas, pois atualmente não existem tais leis.

- __sistemas Causais__: sistemas causais são sistemas que "sabendo o passado",
tendo "informações do presente" é possível "prever o futuro". Atualmente só existem
leis físicas causais. [Sinais e Sistemas Lineares](https://www.amazon.com.br/Sinais-Sistemas-Lineares-B-P-Lathi-ebook/dp/B016V9PZYE)

__OBS:__ se você está com medo de uma certa IA programando, significa que você é um péssimo programador e eu não gosto de você (como programador).


## Referências:

[SOMMERVILLE Engenharia de Software](engenhariaSoftwareSommerville.pdf)

[SINAIS E SISTEMAS LINEARES SEGUNDA EDIÇÃO](Sinais%20e%20Sistemas%20Lineares%20-%202.ed_%20-%20B.%20P.%20Lathi.pdf)