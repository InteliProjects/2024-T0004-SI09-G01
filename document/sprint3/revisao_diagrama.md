# Sumário

[1. Diagrama de Classe](#c1)

[2. Diagrama de Caso de Uso](#c2)

[3. Diagrama de Componente](#c3)

[4. Referências](#c4)

<br>

# <a name="c1"></a> 1. Diagrama de Classe

&emsp;&emsp; A criação do diagrama tem como objetivo modelar os objetos e definir os relacionamentos que irão compor o sistema. O diagrama facilita a construção da solução e auxilia o entendimento de seu funcionamento. Para esta solução foi realizado as modelagens abaixo, tanto para o frontend/web quanto para o backend . 

## 1.1 Diagrama de classe(backend)


![DiagramaClasse_G1_backend drawio](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99191485/428a330f-1726-459c-aeb0-f14bb26b0cfa)
<br> Figura 1: Diagrama UML Classes - Backend <br>
Fonte: Elaboração própria

&emsp;&emsp; Sobre as classes criadas para o diagrama e a sua estrutura, vale ressaltar que:

- _StibaPerguntas_,_GptwPerguntas_: Classes responsáveis por elencar as perguntas de suas respectivas pesquisas, e a nota fornecida para cada pergunta;

- _StibaInfo_, _GptwInfo_: Classes responsáveis por elencar os dados coletados pelas pesquisas da GPTW e Stiba;

- _CidInfo_: Responsável por representar as informações sobre os atestados entregues a empresa;

- _Unidade_: Classe para representar cada unidade, associando a ela os resultados obtidos de cada pesquisa;

- _Diretoria_: Classe para representar cada diretoria, e associar as Unidades pertencentes a cada diretoria;

- _ZenKlubInfo_: Classe para representar informações sobre o Zenklub.


## 1.2 Diagrama de classe(frontend) 


![DiagramaG3ClasseFront drawio](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99202408/4b5c3df7-997c-4a41-9117-cf619f1f75cc)
<br> Figura 2: Diagrama UML Classes - Frontend <br>
Fonte: Elaboração própria

&emsp;&emsp; Sobre esse diagrama vale mencionar que as classes referentes às pesquisas se mantém, uma vez que serão utilizadas para lidar com os dados que serão recebidos do backend da solução. Mas além delas algumas novas classes foram adicionadas, sendo elas:

- _Gráficos_: responsável por definir as características do gráfico e gerenciar as informações que serão _plotadas_ por eles;

- _Dashboard_: Classe utilizada para elencar quais gráficos serão de cada dashboard e o disponibilizar;

- _Usuário_: Classe que representa o usuário que irá acessar o dashboard, gerenciando seus dados e credenciais.


# <a name="c2"></a> 2. Diagrama de caso de uso 

&emsp;&emsp; O diagrama de caso de uso é uma representação gráfica que descreve as interações entre os usuários (atores) e um sistema de software. Ele é usado para capturar os requisitos funcionais do sistema e entender como os usuários interagem com ele. No diagrama abaixo, pode-se observar que os atores são representados por ícones (como figuras humanas) e os casos de uso são representados por retângulos. As linhas conectam os atores aos casos de uso correspondentes, mostrando quem realiza quais ações no sistema.

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/2b3273dc-f2e2-4a75-93ad-d8dfbc49f837)
<br> Figura 3: Diagrama UML Caso de Uso <br>
Fonte: Elaboração própria 

<br>

&emsp;&emsp; Temos dois atores: o líder de cada área da empresa e o CEO/VP RH, que terá acesso a todas as informações. É importante ressaltar que o segundo ator está como CEO/VP RH porque têm a mesma função dentro do sistema. A primeira ação feita por ambos é chamada de "Realizar Login", ação esta que possui um caso de uso incluído, uma vez que para realizar o login, o sistema deve necessariamente verificar a senha. Além disso, também há o caso de uso estendido, que ocorre somente quando alguns critérios são cumpridos, como por exemplo, quando a senha está errada e, por isso, o acesso é recusado. Com essa primeira ação concluída, o ator pode entrar na área de configuração, tela onde terá os dados pessoais e a possibilidade de logout. Com isso, temos outra situação de estender, já que o CEO/VP do RH pode visualizar todas as informações da empresa e o líder de cada visualiza a mesma junção de informações, mas com dados específicos da sua área. 


# <a name="c3"></a> 3. Diagrama de Componente

Utilizado para visualizar a estrutura e as interações dos componentes de um sistema, garante uma visão geral da arquitetura. Conta com 1) Componente: Módulos do software que desempenham funções específicas; 2) Interfaces: Definição das operações que um componente pode disponibilizar para outros; 3) Dependências: Conexões entre os componentes, indicando as interdependências.

## 3.1 Camadas

- **Camada de Interface:** Responsável pela interação direta com o usuário. É onde os elementos visuais são projetados e apresentados. Sua principal função é apresentar os dados de forma compreensível aos usuários.

- **Camada de Aplicação:** Local onde as as regras de negócios são implementadas. Processa as solicitações dos usuários vindas da camada de interface, transformando as entradas dos usuários em ações e resultados.

- **Camada de Persistência:** Armazena e recupera os dados. Responsável por interagir com o banco de dados, garantindo que as informações sejam salvas e possam ser recuperadas quando necessário.

- **Camada de Integração:** Facilita a comunicação entre os diversos componentes do software, integração de módulos, serviços externos ou APIs.

- **Camada de Infraestrutura:** Suporte básico para o funcionamento do sistema. Garante que o software seja executado de maneira segura e confiável.


## 3.2 Componentes e Funções

![image](https://github.com/Inteli-College/2024-T0004-SI09-G01/assets/99206636/3ce63cf7-b9cc-46de-8539-b3ff50b2761b)
<br> Figura 4: Diagrama de Componente <br>
Fonte: Elaboração própria

<br>

**1. Camada de Interface:**

- **Front-end:** Parte do sistema com a qual o usuário final interage diretamente. Responsável por apresentar a interface gráfica e gerenciar as interações do usuário. Neste caso o desenvolvimento será feito em frameworks Angular utilizando TypeScript.

**2. Camada de Aplicação:**

- **Backend/API:** Responsável por processar requisições do front-end, acessar dados do banco de dados e gerar respostas. A api será utilizada como intermediário de comunicação e envio de dados entre o backend e o Script. Neste caso será desenvolvido em dotnet (C#). 


**3. Camada de Persistência:**

- **Banco de dados:** Armazena os dados que serão consumidos no sistema e logs.Neste caso, será utilizado bancos de dados relacional PostgreSQL.

- **Script:** Permite manipular e analisar os dados armazenados no banco de dados. Isso pode ser feito para fins de BI (Business Intelligence) ou geração de relatórios. Neste caso será realizado em Python.

**4. Camada de Integração:**

- **Requisição HTTP:** Permite que o sistema se comunique com serviços externos através do protocolo HTTP. Utilizado para integrar com APIs.

**5. Camada de Infraestrutura:**

- **Logs do sistema:** Registram eventos e atividades do sistema, podem ser analisados para identificar problemas, entender o comportamento do sistema e garantir sua segurança.
  
- **Docker:** Utilizado para contêinerização que permite "empacotar" e distribuir aplicações de forma independente. Facilitando a implantação e o gerenciamento do sistema.


**Considerações:** Para uma simulação local, vamos utilizar o Render, que tem as seguintes configurações: <br> <br>
1 GB de HD <br>
3 a 4% de CPU <br>
10% utilizado no hd (até o momento) <br>
256MB memória <br> <br>
1 GB de HD <br>
3 a 4% de CPU <br>
10% utilizado no hd (até o momento) <br>
256MB memória <br> <br>
webservice <br>
256MB de memória <br>
0,5 de CPU <br>
SO_UBUNTU <br>
HD Dinâmico <br>


# <a name="c4"></a> 4. Referências

GUIA DEV. Arquitetura em Camadas. Guia Dev, 2023. Disponível em: https://guia.dev/pt/pillars/software-architecture/layers.html. Acesso em: 18 fev. 2024.

LUCIDCHART. Diagrama de componentes UML. [S. l.], [s. d.]. Disponível em: https://www.lucidchart.com/pages/pt/diagrama-de-componentes-uml. Acesso em: 15 fev. 2024.
