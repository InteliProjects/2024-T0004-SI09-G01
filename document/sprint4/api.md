# Sumário

[1. Cid](#c1)

[2. ZenKlub](#c2)

[3. Employees](#c3)

[4. Gptw](#c4)

[5. Logs](#c5)

[6. Stiba](#c6)

<br>

# <a name="c1"></a> 1. Cid

## 1.1 Obter CID por Ano

- **Método HTTP:** GET
- **Endpoint:** `/api/cid/year`
- **Descrição:** Este endpoint retorna dados relacionados ao CID por ano, incluindo o total de dias abonados e o número de atestados por ano.
- **Exemplo de Requisição:** `GET /api/cid/year`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "DiasAbonados": 123,
            "NumeroDeAtestados": 45
        },
        {
            "DiasAbonados": 98,
            "NumeroDeAtestados": 32
        },
        ...
    ]
    ```

### 1.2 Obter CID por Mês

- **Método HTTP:** GET
- **Endpoint:** `/api/cid/month`
- **Descrição:** Este endpoint retorna dados relacionados ao CID por mês, incluindo o total de dias abonados e o número de atestados por mês.
- **Exemplo de Requisição:** `GET /api/cid/month`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "MesOcorrencia": "Janeiro",
            "DiasAbonados": 45,
            "NumeroDeAtestados": 20
        },
        {
            "MesOcorrencia": "Fevereiro",
            "DiasAbonados": 32,
            "NumeroDeAtestados": 15
        },
        ...
    ]
    ```

### 1.3 Obter Frequência de CID

- **Método HTTP:** GET
- **Endpoint:** `/api/cid/cidFrequency`
- **Descrição:** Este endpoint retorna a frequência dos CIDs mais comuns, incluindo o total de dias abonados, o número de atestados e a descrição do CID.
- **Exemplo de Requisição:** `GET /api/cid/cidFrequency`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "DiasAbonados": 123,
            "NumeroDeAtestados": 45,
            "CidDescricao": "CID-10"
        },
        {
            "DiasAbonados": 98,
            "NumeroDeAtestados": 32,
            "CidDescricao": "CID-11"
        },
        ...
    ]
    ```

### 1.4 Obter Informações de CID por Unidade

- **Método HTTP:** GET
- **Endpoint:** `/api/cid/cidUnit`
- **Descrição:** Este endpoint retorna dados relacionados ao CID por unidade, incluindo o total de dias abonados e o número de atestados por unidade.
- **Exemplo de Requisição:** `GET /api/cid/cidUnit`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "Unidade": "Unidade A",
            "DiasAbonados": 45,
            "NumeroDeAtestados": 20
        },
        {
            "Unidade": "Unidade B",
            "DiasAbonados": 32,
            "NumeroDeAtestados": 15
        },
        ...
    ]
    ```

# <a name="c2"></a> 2. ZenKlub

## 2.1 Obter Sessões por Fábrica

- **Método HTTP:** GET
- **Endpoint:** `/api/zenklub/sessionsFactory`
- **Descrição:** Este endpoint retorna o total de sessões por departamento na fábrica ZenKlub.
- **Exemplo de Requisição:** `GET /api/zenklub/sessionsFactory`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "Departamento": "Departamento A",
            "TotalSessoes": 123
        },
        {
            "Departamento": "Departamento B",
            "TotalSessoes": 98
        },
        ...
    ]
    ```

### 2.2 Obter Total de Sessões

- **Método HTTP:** GET
- **Endpoint:** `/api/zenklub/sessionsTotal`
- **Descrição:** Este endpoint retorna o total de sessões em todas as áreas do ZenKlub.
- **Exemplo de Requisição:** `GET /api/zenklub/sessionsTotal`
- **Exemplo de Resposta:**
    ```json
    {
        "TotalSessoes": 1000
    }
    ```

### 2.3 Obter Sessões por Funcionário

- **Método HTTP:** GET
- **Endpoint:** `/api/zenklub/employeesSessions`
- **Descrição:** Este endpoint retorna o total de sessões por número de pessoal (funcionário) no ZenKlub.
- **Exemplo de Requisição:** `GET /api/zenklub/employeesSessions`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "NumeroPessoal": "123",
            "TotalSessoes": 45
        },
        {
            "NumeroPessoal": "456",
            "TotalSessoes": 32
        },
        ...
    ]
    ```

### 2.4 Obter Sessões por Mês

- **Método HTTP:** GET
- **Endpoint:** `/api/zenklub/byMonthSessions`
- **Descrição:** Este endpoint retorna o total de sessões agrupadas por mês no ZenKlub.
- **Exemplo de Requisição:** `GET /api/zenklub/byMonthSessions`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "Mes": "Janeiro",
            "TotalSessoes": 100
        },
        {
            "Mes": "Fevereiro",
            "TotalSessoes": 80
        },
        ...
    ]
    ```

# <a name="c3"></a> 3. Employees

## 3.1 Obter Modelos de Empregados

- **Método HTTP:** GET
- **Endpoint:** `/api/volks/employees`
- **Descrição:** Este endpoint retorna modelos de empregados da Volks, incluindo informações como texto RH e total de empregados.
- **Exemplo de Requisição:** `GET /api/volks/employees`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "TextoRH": "Departamento A",
            "TotalEmpregados": 123
        },
        {
            "TextoRH": "Departamento B",
            "TotalEmpregados": 98
        },
        ...
    ]
    ```

# <a name="c4"></a> 4. Gptw

## 4.1 Obter Pontuação de Questões por Tópico

- **Método HTTP:** GET
- **Endpoint:** `/api/gptw/topic`
- **Descrição:** Este endpoint retorna a pontuação de questões por tópico no GPTW.
- **Exemplo de Requisição:** `GET /api/gptw/topic`
- **Exemplo de Resposta:**
    ```json
    {
        "Credibilidade": 80,
        "Respeito": 85,
        "Imparcialidade": 75,
        "Orgulho": 90,
        "Camaradagem": 80,
        "Adicional": 70
    }
    ```

## 4.2 Obter Modelos de Empregados GPTW

- **Método HTTP:** GET
- **Endpoint:** `/api/gptw/models`
- **Descrição:** Este endpoint retorna modelos de empregados GPTW, incluindo informações como idade do empregado e tipo de ausência.
- **Exemplo de Requisição:** `GET /api/gptw/models`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "IdadeEmpregado": 30,
            "TipoAusencia": "Férias"
        },
        {
            "IdadeEmpregado": 35,
            "TipoAusencia": "Licença Maternidade"
        },
        ...
    ]
    ```

## 4.3 Obter Engajamento GPTW

- **Método HTTP:** GET
- **Endpoint:** `/api/gptw/engage`
- **Descrição:** Este endpoint retorna informações sobre o engajamento GPTW, incluindo percentual de engajamento, índice de confiança e auditoria cultural.
- **Exemplo de Requisição:** `GET /api/gptw/engage`
- **Exemplo de Resposta:**
    ```json
    [
        {
            "Year": 2023,
            "EngagementPercent": 85,
            "Trust": 90,
            "Culture": 80
        },
        {
            "Year": 2022,
            "EngagementPercent": 82,
            "Trust": 88,
            "Culture": 75
        },
        ...
    ]
    ```

## 4.4 Obter Métricas de Pontuação Média e Engajamento

- **Método HTTP:** GET
- **Endpoint:** `/api/gptw/metrics`
- **Descrição:** Este endpoint retorna métricas de pontuação média e engajamento no GPTW.
- **Exemplo de Requisição:** `GET /api/gptw/metrics`
- **Exemplo de Resposta:**
    ```json
    {
        "PontuacaoMedia": 85,
        "Engajamento": 80
    }
    ```

# <a name="c5"></a> 5. Log

## 5.1 Registrar Log de Solicitação

- **Método HTTP:** POST
- **Endpoint:** `/logs/request`
- **Descrição:** Este endpoint permite registrar logs de solicitações, incluindo informações como mensagem, status, horário e ID do usuário.
- **Corpo da Requisição:** Deve incluir um objeto JSON com os seguintes campos:
    - `Mensagem` (string): Mensagem associada ao log.
    - `Status` (string): Status da solicitação.
    - `Horario` (string, opcional): Horário da solicitação.
    - `IdUsuario` (int, opcional): ID do usuário associado à solicitação.
- **Exemplo de Requisição:**
    ```json
    {
        "Mensagem": "Solicitação processada com sucesso.",
        "Status": "200 OK",
        "Horario": "2024-03-29T15:30:00",
        "IdUsuario": 123
    }
    ```
- **Resposta:** Retorna um código de status 200 indicando que o log foi registrado com sucesso.

## 5.2 Registrar Log de Interação

- **Método HTTP:** POST
- **Endpoint:** `/logs/interaction`
- **Descrição:** Este endpoint permite registrar logs de interações, incluindo informações como mensagem, status, horário e ID do usuário.
- **Corpo da Requisição:** Deve incluir um objeto JSON com os seguintes campos:
    - `Mensagem` (string): Mensagem associada ao log.
    - `Status` (string): Status da interação.
    - `Horario` (string, opcional): Horário da interação.
    - `IdUsuario` (int, opcional): ID do usuário associado à interação.
- **Exemplo de Requisição:**
    ```json
    {
        "Mensagem": "Interacao registrada com sucesso.",
        "Status": "OK",
        "Horario": "2024-03-29T15:35:00",
        "IdUsuario": 456
    }
    ```
- **Resposta:** Retorna um código de status 200 indicando que o log foi registrado com sucesso.

# <a name="c6"></a> 6. Stiba

## 6.1 Obter Informações de Participação

- **Método HTTP:** `GET`
- **Endpoint:** `/api/stiba/participation`
- **Descrição:** Recupera informações sobre a participação no Stiba, incluindo a porcentagem de respostas e a pontuação média do Stiba.
- **Resposta:** Retorna as informações de participação no Stiba como um objeto JSON.

## 6.2 Obter Áreas de Pesquisa

- **Método HTTP:** `GET`
- **Endpoint:** `/api/stiba/researchArea`
- **Descrição:** Recupera informações sobre as áreas de pesquisa do Stiba, incluindo a porcentagem de respostas, origem das respostas, respostas elegíveis, respondentes e pontuação média do Stiba.
- **Resposta:** Retorna informações sobre as áreas de pesquisa do Stiba como um array JSON.

## 6.3 Filtrar por Área Específica

- **Método HTTP:** `GET`
- **Endpoint:** `/api/stiba/participationAreaFilter?area={area}`
- **Descrição:** Recupera informações sobre a participação no Stiba filtrada por uma área específica.
- **Parâmetros:** 
  - `area` (string, obrigatório): A área para filtrar as informações de participação.
- **Resposta:** Retorna informações sobre a participação no Stiba filtradas pela área especificada como um array JSON.

## 6.4 Obter Classificações de Perguntas

- **Método HTTP:** `GET`
- **Endpoint:** `/api/stiba/questionsRank?area={area}`
- **Descrição:** Recupera as classificações das perguntas do Stiba com base nas pontuações em uma área específica.
- **Parâmetros:** 
  - `area` (string, obrigatório): A área para recuperar as classificações das perguntas.
- **Resposta:** Retorna as classificações das perguntas do Stiba para a área especificada como um array JSON.



