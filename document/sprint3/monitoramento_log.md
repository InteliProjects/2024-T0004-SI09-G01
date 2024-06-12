# Sumário

[1. Monitoramento - Sonarqube](#c1)

[2. Logging](#c2)

<br>

# <a name="c1"></a> 1. Monitoramento - Sonarqube

&emsp;&emsp; O SonarQube é uma plataforma de código aberto usada para análise estática de código, visando melhorar a qualidade do código-fonte. Ele funciona realizando uma análise detalhada do código, identificando problemas como erros de sintaxe, violações de estilo de codificação, vulnerabilidades de segurança e padrões de codificação inadequados. A ferramenta suporta diversas linguagens de programação, mas para esse projeto vamos utilizar o C#. Após a análise, o SonarQube gera relatórios detalhados que destacam os problemas encontrados, classificando-os por gravidade e oferecendo sugestões para correção.

# <a name="c2"></a> 2. Logging

&emsp;&emsp; Para a persistência dos logs do sistema, vamos criar uma tabela denominada Logs. Esta tabela terá campos para armazenar informações essenciais sobre cada registro de log. Como por exemplo, a tabela abaixo: 

```
CREATE TABLE Logs (
    LogID INT PRIMARY KEY AUTO_INCREMENT,
    status_code VARCHAR(20),
    horario DATETIME,
    Message TEXT,
    id_user VARCHAR(100),
);
```

&emsp;&emsp; Assim resultando em uma tabela capaz de armazenar diversas informações sobre o status do sistema. Como por exemplo horario, para ter rastreabilidade de quando o erro ocorreu, message, para controlar o que ocorreu no sistema, LogID para identificação dos eventos e id_user para identificar quem realizou a ação.

Abaixo é possível visualizar a tabela criada pelo grupo para controle dos logs:

![Tabela de Logs](../../assets/tabelalogs.png)


 
