TG1 - 5º semestre de BD
Professor da Disciplina: Giuliano Bertoti

TG
### Aluno: Sandro Toline - ra 
#### Orientador: Juliana Pasquini

## Título do TG: SISTEMA DE MONITORAMENTO DE CARGA.

1-INTRODUÇÃO
----
Devido à alta demanda de produtos, em alguns momentos por furto, roubo ou a por
acidente, as cargas de caminhões são perdidas, afim de evitar essas perdas, foi pensando em
uma solução de para que seja observado através de um monitoramento em tempo real, esse
monitoramento traria uma segurança tanto para o motorista, tanto pois para a empresa gera-se
um prejuízo.

Segunda a Policia Federal e a CNT houve um prejuízo de 1 bilhão contabilizados pelas
cargas perdidas e os caminhões que não foram recuperados após os ataques criminosos em
2014, em 2013 foram contabilizadas 17,5 mil ocorrências.

18% dos ataques criminosos ocorreram em pontos de parada e em 16% quando os
caminhões estavam parados nos acostamentos. Os dados indicam, ainda, que 63% foram com
o veículo em movimento.

No Brasil foram registrados 22 mil roubos de carga em 2018, um levantamento da
Associação Nacional do Cargas e Logística (NTC) mostra que o prejuízo da perda de cargas e
veículos chegou a cerca de 2 bilhões.

O número de ataques a transportadores foi levantado pela entidade a partir do
cruzamento de dados da Polícia Civil, da Polícia Militar e da Polícia Rodoviária Federal. O
levantamento mostra que as ocorrências vêm aumento desde de 2017, quando se chegou a
25.950.

A região Sudeste é a mais afetada, arcando com 84,79% das ocorrências, em seguida
aparece a região Nordeste com 6,43%; Sul, com 5,69%; Centro-oeste, ,34%; e por último a
região Norte, com 0,75%.

1.1- Objetivo
---
O objetivo deste trabalho é o desenvolvimento do Sistema para o monitoramento de
carga, afim de evitar possiveis roubos de carga.
- Monitoramento 24h do caminhão.
- Acompanhamento via rota.
- Gerar relatório ao final de cada viagem.

----
## 2. FUNDAMENTAÇÃO TÉCNICA

O objetivo desse capitulo é apresentar as tecnologias e processos que serão utilizados para a construção do sistema.

2.1 TECNOLOGIAS
Tecnologia usadas serão:

- Java - Back-end.

- Vue.js - Front-end.

- SaSS - desenvolvido toda a folha de estilo

- MySQL - Banco de dados.

- Spring Boot - configurações e publicações da aplicação.
---
## 3. DESENVOLVIMENTO

3.1 - Modelagem do sistema 

O modelo utilizado nesse projeto sera o padrão MVC, onde o usuário faz uma requisição, que passa pelo controller é encaminhada ao model, e após isso é devolvida ao view para o retorno ao usuário que fez a requisição inicial.

3.2 - Arquitetura de banco de dados 

O banco de dados utilizado será o MySQL, que é um SGBD, um dos mais utilizados no mercado.

3.3 - Projeto da aplicação

A ideia do sistema é fazer um monitoramento de carga, onde será armazenadas as rotas e seus tempos, afim de evitar que a carga seja furtada.
Caso a carga fique muito tempo parada, será emitido um alerta amarelo, onde será tentado contactar o motorista.
Caso não haja resposta, entrará em alerta laranja, emitindo um alerta para a empresa avisando-a de tal situação.
Caso permaneça no mesmo estado, será enviando um alerta a policia do estado/cidade.
