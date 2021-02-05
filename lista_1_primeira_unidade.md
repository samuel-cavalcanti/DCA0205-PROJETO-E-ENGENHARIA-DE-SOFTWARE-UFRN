# Primeira Lista Projeto e Engenharia de Software

1. Diferencie requisitos funcionais de requisitos não-funcionais.

        Requisitos Funcionais não requisitos que o cliente consegue reconhecer
        e ou interagir com ele, em determinada aplicação como por exemplo,
        a realização de um login no sistema.
        Já requisitos não funcionais são as features do sistema que o usuário
        não vê, como por exemplo, um banco de dados relacional ou não, ou
        features voltados a segurança que garantem a integridade dos dados/ 

2. Explique porque testes podem ser considerados tanto uma atividade de verificação como de validação de software. Qual tipo de teste é mais adequado se o objetivo for verificação ?
Qual tipo de teste é mais adequado se o objetivo for validar um sistema de software ?

                Um software é considerado validado quando o mesmo cumpre o as expectativas
                do cliente, para garantir que isso aconteça é muito comum existir testes
                de release onde uma equipe de teste independente testa uma versão completa
                do sistema e verifica se o sistema atende aos requisitos dos stakeholders
                ou pode existir testes de usuários, onde potenciais usuários do sistema
                testam o sistema e reportam bugs e comportamentos inadequados do sistema.

                Um software é considerado verificado quando o mesmo possui testes que
                demostram o funcionamento de cada unidade ou classe, módulo e sistema,
                onde o testes do sistemas são testes que demonstram que a relações entre
                os módulos estão acontecendo como o esperado. Para verificar o sistema
                é muito comúm a utilização de testes automatizados, tanto para a 
                a verificação de classes, módulos.  

3. Por que testes não conseguem provar a ausência de bugs ?

        Para provar que uma aplicação funciona você Obrigatoriamente,
        necessita provar matemáticamente que para todas as entradas
        possíveis o sistema responte corretamente. Testes são um meio
        ciêntifico de mitigar essa falta de teoremas matemáticos que
        prove que o seu software funciona, uma vez que ele demostra para
        um pequeno grupo de entradas que o seu sistema responde corretamente.

4. Suponha um programa que tenha uma única entrada: um inteiro de 64 bits. Em um teste exaustivo, temos que testar esse programa com todos os possíveis inteiros (logo, 264). Se cada teste levar 1 nanossegundo (10-9 segundos),quanto tempo levará esse teste exaustivo ?

        Sabendo que um numero inteiro de 64 bits pode representar até
        18446744073709551616 (2^64) números possíveis, se cada número demora
        10^⁻9 segundos então: (2^64)*10^-9  = 18446744073.709553 segundos 
        é o tempo total necessário para rodar o teste em anos seria de
        584.554531 anos ( praticamente impossível de se verificar)

5. Se considerarmos o contexto histórico, por que foi natural que os primeiros processos de desenvolvimento de software tivessem características sequenciais e fossem baseados em planejamento e documentação detalhados ?

        O Modelo Sequencial Linear também chamado de cascata, foi o primeiro modelo mais
        amplamente usado devido ao fato da sua fácil compreensão, fácil estimação de tempo.
        Em uma época onde não se tinha muito conhecimento sobre programação de software,
        simplicidade no modelo de desenvolvimento reina. Segundo McCONNEL, Steve em
        Rapid development. Redmond, WA: Microsoft Press, 1996. Cascata é aconselhado quando
        sua équipe é tecnicamente fraca. 

6. Refactoring é uma transformação de código que preserva comportamento. Qual o
significado da expressão preservar comportamento? Na prática, qual restrição ela impõe a uma operação de refactoring ?

        Ná pratica, a medida que um sistema vai aumentando a sua complexidade
        o código fonte fica ainda maior e como esse código é mantido
        por seres humanos, logo existe uma necessidade de que o código fonte
        se torne o mais legível quanto possível, refactoring é uma operação
        altera o código melhorando a sua visibilidade visando não alterar o
        comportamento do sistema, no entanto fazer alterações no código pode
        ser perigoso, uma vez mudanças pode ocasionar bugs e outros
        comportamentos inesperados, na prática, para mitigar esses efeitos
        nos consideramos que um refactoring foi finalizando quando o mesmo
        código passa nos testes que demostra o comportamento do sistema,
        geralmente feitos antes de refactoring.

7. Dê exemplos de sistemas A (Acute, ou críticos) e B (Business, ou comerciais) com os quais já tenha interagido.

     Sistemas A:  [cinemática de um braço robótico](https://github.com/samuel-cavalcanti/Self-Learning-in-the-Inverse-Kinematics-of-Robotic-Arm),
     [Robô seguidor de linha (Projeto URA)](https://github.com/samuel-cavalcanti/Toninho),  
     Sistemas B: [Elasticsearch, Logstash e Kibana](https://www.elastic.co/pt/what-is/elk-stack)

8. Dê exemplos de sistemas C (casuais) que você já tenha desenvolvido.

- [__rust-activities__ Resolvendo atividades propostas pelo livro The Rust Programming language](https://github.com/samuel-cavalcanti/rust-activities)  
- [__exemplos_tdd__ Implementações dos códigos do livro TDD Desenvolvimento Guiado por Testes kent beck](https://github.com/samuel-cavalcanti/exemplos_tdd)  
- [__DuckDuckGo-Image-Search-API__ API para Download de imagens no https://duckduckgo.com/](https://github.com/samuel-cavalcanti/DuckDuckGo-Image-Search-API)  
- [__FindByColor__ Com a Proposta de axilar as aulas de Computação Numérica na Universidade Federal do Rio Grande do Norte. Foi desenvolvido um aplicativo que possui a função de rastrear um determinado Objeto pela sua cor](https://play.google.com/store/apps/details?id=cavalcanti.samuel.findbycolor2&hl=pt_BR&gl=US)

- [__teddy bear filter__ Teddy Bear Filter é um Bot no telegram que recebe uma imagem e diz se é ou não um conteúdo pornográfico](https://github.com/samuel-cavalcanti/teddy_bear_filter)  

- [__an-chrome-extension__ Essa é uma aplicação que utiliza os classificadores do tensor hub e o framework Tensorflow JS para a criação de uma extensão chrome que filtre toda imagens](https://github.com/samuel-cavalcanti/an-chrome-extension)  

- [__Fuzzy and reinforment learning__ Desviando de obstáculos com aprendizado por reforço e logica fuzzy](https://github.com/samuel-cavalcanti/Fuzzy-and-reinforment-learning)

- [__web scraping google geocoder__ Uma aplicação simples que utilizar Selenium e Beautiful Soup para fazer geocoding com a API da google (eticamente duvidoso)](https://github.com/samuel-cavalcanti/web_scraping_google_geocoder)

- [__DATAJS__ Visualizador para a Rede neural SOM (kohonen map)](https://github.com/samuel-cavalcanti/DataJS)

- São por volta 50 repositories e nem listei os cursos de harvard.

9. Em 2015, descobriu-se que o software instalado em mais de 11 milhões de carros da
Volkswagen detectava quando eles estavam sendo testados em um laboratório de
certificação. Nessas situações, o carro emitia poluentes dentro das normas legais. Fora do
laboratório, emitia-se mais poluentes, para melhorar o desempenho. Ou seja, o código
incluía uma estrutura de decisão como a seguinte (meramente ilustrativa, para fins deste
exercício):  

```
if "Carro sendo testado em um laboratório"
        "Emita poluentes dentro das normas"
else
        "Emita poluentes fora das normas"

```

O que você faria se seu chefe pedisse para escrever um if como o acima ?

Criar, usar softwares que desrespeitam as leis atuais ? COM CERTEZA !  
Possuo um série de projetos open source e closed source que claramente
desrespeita as leis de propriedade intelectual como meu:
- [(Desatualizado) My libgen calibre plugin](https://github.com/samuel-cavalcanti/MY-libgen-calibre-plugin) que facilida o download de livros piratas na internet

- [scrip que baixa livro no Passei Direto](https://github.com/samuel-cavalcanti/scripts/tree/master/livroPasseiDireto) um exemplo de código que mostra como baixar livros e documentos no [passei direto](https://www.passeidireto.com/)

- e muitos outros que devem estar por ai... no meu github :smiley:

Mas eu escreveria o if a cima ? NUNCA, ~~enfim a hipocrisia~~

Eu não sigo regras porque são regras, eu sigo quando vejo que elas fazem sentido, poluir o meu ambiente ou denegrir o proxímo é algo que destrói uma
sociedade ou o outro, então eu não sigo ordens ou regras porque são regras.
Não me importo se não é "certo" as pessoas terem acesso a livros que não
compraram, as consequência das pessoas terem acesso a artigos e livros sem
pagar vale muito mais apena.
