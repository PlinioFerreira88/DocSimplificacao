> Plataforma &#10145; Comuns

Neste menu você encontra configurações comuns para Dashboards, Dispositivos Móveis, Auditorias e Processos. 

## Agendamentos

Através dos agendamentos é possível criar e definir períodos para execução das auditorias.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único do agendamento.</td></tr>
<tr><td>Nome</td><td>Nome do agendamento.</td></tr>
<tr><td>Frequência</td><td>Indica a frequência de execução do agendamento.</td></tr>
<tr><td>Dia da Semana</td><td>Indica os dias da semana que o agendamento será executado.</td></tr>
<tr><td>Intervalo</td><td>Indica o intervalo de execução do agendamento.</td></tr>
<tr><td>Qtde. Execuções</td><td>Indica a quantidade de vezes que o agendamento será realizado.</td></tr>
<tr><td>Primeira Execução</td><td>Indica a data e hora da primeira execução.</td></tr>
<tr><td>Executar na Ativação</td><td>Indica que no momento da ativação o agendamento será executado, indiferentemente da data e hora da primeira execução.</td></tr>
</table>

!> Para um agendamento ser executado é necessário que existam auditorias vinculadas e que ele seja ativado.

<figure>
    <img src="./_assets/img/comuns_agendamentos_inclusao.png" alt='missing' />
    <figcaption>Inclusão novo agendamento</figcaption>
</figure>

> Auditorias

Nesta guia será mostrada todas as auditorias vinculadas a este agendamento. Através do botão ordenação no canto direito da tela, poderá criar a ordenação desejada para a execução dos agendamentos.

<figure>
    <img src="./_assets/img/comuns_agendamentos_auditorias.png" alt='missing' />
    <figcaption>Auditorias agendamento</figcaption>
</figure>


## Ações

Ações são baseadas nas queries de manutenção de dados (Insert, Update ou Delete) ou Stored Procedures. As ações são utilizadas em menus do tipo workflow ou em qualquer tipo de menu que necessite que o usuário execute funções previamente definidas.

São exemplos de atividades implementadas através das Ações, não se limitando a estas:

`Aprovação/Reprovação de um processo`

`Impressão de etiquetas`

`Atualização de dados no ERP`

`Atividades de Auditoria`

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único da ação.</td></tr>
<tr><td>Nome</td><td>Nome da ação.</td></tr>
<tr><td>Módulo</td><td>Identifica em qual modulo do sistema será utilizado.</td></tr>
<tr><td>Descrição</td><td>Descrição detalhada da ação.</td></tr>
<tr><td>Nome Reduzido</td><td>Nome reduzido da ação a ser utilizada no sistema.</td></tr>
<tr><td>Cor Padrão</td><td>Identifica a cor do botão da ação.</td></tr>
<tr><td>Execução Online</td><td>Identifica se será executado imediatamente ou irá para uma fila de ações.</td></tr>
<tr><td>Exibir Mensagem de Conclusão de Ação</td><td>Identifica se será exibida mensagem após a execução da ação.</td></tr>
</table>

<figure>
    <img src="./_assets/img/comuns_acoes_inclusao.png" alt='missing' />
    <figcaption>Inclusão ação</figcaption>
</figure>

> Objetos

Na guia objetos será indicado quais ações serão utilizadas através de Queries ou Stored Procedure.

<figure>
    <img src="./_assets/img/comuns_acoes_objetos.png" alt='missing' />
    <figcaption>Ação objetos</figcaption>
</figure>

> Workflow

Na guia workflow podem ser definidas algumas pre-defenições para o comportamento da ação.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Tratar como pendente</td><td>Marca o item como pendente ao invés de marcar como checado nos menus tipo Workflow.</td></tr>
<tr><td>Exclui ações anteriores</td><td>Exclui as ações anteriores executadas para o mesmo item.</td></tr>
<tr><td>Marcar ações anteriores como executadas</td><td>Muda o status das ações processadas anteriormente para o item como executadas para utilização em estatísticas.</td></tr>
<tr><td>Manter em Pendentes</td><td>Se marcado e em conjunto com o parâmetro Exclui Ações Anteriores, não excluirá as ações que estiverem marcadas como pendentes.</td></tr>
<tr><td>Tempo vida Semáforo</td><td>Permite definir quanto tempo o item não será mostrado no dispositivo móvel após a tomada da ação. Utilizado para quando existe um delay entre a execução da ação e a mudança do status do registro no sistema de gestão de forma que o registro não fique sendo visualizado até que o processamento de mudança de status ocorra.</td></tr>
</table>

<figure>
    <img src="./_assets/img/comuns_acoes_workflow.png" alt='missing' />
    <figcaption>Ação workflow</figcaption>
</figure>

> Entrada de Dados

Na guia entrada de dados será possível informar algum dado adicional para a conclusão da ação.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Solicitar Formulário</td><td>Permite informar um formulário para ser utilizado como entrada de dados para a ação. Com esta opção marcada, as demais formas de entrada de dados são desativadas.</td></tr>
<tr><td>Solicitar Quantidade</td><td>Ao processar a ação exige a digitação de um campo de quantidade/valor.</td></tr>
<tr><td>Solicitar Texto</td><td> Ao processar a ação exige a digitação de um campo texto.</td></tr>
<tr><td>Solicitar Data</td><td>Ao processar a ação exige a digitação de um campo data.</td></tr>
</table>

<figure>
    <img src="./_assets/img/comuns_acoes_entradadados.png" alt='missing' />
    <figcaption>Ação entrada dados</figcaption>
</figure>


> Alertas

Na guia alertas é possível realizar o envio de mensagens a partir dos Provedores de Mensagem cadastrados


> Atividades

Na guia atividades 

## Expressões

## Formulários

Os Formulários são um poderoso componente para utilização em sistemas para dispositivos móveis para entrada de dados seja num nível de menu ou numa ação. Através dos formulários é possível criar:

`Telas para apontamentos de dados.`

`Definir entrada de valores variáveis para sistemas`

`Criar ações com entradas de dados mais aprimoradas`

`Realizar coleta de dados offline*`

!> Offline

<figure>
    <img src="./_assets/img/comuns_formularios_diagrama.png" alt='missing' />
    <figcaption>Fluxo cadastro formulárioss</figcaption>
</figure>



## Mensagens

## Objetos

