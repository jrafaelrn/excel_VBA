## Controle Operacional de Ações no Excel ##
(integrado com Tryd&reg;)


------------



📜	**Requisitos** 📜
-  Instalar o Tryd e registrar a DLL 
- Ter uma versão do Microsoft Excel&reg; e habilita-lá para executar macros.
- Ter uma conexão com a internet para receber as cotações em tempo real do Tryd para o Excel

> Os valores apresentados no arquivo são meramente ilustrativos
------------


> [ ⬇ CLIQUE AQUI PARA BAIXAR ⬇ ](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/Tryd_Robot_v1-0.xlsm "**⬇ CLIQUE AQUI PARA BAIXAR ⬇**")


🤔 **Como funciona?** 🤔

*A planilha está direcionada inicialmente para **operar comprado**, as próximas atualizações poderão contar com uma flexibilização desse modelo.*

Ao abrir a planilha, ela será direcionada para a tela abaixo.
Aqui, a jornada foi pensada no seguinte fluxo (cada item será detalhado posteriormente):
1. Antes de mais nada, é feita a ANÁLISE DE RISCO da operação;
1. Após isso, podem ser cadastrados ALERTAS para que a planilha "fale" quando o valor da cotação atingir o gatilho configurado;
1. Quando um gatilho é acionado e de fato você realiza a operação, então ela pode ser cadastrada em ORDENS.


Na barra **superior** existem 2 opções:
- **Visão Mercado:** é possível acompanhar a situação geral do mercado e da sua carteira em uma mesma tela;
- **Desempenho:** Resumo das suas operações com resultados finais processados, para analisar o desempenho de cada operação.


Na barra **lateral** existem as seguintes configurações:
- **Contas:** é possível cadastrar as corretoras e as contas com as quais opera
- **Book:** onde é cadastrado os papéis que vocês gostaria de acompanhar
- **Cotas:** opção disponível para quem opera em fundos de investimento privado e precisa gerir as cotas
- **Mais configurações:** ajustes e tabelas de suporte para o funcionamento da planilha
- Ainda é possível encontrar os botões de zoom e o *Sobre.*



![Página Inicial](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Tela%20Inicial.PNG?raw=true "Página Inicial")

------------


![Análise de Risco](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Analise%20de%20Risco_icon.PNG?raw=true "Análise de Risco")

Abaixo se encontram os campos que podem ser ajustados conforme a estratégia de cada investidor, alguns estão comentados dentro da própria planilha .

Após definido os valores de entrada e saída da operação e analisado se a relação **RISCO/RETORNO** está dentro de sua estratégia, você pode:
	⏰ **ADICIONAR UM ALERTA** e quando o papel atingir o **VALOR DISPARO**, uma mensagem de voz será gerada pela planilha.
	*(Uma tela de "envio para automatizador" irá aparecer, para que seja possível enviar a ordem para o Tryd lançar no sistema da Bolsa, mas essa função ainda não está funcional, aguardem as próximas versões)*

![Análise de Risco Detalhada](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Analise%20de%20Risco.PNG?raw=true "Análise de Risco Detalhada")

------------

![Alertas](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Alertas_icon.PNG?raw=true "Alertas")

A imagem abaixo mostra a tabela de **alertas**.
Aqui é feito o lançamento quando se clica no botão "ADICIONAR ALERTA" demonstrado anteriormente, mas também é possível incluir manualmente.

No grupo **EXECUÇÕES** as datas/horas são preenchidas automaticamente quando os gatilhos são atingidos. 



![Alertas detalhados](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Alertas.PNG?raw=true "Alertas detalhados")
> A planilha faz a verificação dos valores para gerar os alertas a cada 30 segundos.

------------

![Ordens](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Ordens_icon.PNG?raw=true "Ordens")

Abaixo a tabela de ordens.

No barra superior, no lado direito é possível encontrar o botão para incluir um nova operação/ordem. Essa opção também pode ser evocada através de outras partes da planilha, mas é possível fazer os lançamentos manuais.

> É a partir dessa tabela que o **Desempenho** é calculado na planilha.

![Ordens](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Ordens.PNG?raw=true "Ordens")


Janela para lançamento de operações/ordens.

![Incluir Operação](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Incluir%20Ordem.PNG?raw=true "Incluir Operação")

Ao se escolher a opção de **Venda**, é possível (e recomendado) lançar a Referência de Compra daquela operação, (se você não souber, pode clicar na lupa).
Com isso, o saldo será calculado, evitando erros. 

Quando o
> saldo atual - quantidade vendida no lançamento = 0 

será lançado uma indicação "#" no lançamento inicial de compra dentro da tabela de **Ordens**, identificando assim que aquela operação foi finalizada e não deverá constar mais no **Acompanhamento da Carteira** na tela **Visão Mercado.**

![Ordem de Venda](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Incluir%20Ordem_Venda.PNG?raw=true "Ordem de Venda")

------------

![Visão Mercado](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Visao%20Geral_icon.PNG?raw=true "Visão Mercado")

Na tela abaixo é possível acompanhar o mercado de forma geral.
Cada "grupo" de ações pode ser configurado conforme necessidade.

> Na parte superior existe alguns indicadores do mercado e os alertas.
No meio existem os papéis agrupados por setor.
Por fim, é possível acompanhar a carteira em tempo real, com alguns indicadores.



![Visão Mercado](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Visao%20Geral.PNG?raw=true "Visão Mercado")


------------

![Desempenho](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Desempenho_icon.PNG?raw=true "Desempenho")

Nessa tela você consegue obter os resultados finais de suas operações e avaliar o desempenho de sua estratégia.
Você pode fazer o acompanhamento individual de cada conta, trocando-as na barra superior.

*As fórmulas estão desbloqueadas para alteração conforme necessidade.*


![Desempenho](https://github.com/jrafaelrn/excel_VBA/blob/master/TRYD/HOW_TO/Desempenho.PNG?raw=true "Desempenho")
