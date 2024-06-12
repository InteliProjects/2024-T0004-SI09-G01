# 1. Regra de Negócios

## 1.1. Gerenciar acesso dos colaboradores

- **Nome:** Controle de Acesso
- **Identificador:** RN000001
- **Descrição:** Para garantir a segurança e a confidencialidade dos dados, é necessário gerenciar o acesso dos colaboradores à plataforma. Apenas usuários autorizados terão permissão para visualizar e interagir com as informações do dashboard.
- **Evento:** Acesso à plataforma.
- **Exemplo:** Ao tentar acessar o sistema, o colaborador deve fornecer credenciais válidas (E-mail e senha). O sistema verificará as permissões associadas à conta do usuário. Se o usuário não possuir as permissões necessárias, ele será redirecionado para uma página de acesso negado.
- **Pseudo-Código:**

    ```JAVASCRIPT
    if usuario.autenticado:
        if usuario.tem_permissao("Visualizar Dashboard"):
            permitir_acesso()
        else:
            redirecionar_acesso_negado()
    else:
        redirecionar_login()
    ```

- **Documentação:** Registrar as permissões de acesso e restrições em um documento de configurações para desenvolvimento.
- **Responsável:** Equipe de desenvolvimento.


## 1.2 Selecionar período de tempo

- **Nome:** Filtro por Período
- **Identificador:** RN000002
- **Descrição:** Para fornecer uma visão mais específica dos dados, os usuários devem poder selecionar um período de tempo ao visualizar o dashboard. Permitindo uma análise de tendências e padrões ao longo dos anos.
- **Evento:** Aplicação do filtro de período.
- **Exemplo:** Durante a visualização do dashboard, o usuário deve ter a opção de escolher um período de tempo específico, como "2019". Os dados exibidos no dashboard serão automaticamente ajustados conforme o período selecionado.
- **Pseudo-Código:** 

    ```JAVASCRIPT
    periodo_selecionado = usuario.escolher_periodo()
    dados_exibidos = consultar_dados_periodo(periodo_selecionado)
    exibir_dados_dashboard(dados_exibidos)
    ```
- **Documentação:** Incluir instruções sobre como utilizar o filtro de período na documentação de UX e Programação.
- **Responsável:** Equipe de desenvolvimento.
