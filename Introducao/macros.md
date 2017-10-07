# Macros

<p>As macros são variáveis internas da plataforma que disponibilizam informações relacionadas à atividade em execução e informações gerais do ambiente.</p>
<p>Estas macros estão disponíveis em todos os módulos da plataforma e podem ser utilizadas em parâmetros para execução de objetos, expressões e filtros.</p>

## Datas
As macros de data são utilizadas para obter informações relacioandas à data de movimento ou data atual e, em alguns casos podem ser manipuladas pelo usuário	.
<table>
<thead>
<th>Nome</th>
<th>Descrição</th>
<th>Versão</th></thead>
<tr><td>DATA</td><td>Retorna a data do movimento (inicializada como a data atual).</td><td></td>
<tr><td>DATAATUAL</td><td>Retorna a data do servidor de banco de dados.</td><td></td>
<tr><td>AMANHA</td><td>Retorna a data do próximo dia a partir da macro DATA</td><td></td>
<tr><td>ONTEM</td><td>Retorna a data do dia anterior a partir da macro DATA</td><td></td>
<tr><td colspan="3"></td>
<tr><td>DOMINGO</td><td>Retorna 1 se a data contida na macro DATA for domingo.</td><td></td>
<tr><td>SEGUNDA</td><td>Retorna 1 se a data contida na macro DATA for segunda.</td><td></td>
<tr><td>TERCA</td><td>Retorna 1 se a data contida na macro DATA for terça.</td><td></td>
<tr><td>QUARTA</td><td>Retorna 1 se a data contida na macro DATA for quarta.</td><td></td>
<tr><td>QUINTA</td><td>Retorna 1 se a data contida na macro DATA for quinta.</td><td></td>
<tr><td>SEXTA</td><td>Retorna 1 se a data contida na macro DATA for sexta.</td><td></td>
<tr><td>SABADO</td><td>Retorna 1 se a data contida na macro DATA for sábado.</td><td></td>
<tr><td colspan="3"></td>
<tr><td>INICIODOANO</td><td>Retorna a data do primeiro dia do ano a partir da macro DATA.</td><td></td>
<tr><td>FIMDOANO</td><td>Retorna a data do último dia do ano a partir da macro DATA.</td><td></td>
<tr><td>INICIODOMES</td><td>Retorna a data do primeiro dia do mês a partir da macro DATA.</td><td></td>
<tr><td>FIMDOMES</td><td>Retorna a data do último dia do mês a partir da macro DATA.</td><td></td>
<tr><td>INICIODOBIMESTRE</td><td>Retorna a data do primeiro dia do bimestre a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>FIMDOBIMESTRE</td><td>Retorna a data do último dia do bimestre a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>INICIODOTRIMESTRE</td><td>Retorna a data de primeiro dia do trimestre a patir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>FIMDOTRIMESTRE</td><td>Retorna a data do último dia do trimestre a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>INICIODOSEMESTRE</td><td>Retorna a data do primeiro dia do semestre a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>FIMDOSEMESTRE</td><td>Retorna a data do último dia do semestre a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td colspan="3"></td>
<tr><td>INICIODOANOANTERIOR</td><td>Retorna a data do primeiro dia do ano anterior a partir da macro DATA.</td><td></td>
<tr><td>FIMDOANOANTERIOR</td><td>Retorna a data do último dia do ano anterior a partir da macro DATA.</td><td></td>
<tr><td>INICIODOMESANTERIOR</td><td>Retorna a data do primeiro dia do mês anterior a partir da macro DATA.</td><td></td>
<tr><td>FIMDOMESANTERIOR</td><td>Retorno a data do último dia do mês anterior a partir da macro DATA</td><td></td>
<tr><td>INICIODOBIMESTREANOANTERIOR</td><td>Retorno a data do primeiro dia do bimestre do ano anterior a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>FIMDOBIMESTREANOANTERIOR</td><td>Retorna a data do último dia do mesmo bimestre do ano anterior a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>INICIODOTRIMESTREANOANTERIOR</td><td>Retorna a data do primeiro dia do mesmo trimestre do ano anterior a patir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>FIMDOTRIMESTREANOANTERIOR</td><td>Retorna a data do último dia do mesmo trimestre do ano anterior a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>INICIODOSEMESTREANOANTERIOR</td><td>Retorna a data do primeiro dia do mesmo semestre do ano anterior a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td>FIMDOSEMESTREANOANTERIOR</td><td>Retorna a data do último dia do mesmo semestre do ano anterior a partir da macro DATA</td><td>![date version][versao-1-17-1]</td>
<tr><td colspan="3"></td>
<tr><td>INICIOMESDOANOANT</td><td>Retorna a data do primeiro dia do mesmo mês do ano anterior a partir da macro DATA.</td><td></td>
<tr><td>FIMMESDOANOANT</td><td>Retorna a data do último dia do mesmo mês do ano anterior a partir da macro DATA.</td><td></td>
<tr><td>INICIOMESANTDOANOANT</td><td>Retorna a data do primeiro dia do mês e ano anteriores a partir da macro DATA.</td><td></td>
<tr><td>FIMMESANTDOANOANT</td><td>Retorna a data do último dia do mês e ano anteriores a partir da macro DATA.</td><td></td>
<tr><td></td><td></td><td></td>
<tr><td>DATAMAIS</td><td>Retorna a data da macro DATA + qtde de dias de incremento informada na criação do parâmetro.</td><td></td>
<tr><td>DATAMENOS</td><td>Retorna a data da macro DATA - qtde de dias de decremento informada na criação do parâmetro.</td><td></td>
<tr><td>INICIODOANOMENOS</td><td>Retorna a data do primeiro dia do ano a partir da macro DATA - qtde de dias de decremento informada na criação do parâmetro</td><td></td>
<tr><td>FIMDOANOMENOS</td><td>Retorna a data do último dia do ano a partir da macro DATA - qtde de dias de decremento informada na criação do parâmetro</td><td></td>
<tr><td>INICIOMESMENOS</td><td>Retorna a data do primeiro dia do mês a partir da macro data - qtde de dias de decremento informada na criação do parâmetro.</td><td></td>
<tr><td>FIMMESMENOS</td><td>Retorna a data do último dia do mês a partir da macro data - qtde de dias de decremento informada na criação do parâmetro.</td><td></td>
<tr><td colspan="3"></td>
<tr><td>DATAINICIALANOANT</td><td>Retorna a data do mesmo dia do ano anterior a partir da macro DATAINICIAL.</td><td></td>
<tr><td>DATAFINALANOANT</td><td>Retorna a data do mesmo dia do ano anterior a partir da macro DATAFINAL.</td><td></td>
<tr><td>DATAINICIALMESANT</td><td>Retorna a data do mesmo dia do mês anterior a partir da macro DATAINICIAL.</td><td></td>
<tr><td>DATAFINALMESANT</td><td>Retorna a data do mesmo dia do mês anterior a partir da macro DATAFINAL.</td><td></td>
<tr><td>MESMODIADOANOANT</td><td>Retorna a data do mesmo dia do ano anterior a partir da macro DATA.</td><td></td>
<tr><td>MESMODIADOMESANT</td><td>Retorna a data do mesmo dia do mês anterior a partir da macro DATA.</td><td></td>
<tr><td>ONTEMDOANOANT</td><td>Retorna a data o mesmo dia do ano anterior a partir da macro ONTEM.</td><td></td>
<tr><td>ONTEMDOMESANT</td><td>Retorna a data do mesmo dia do mês anterior a partir da macro ONTEM.</td><td></td>
</table>

## Usuario
As macros de usuário são utilizadas para obter informações relacioandas ao usuário logado.

<table>
<thead>
<th>Nome</th>
<th>Descrição</th>
<th>Versão</th></thead>
<tr><td>USUARIO</td><td>Retorna o código do usuário SimplificAção logado.</td><td></td>
<tr><td>USUARIOEMAIL</td><td>Retorna o e-mail do usuário SimplificAção logado.</td><td></td>
<tr><td>USUARIOERP</td><td>Retorna o código da integração ERP para o usuário SimplificAção logado.</td><td></td>
<tr><td>USUARIOLOGIN</td><td>Retorna o login do usuário SimplificAção logado.</td><td></td>
<tr><td>USUARIONOME</td><td>Retorna o nome do usuário SimplificAção logado.</td><td></td>
<tr><td>USUARIOTELEFONE</td><td>Retorna o telefone do usuário SimplificAção logado.</td><td></td>
<tr><td>SUPERVISOR</td><td>Retorna o código do supervisor utilizado na liberação de envio de dados no dispositivo móvel.</td><td></td>
<tr><td>SUPERVISORNOME</td><td>Retorna o nome do supervisor utilizado na liberação de envio de dados no dispositivo móvel.</td><td></td>
</table>

## Identificadores
As macros denominadas identificadores retornam valores relacionados ao processo que o usuário executou. Com estas macros é possível identificar as seleções efetuadas pelo usuário ou as atividades executadas.

<table>
<thead>
<th>Nome</th>
<th>Descrição</th>
<th>Versão</th></thead>
<tr><td>ACAO</td><td>Retorna a ação realizada</td><td></td>
<tr><td>CHAVEACOESRETORNO</td><td>Retorna a chave de retorno da ação executada</td><td></td>
<tr><td>CHAVEAUDITORIA</td><td>Retorna a sequência (chave) de execução da auditoria em um agendamento.</td><td>![date version][versao-1-9-0]</td>
<tr><td>CHAVEFORMULARIO</td><td>Retorna a sequência (chave) de digitação do formulário utilizado em uma ação.</td><td>![date version][versao-1-6-1]</td>
<tr><td>CHAVEPDV</td><td>Retorna a sequência (chave) do pedido gerado a partir de um menu tipo Digitação de Ações e Digitação MIP.</td><td>![date version][versao-1-15-2]</td>
<tr><td>CHAVEPDVITENS</td><td>Retorna a sequência do item (chave) digitado em um menu tipo Digitação de Ações e Digitação MIP.</td><td>![date version][versao-1-15-2]</td>
<tr><td>DASHBOARD</td><td>Retorna o código do Dashboard em execução</td><td></td>
<tr><td>FORMULARIO</td><td>Retorna o código do formulário utilizado em uma ação.</td><td>![date version][versao-1-6-1]</td>
<tr><td>LOJA</td><td>Retorna o código da Loja para integração com sistema Superus.</td><td></td>
<tr><td>MATRIZ</td><td>Retorna o código da Matriz/Empresa do ERP.</td><td></td>
<tr><td>MENU</td><td>Retorna o código do menu atual.</td><td></td>
<tr><td>NIVEL1</td><td>Retorna o conteúdo do campo CODIGO do primeiro nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL2</td><td>Retorna o conteúdo do campo CODIGO do segundo nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL3</td><td>Retorna o conteúdo do campo CODIGO do terceiro nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL4</td><td>Retorna o conteúdo do campo CODIGO do quarto nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL5</td><td>Retorna o conteúdo do campo CODIGO do quinto nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL6</td><td>Retorna o conteúdo do campo CODIGO do sexto nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL7</td><td>Retorna o conteúdo do campo CODIGO do sétimo nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL8</td><td>Retorna o conteúdo do campo CODIGO do oitavo nível do menu de um sistema.</td><td></td>
<tr><td>NIVEL9</td><td>Retorna o conteúdo do campo CODIGO do nono nível do menu de um sistema.</td><td></td>
<tr><td>NOME</td><td>Retorna o conteúdo do campo NOME do menu atual.</td><td></td>
<tr><td>NOME1</td><td>Retorna o conteúdo do campo NOME do menu do primeiro nível de um sistema.</td><td></td>
<tr><td>NOME2</td><td>Retorna o conteúdo do campo NOME do menu do segundo nível de um sistema.</td><td></td>
<tr><td>NOME3</td><td>Retorna o conteúdo do campo NOME do menu do terceiro nível de um sistema.</td><td></td>
<tr><td>NOME4</td><td>Retorna o conteúdo do campo NOME do menu do quarto nível de um sistema.</td><td></td>
<tr><td>NOME5</td><td>Retorna o conteúdo do campo NOME do menu do quinto nível de um sistema.</td><td></td>
<tr><td>NOME6</td><td>Retorna o conteúdo do campo NOME do menu do sexto nível de um sistema.</td><td></td>
<tr><td>NOME7</td><td>Retorna o conteúdo do campo NOME do menu do sétimo nível de um sistema.</td><td></td>
<tr><td>NOME8</td><td>Retorna o conteúdo do campo NOME do menu do oitavo nível de um sistema.</td><td></td>
<tr><td>NOME9</td><td>Retorna o conteúdo do campo NOME do menu do nono nível de um sistema.</td><td></td>
<tr><td>RETORNO</td><td>Retorna o conteúdo do campo código do menu atual</td><td></td>
<tr><td>SISTEMA</td><td>Retorna o código do sistema em uso.</td><td></td>
<tr><td>SITE</td><td>Retorna o código do site.</td><td></td>
<tr><td>WF_CASO</td><td>Retorna o código do Caso do Processo</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_CASONOME</td><td>Retorno o nome do Caso do Processo</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_CHAVEEXECUCAO</td><td>Retorno a chave do trâmite do Processo</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_DECISAO</td><td>Retorna o código da Decisão selecionada pelo usuário</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_DECISAONOME</td><td>Retorna o nome da Decisão selecionada pelo usuário</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_PROCESSO</td><td>Retorna o código do Processo</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_PROCESSONOME</td><td>Retorna o nome do Processo</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_TAREFA</td><td>Retorna o código da Tarefa do Processo</td><td>![date version][versao-1-15-0]</td>
<tr><td>WF_TAREFANOME</td><td>Retorno o nome da Tarefa do Processo</td><td>![date version][versao-1-15-0]</td>
</table>

## Miscelania

<table>
<thead>
<th>Nome</th>
<th>Descrição</th>
<th>Versão</th></thead>
<tr><td>DATADIGITADA</td><td>Retorna a data digitada na Ação.</td><td></td>
<tr><td>DESTINATARIOEMAIL</td><td>Retorna o email para envio de mensagens</td><td></td>
<tr><td>DESTINATARIOGRUPO</td><td>Retorna o grupo de usuários para envio de mensagens</td><td></td>
<tr><td>DESTINATARIOTELEFONE</td><td>Retorna o telefone (celular) para envio de mensagens</td><td></td>
<tr><td>DESTINATARIOUSUARIO</td><td>Retorna o código de usuário para envio de mensagens</td><td></td>
<tr><td>EMPRESA</td><td>Retorna o código da empresa SimplificAção.</td><td></td>
<tr><td>HORADISPOSITIVO</td><td>Retorna a hora do dispositivo móvel.</td><td></td>
<tr><td>HORASERVIDOR</td><td>Retorna a hora do servidor (momento da última verificação da hora no servidor).</td><td></td>
<tr><td>IDMENSAGEM</td><td>Retorna a identificação da mensagem gerada pelo usuário.</td><td></td>
<tr><td>INPUTDATA</td><td>Deve ser o alias de um campo da query. O conteúdo deste campo na query alimentará a entrada Data nas ações que exigem entrada de dados do tipo Data. Também pode ser utilizado como valor default de campos tipo Data em formulários de ações.</td><td></td>
<tr><td>INPUTTEXTO</td><td>Deve ser o alias de um campo da query. O conteúdo deste campo na query alimentará a entrada Texto nas ações que exigem entrada de dados do tipo Texto. Também pode ser utilizado como valor default de campos tipo Texto, Memo e Título em formulários de ações.</td><td></td>
<tr><td>INPUTVALOR</td><td>Deve ser o alias de um campo da query. O conteúdo deste campo na query alimentará a entrada Valor nas ações que exigem entrada de dados do tipo Valor. Também pode ser utilizado como valor default de campos tipo Numérico em formulários de ações.</td><td></td>
<tr><td>MENSAGEMCURTA</td><td>Retorna o assunto do e-mail ou texto do SMS da mensagem</td><td></td>
<tr><td>MENSAGEMLONGA</td><td>Retorna o corpo do e-mail da mensagem</td><td></td>
<tr><td>SAUDACAO</td><td>Retorna Bom dia/Boa tarde/Boa noite conforme o horário da sua utilização.</td><td>![date version][versao-1-8-1]</td>
<tr><td>TEXTO</td><td>Retorna o texto digitado na ação.</td><td></td>
<tr><td>VALIDAQUANTIDADE</td><td>Validação de quantidade em menus tipo Pedido (implementação futura).</td><td></td>
<tr><td>VALIDAVALOR</td><td>Validação de valor em menus tipo Pedido (implementação futura).</td><td></td>
<tr><td>VALOR</td><td>Retorna o valor digitado na ação.</td><td></td>
<tr><td>VARIAVEL1</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL2</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL3</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL4</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL5</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL6</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL7</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL8</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL9</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
<tr><td>VARIAVEL10</td><td>Macro genérica para receber qualquer valor definido pelo usuário.</td><td>![date version][versao-1-17-0]</td>
</table>



[versao-1-6-1]: https://img.shields.io/badge/v-1.6.1-green.svg
[versao-1-8-1]: https://img.shields.io/badge/v-1.8.1-green.svg
[versao-1-9-0]: https://img.shields.io/badge/v-1.9.0-green.svg
[versao-1-15-0]: https://img.shields.io/badge/v-1.15.0-green.svg
[versao-1-15-2]: https://img.shields.io/badge/v-1.15.2-green.svg
[versao-1-17-0]: https://img.shields.io/badge/v-1.17.0-green.svg
[versao-1-17-1]: https://img.shields.io/badge/v-1.17.1-green.svg
