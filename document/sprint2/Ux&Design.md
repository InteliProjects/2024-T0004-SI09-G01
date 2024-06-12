# Sumário

[1. Mockup](#c1)

[2. Fragilidade e Dificuldade no processo](#c2)

[3. Pontos que poderia ser implementado e Plano de Ação](#c3)

[4. Design System](#c4)

<br>

# <a name="c1"></a>1. Mockup

Link do Figma: https://www.figma.com/file/X7zrBZLA2KC8Ot9aL15BCg/Wireframe?type=design&node-id=166%3A2892&mode=design&t=q39d1LzvGq6LphSs-1

## 1.1 Telas em comum

&emsp;&emsp; A primeira tela com a qual o usuário terá contato é a **Tela de Login**, responsável por validar a entrada, principalmente para diferenciar o acesso do CEO/VP do RH e do líder de cada área. Do lado esquerdo da tela, podemos observar uma imagem de um Fusca, representando o grupo que desenvolveu o projeto, enquanto do lado direito estão os campos de entrada para o nome do usuário e a senha. Esta tela foi desenvolvida em duas opções: _Light_ e _Dark_, que podem ser escolhidas na tela de Configurações a seguir.

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/71dbed0b-6dfa-48dc-8986-4d6e004d95ba)
Figura 01: Tela de Login - Modo Light <br>
Fonte: Autoria própria

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/7633164a-269f-4075-bd19-e21a12df4c28)
Figura 02: Tela de Login - Modo Dark <br>
Fonte: Autoria própria

&emsp;&emsp; A segunda tela compartilhada pelos dois tipos de acesso é a **Tela de Configuração**, na qual é possível visualizar o nome de usuário e o cargo do usuário na Volkswagen. Além disso, é possível selecionar o modo de visualização das informações: _Light_ e _Dark_. Essa opção será exibida em um modal quando o usuário selecionar "Configurações" no canto inferior esquerdo.

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/875a98fd-4565-48be-84af-7746a6e14b7a)
Figura 03: Modal de Configuração - Modo Light <br>
Fonte: Autoria própria

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/3312435f-ca88-4a42-b355-0455d0b7d4ea)
Figura 04: Modal de Configuração - Modo Dark <br>
Fonte: Autoria própria

## 1.2 Visão CEO / VP de RH

&emsp;&emsp; Com o acesso validado na **Tela de Login**, o usuário terá acesso a uma tela inicial, denominada Home. Esta tela exibe as principais informações das duas pesquisas de satisfação utilizadas pela empresa: STIBA e GPTW. Na primeira seção, é possível visualizar os indicadores das pesquisas: STIBA Volkswagen, GPTW Volkswagen, STIBA por área e GPTW por Dimensões. As áreas mostradas no STIBA referem-se a todas as áreas de nível 1 que a empresa possui, enquanto as dimensões do GPTW avaliadas nas empresas incluem: Credibilidade, Respeito, Imparcialidade, Orgulho e Camaradagem.

&emsp;&emsp; Na segunda seção, encontra-se o gráfico principal da tela, no qual o usuário pode visualizar as notas e o engajamento do STIBA de cada área da empresa. Isso permite observar a diferença entre as duas variáveis em uma área específica, como por exemplo B-X. A ideia é que, durante a implementação do mockup, ao passar o mouse sobre cada coluna, o nome completo da área seja exibido. Essa é a última tela que foi desenvolvida com a opção Dark, pois a validação com o parceiro ocorre primeiro e depois serão desenvolvidas as demais telas.

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/67b4fc3d-594a-4cb6-ba40-ff915e5ea07d)
Figura 05: Tela Home - CEO - Modo Light <br>
Fonte: Autoria própria

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/3d5dfd1a-5449-4c25-9850-4f637a88b04a)
Figura 06: Tela Home - CEO - Modo Dark <br>
Fonte: Autoria própria

&emsp;&emsp; No header de todas as páginas, é possível navegar entre elas. Se o usuário clicar em "Saúde Mental", será direcionado para a tela abaixo. Esta tela é dividida em três seções:

&emsp;&emsp; Na primeira seção, são apresentados os principais indicadores sobre saúde mental aos quais a empresa tem acesso. Isso inclui os seguintes indicadores: Dias Abonados, CID (Classificação Estatística Internacional de Doenças e Problemas Relacionados com a Saúde) mais recorrente e Atestados. O primeiro indicador soma todos os dias abonados devido a questões de saúde mental (CID começando com "F"), enquanto ao lado é exibido o CID mais recorrente em 2023 entre todos os colaboradores da Volkswagen. Abaixo desses indicadores, são fornecidas informações mais granulares, como a quantidade de dias abonados por mês e a relação dos dias com o CID. É importante destacar que será implementado um modelo ARIMA para prever quantos dias abonados a empresa poderá ter em janeiro.

&emsp;&emsp; Do lado direito da tela, as primeiras informações referem-se à quantidade de atestados que a empresa possui relacionados à saúde mental. É relevante lembrar que essa solução foi implementada com dados filtrados pelo CID "F", portanto, se a empresa deseja continuar com o projeto, é crucial prestar atenção nos dados implementados. O primeiro indicador soma todos os atestados, enquanto o segundo demonstra qual unidade possui a maior parte desses atestados. O gráfico abaixo permite visualizar todos os meses de 2023 e a quantidade de atestados registrados em cada período. O último conjunto de informações focaliza no ZenKlub, uma plataforma de terapia parceira, que disponibiliza o número de sessões realizadas pela empresa em 2023 e como essa distribuição é feita por fábrica.

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/39d9754f-f89d-4c13-aeec-6021c7820eb7)
Figura 07: Tela Saúde Mental - CEO - Modo Light <br>
Fonte: Autoria própria

&emsp;&emsp; Todas as telas explicadas anteriormente foram desenvolvidas também em mobile. Porém essa visualização ocorre de uma forma diferente, ela foi pensada para situações diárias, ou seja, momentos de alinhamento com o time, faz mais sentido visualizar os indicadores de cada dado. Abaixo, é possível visualizar as duas telas desenvolvidas para a visão do CEO / VP do RH. 

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/204ac8d0-a6dc-423e-91ca-2907d84c3f46)
Figura 08: Telas Mobile - CEO - Modo Light <br>
Fonte: Autoria própria

## 1.3 Visão Líder

&emsp;&emsp; No momento em que o líder tiver o acesso validado na Tela de Login, ele será direcionado à Home, onde poderá visualizar todas as informações relacionadas às pesquisas de satisfação (STIBA e GPTW). Os primeiros indicadores no lado esquerdo da tela concentram-se na nota e no engajamento do STIBA na área daquele líder, enquanto ao lado é possível visualizar a nota da empresa, permitindo assim uma comparação entre a área e a empresa como um todo.

&emsp;&emsp; Abaixo dessas informações, encontram-se dois componentes distintos. O primeiro é um resumo das informações sobre os colaboradores, incluindo a média de idade, a quantidade de colaboradores afastados e de férias, além do total de colaboradores. Ao lado, estão listadas todas as dimensões do GPTW e as respectivas notas da empresa em 2023. Este último dado é relevante, pois a nota é construída pela cultura de cada área, e para isso os líderes também precisam implementá-la. Por último, do lado direito, são exibidas duas tabelas: a primeira lista as 5 perguntas com as maiores notas no STIBA, enquanto a segunda apresenta as 10 piores perguntas. É importante destacar que o cálculo dessas notas foi feito utilizando a média dos valores de toda a área.

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/4ca59027-0b37-4d61-9fbc-caf329482113)
Figura 09: Tela Home - Líder - Modo Light <br>
Fonte: Autoria própria

&emsp;&emsp; Por fim, temos a Visão de Saúde Mental da área daquele usuário, dividida em 4 partes, cada uma focando em um tipo de dado disponível. A primeira parte apresenta todas as informações sobre os atestados, com a principal ideia de granularizar as informações desde a área geral até o colaborador individual. Esta abordagem também se aplica aos dias abonados. Os gráficos serão alimentados por um modelo ARIMA para prever o valor do próximo mês antes de sua ocorrência. Além disso, é possível visualizar os dados do ZenKlub, como a quantidade de sessões, a divisão por mês e a utilização por alguns colaboradores.

&emsp;&emsp; Por último, temos a correlação de todos esses dados por colaborador. No lado esquerdo, estão representadas essas informações para o ano de 2022 (Dias abonados X Atestados), enquanto no lado direito estão para 2023 (Dias abonados X Atestados X ZenKlub). É relevante notar que o último gráfico utiliza o tamanho das bolhas para representar a quantidade de sessões do ZenKlub.

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/fd04fe15-bb70-4e01-bee5-572adce281e6)
Figura 10: Tela Saúde Mental - Líder - Modo Light <br>
Fonte: Autoria própria

&emsp;&emsp; Todas as telas explicadas anteriormente foram desenvolvidas também em mobile. Porém essa visualização ocorre de uma forma diferente, ela foi pensada para situações diárias, ou seja, momentos de alinhamento com o time, faz mais sentido visualizar os indicadores de cada dado. Abaixo, é possível visualizar as duas telas desenvolvidas para a visão do Líder. 

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/5fc4de1b-5575-4da0-b8f1-69ff80fb063d)
Figura 11: Telas Mobile - Líder - Modo Light <br>
Fonte: Autoria própria

# <a name="c2"></a>2. Fragilidade e Dificuldade no processo 

&emsp;&emsp; A grande dificuldade enfrentada pelo time com o Mockup foi a necessidade de revisar os dados para compreender quais gráficos poderiam ser construídos e identificar possíveis correlações entre eles. Além disso, o parceiro mencionou que eles sempre utilizaram o Excel como ferramenta de geração de gráficos. Por esse motivo, tentamos manter os tipos de gráficos semelhantes, ou seja, mais simples. Essa abordagem visa facilitar a transição e garantir uma experiência mais fluida para o usuário final.

# <a name="c3"></a>3. Pontos que poderia ser implementado 

&emsp;&emsp; Alguns pontos que podem ser implementados no momento da criação do Front-End incluem: Mudança dinâmica de acordo com os filtros e Interação com os gráficos. O primeiro ponto será abordado durante a implementação do Mockup. Quando o usuário selecionar que deseja visualizar apenas informações sobre o STIBA, somente os gráficos relacionados a essa pesquisa serão exibidos. Já o segundo ponto será realizado por meio da utilização do Material UI. Com essa ferramenta, ao passar o mouse sobre o gráfico, os valores de X e Y serão mostrados, fornecendo uma interação mais detalhada e informativa aos usuários. Essas implementações visam melhorar a experiência do usuário e tornar a visualização dos dados mais intuitiva e eficiente.

&emsp;&emsp; O nosso plano de ação para o desenvolvimento desses pontos a serem implementados são: 1. Estudar como podemos realizar a utilização de filtros no Angular e 2. Utilização do _Material UI_ para realizar o _hover_ nos gráficos. 

# <a name="c4"></a>4. Design System

&emsp;&emsp; Um Design System é uma coleção de padrões, diretrizes, componentes e ferramentas utilizadas para garantir consistência e eficiência no processo de design e desenvolvimento de produtos digitais. O grupo está utilizando o Design System da Volkswagen, e ele é um exemplo notável na indústria automotiva. Com uma ênfase na simplicidade, acessibilidade e usabilidade, o Design System reflete os valores da marca, proporcionando uma experiência coesa e intuitiva para os usuários em todos os seus aplicativos, sites e interfaces digitais. Com isso, estamos utilizando os padrões da empresa abaixo para o desenvolvimento da nossa solução. 

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/4929c4ce-064c-476b-b043-279e413d7ee4)
Figura 12: Design System <br>
Fonte: Baseado no Manual da Marca - Volkswagen

