
# Terceira Lista Metologias Ágeis

## 1. Quando você não recomendaria o uso de um método ágil para o desenvolvimento de um sistema de software ?

Não é recomendado a utilização de metodologias ágeis para sistemas
que necessitam de uma análise completa, pois uma abordagem dirigida
a planos é a melhor opção nesses casos.

## 2. Por que métodos como o Processo Unificado (UP) e Espiral não são considerados ágeis? E qual a diferença deles para o Modelo Waterfall ?

Questão repetida. [Segunda Lista questão 6](lista_2_primeira_unidade.md).

## 3. Extreme Programming expressa os requisitos dos usuários como estórias, com cada estória escrita em um cartão. Discuta as vantagens e desvantagens dessa abordagem para a descrição de requisitos

as principal vantagem em basear os requisitos em cenários ou estórias de clientes é a utilização
de um linguajar não técnico e simples, tornando fácil a comunicação entre os desenvolvedores e
o futuro dono do software. No entanto devido a sua informalidade, as estórias não
contém detalhes importantes da aplicação ou tecnicalidades, quando se é necessário capturar
essas informações, não é recomendando a utilização de estórias de usuários.

## 4. Explique por que o desenvolvimento test-first ajuda o programador a desenvolver um melhor entendimento dos requisitos do sistema. Quais são as potenciais dificuldades com o desenvolvimento test-first

Segundo KENT BECK autor de Test-driven-development (TDD): "Nenhum estudo demonstrou categoricamente a diferença entre TDD e qualquer uma das muitas alternativas de qualidade, produtividade ou diversão.",
Portanto não existe evidências ciêntificas que TDD ajuda no entendimento dos requisitos do sistema.
Dificuldades encontradas utilizando TDD, estão desde criação de testes em GUIs, testes em programação concorrente
e paralela, limitações quando não se é possível criar testes automatizados, **Código Legado**.

## 5. Como XP preconiza que devem ser os contratos de desenvolvimento de software ?

Escreva contratos para desenvolvimento de software que  fixa o tempo, custo e qualidade de código.
Dê preferência a uma sequência de contratos pequenos do que um único grande. O desenvolvedor deve
ter em mente que mudanças acontecem, não coloque preços abusivos por esses pedidos.

## 6. Quais as diferenças entre XP e Scrum ?

XP impõe práticas de programação, como a necessidade de duas pessoas por especialidade,
onde uma valida o código da outra e testes automáticos o quanto possível. Já o Scrum não impõe
práticas de programação e nem a necessidade de duas pessoas por especialidade. O XP foca em
sugerir disciplinas para um engenheiro de software, já o Scrum foca em disciplinas que buscam
tornar o desenvolvimento mais previsível possível utilizando dados empíricos, em um ambiente
onde as mudanças acontecem com frequência.

## 7. Times Scrum são ditos cross-funcionais e auto-organizáveis. Por quê? Defina esses termos

- times cross-funcionais ou multidisciplinares, é um time que possui integrantes de diferentes
áreas, mas que se complementam para o desenvolvimento da solução

- time auto-organizável, é um time que possui a inteligência e autonomia para decidir como o problema
será resolvido.

Um time scrum é dito como multidisciplinar, nele está contido o Scrum Master, o Dono do produto
(ou seu representante) e todos os especialistas necessários para desenvolver o produto, especialistas
que não necessáriamente atuam na mesma área. É também dito como auto-organizável, uma vez que é o time
que decide quais estórias de usuário serão implementadas e por quem serão implementadas.

## 8. Qual a diferença entre as histórias do “topo” e do “fundo” do Backlog do Produto, em Scrum ?

O backlog do produto é um artefato que possui a seguinte organização: itens mais ao topo são itens mais
importantes e mais detalhados e os itens mais abaixo são menos importantes e menos detalhados. Portanto
um item ao topo deve ser mais urgente e melhor compreendido pela equipe e item mais abaixo deve ser
menos urgente e menos compreendido.

## 9. O que são e para que servem story points ?

Com o objetivo de estimar o tempo gasto para cada estória de usuário, foi criado o story points que é
um valor inteiro que representa o quão complexo é implementar aquela estória quando comparado as outras
estórias, ou seja, se uma estória A tiver 2 story points e uma estória B tiver 5 story points então
A é mais fácil de implementar do que B. Uma vez que todas as estórias possui seu valor e time começa
a realizar as estórias é possível mensurar a **velocidade** do time ou o quanto story points ele
consegue realizar por sprint, além de cada sprint, tornar mais previsível em quanto tempo o time consegue finalizar cada estória.

## 10. Em Scrum, qual a diferença entre uma sprint review e uma retrospectiva ?

A sprint review é uma reunião do time com os stakeholders e product owner, para avaliar o produto
em desenvolvimento. Já a retrospectiva é a reunião para avaliar o time durante o desenvolvimento.

## 11. Um sprint pode ser cancelado? Se sim, por quem e por qual motivo? Para responder a essa questão, consulte antes o [Scrum Guide](https://www.scrumguides.org/), que é o guia que documenta a versão oficial de Scrum

Uma Sprint pode ser cancelada se a Meta da Sprint se tornar obsoleta. Apenas o Product
Owner tem autoridade para cancelar a Sprint.

## 12. Escreva estórias de usuário para o sistema que você irá desenvolver como projeto da disciplina

[Next restaurant user storie](https://github.com/samuel-cavalcanti/next-restaurant/blob/main/user_stories.md)

## 13. Suponha dois times, A e B, atuando em projetos diferentes, contratados por empresas distintas, sem conexões entre eles. Porém, ambos os times adotam sprints de 15 dias e ambos possuem 5 desenvolvedores. Nos seus projetos, o time A considera que sua velocidade é de 24 pontos. Já o time B assume uma velocidade de 16 pontos. Pode-se afirmar que A é 50% mais produtivo que B? Justifique sua resposta

Não. Segundo a pratica do Scrum é fortemente baseada no empirismo, cada projeto possui sua dificuldade,
sua realidade, somente o que já aconteceu em um projeto pode usado para a tomada de decisão.

## 14. Quais são as principais diferenças entre Scrum e Kanban ?

O kanban funciona mais como ferramenta de visualização, trabalha mais a transparência para a equipe. Mas o seu uso tem um ritmo contínuo, não tem funções nas equipes, é aberto para fazer mudanças em qualquer momento e as entregas vai da escolha da equipe. Já o Scrum é melhor estruturado, o ritmo se segue com as sprints que tem tempos exatos, existe as funções dentro das equipes (Product Owner, Scrum Master, Time de Desenvolvimento), existe regras para se fazer mudanças durante sprits, a cada final de sprint precisa ter uma validação do que foi realizado.

## 15. O artigo [“Development and Deployment at Facebook”](development-and-deployment-at-facebook.pdf) apresenta os métodos e práticas de desenvolvimento de software usados no Facebook. Na primeira seção (páginas 2-3; figura 2), os autores fazem uma distinção entre alguns métodos de desenvolvimento, baseando-se na frequência com que versões de um sistema são liberadas para uso quando se adota cada um deles. Complete a seguinte tabela informando a frequência de releases mencionada no artigo para alguns métodos e políticas de liberação de software

| Método              | Frequência de novas releases|
| --------------------|:---------------------------:|
| waterfall           | entrega única               |
| evolucionário       | meses                       |
| ágil                | semanas                     |
| facebook            | entrega única a cada dia    |
| deployment contínuo | horas                       |
