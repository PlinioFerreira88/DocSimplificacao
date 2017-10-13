> Plataforma &#10145; Configurações


## Conectores

A plataforma Mobilidade permite a conexão com diversos sistemas de gerenciamento de banco de dados ou com diversas instâncias do mesmo banco de dados.
Se um cliente possuir seu sistema de gestão baseado em um banco de dados Oracle&reg; e um sistema especialista baseado em SQL Server&reg;, é possível criar conexões para os dois bancos e utilizar as duas fontes de dados.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único do conector gerado automaticamente.</td></tr>
<tr><td>Nome</td><td>Descrição do conector.</td></tr>
<tr><td>Tipo Conexão</td><td>Identificação de qual banco será acessado.</td></tr>
<tr><td>Servidor</td><td>IP ou hostname do servidor do banco de dados.</td></tr>
<tr><td>Database</td><td>Identificação do Database ou Serviço.</td></tr>
<tr><td>Usuário</td><td>Usuário para conexão com o banco de dados.</td></tr>
<tr><td>Senha</td><td>Senha para conexão com o banco de dados.</td></tr>
<tr><td>Botão `Testar Conexão`</td><td>Validar se os dados informados são satisfatórios para conexão com o banco dados.</td></tr>
</table>

<figure>
    <img src="./_assets/img/configuracoes_conectores_inclusao.png" alt='missing' />
    <figcaption>Inclusão novo conector</figcaption>
</figure>


## Provedores

Permite cadastrar os provedores do serviço de Mensageria. Neste cadastro serão informados as configurações de contas de e-mail ou serviços de SMS para envio das mensagens geradas nas rotinas de Alerta e Ações em Dispositivos Móveis e [Auditorias](/Plataforma/Desenvolvimento/Auditorias/index.md).

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único do provedor gerado automaticamente.</td></tr>
<tr><td>Nome</td><td>Descrição do provedor.</td></tr>
<tr><td>Tipo Mensagem</td><td>Identifica SMS, E-mail ou Notificação Plataforma.</td></tr>
<tr><td>Padrão</td><td>Se marcado provedor será padrão para o tipo selecionado</td></tr>
<tr><td>Botão Testar Provedor</td><td>Validar se os dados informados são satisfátorios para conexão com o provedor</td></tr>
</table>

<figure>
    <img src="./_assets/img/configuracoes_provedores_inclusao.png" alt='missing' />
    <figcaption>Inclusão novo provedor</figcaption>
</figure>

>Parâmetros

Na guia parâmetros permite incluir todos os parâmetros do provedor. Cada tipo de provedor exige tipos diferentes de parâmetros.

Provedores de e-mail necessitam dos parâmetros básicos para configuração de envio de mensagens (e-mail, senha, servidor SMTP, porta, tipo de criptografia, etc). 

Para envio de SMS a configuração requer mais parâmetros. Clique aqui para verificar como configurar o envio de SMS a partir do serviço MobiPronto.

!> Provedores do tipo Notificação Plataforma não possuem parâmetros. Este tipo de provedor gera uma notificação enviada ao aplicativo SimplificAção Smart tanto dno ambiente Windows como iOS e Android. Para que o aplicativo receba as mensagens geradas pelo provedor é necessário que ele esteja carregado.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Sequência</td><td>Identificador da ordem dos parâmetros cadastrados.</td></tr>
<tr><td>Nome</td><td>Descrição do parâmetro.</td></tr>
<tr><td>Operação</td><td>Identifica operação de envio</td></tr>
<tr><td>Parâmetro</td><td>Identifica o parâmetro cadastrado</td></tr>
<tr><td>Valor</td><td>Identifica valores do tipo selecionado acima</td></tr>
</table>

<figure>
    <img src="./_assets/img/configuracoes_provedores_parametros.png" alt='missing' />
    <figcaption>Inclusão parâmetros</figcaption>
</figure>

## Tipo Provedores

Permite cadastrar os tipos utilizados de provedores como e-mail, SMS ou Notificação Plataforma.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único do tipo de provedor gerado automaticamente.</td></tr>
<tr><td>Nome</td><td>Descrição do tipo do provedor.</td></tr>
<tr><td>Tipo</td><td>Identifica o tipo do provedor</td></tr>
</table>

<figure>
    <img src="./_assets/img/configuracoes_tipoprovedores_inclusao.png" alt='missing' />
    <figcaption>Inclusão tipo de provedor</figcaption>
</figure>


## Dispositivos Móveis

Ao instalar o app `SimplificAção Smart` no dispositivo móvel ou no desktop (emulador), antes de efetuar o primeiro acesso será necessário cadastrar as configurações do aplicativo. Somente após efetuar as configurações de acesso será possível iniciar o uso do app.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Código de identificação da instalação.</td></tr>
<tr><td>Nome</td><td>Nome do cliente.</td></tr>
<tr><td>E-mail</td><td>Identifica o e-mail para instalação.</td></tr>
<tr><td>Senha de Instalação</td><td>Identifica a senha para instalação.</td></tr>
</table>

<figure>
    <img src="./_assets/img/configuracoes_dispositivosmoveis_inclusao.png" alt='missing' />
    <figcaption>Inclusão dispositivos móveis</figcaption>
</figure>

>Servidor

Na guia servidor permite informar os parâmetros necessários para o acesso do `SimplificAção Smart`.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Matriz</td><td>Informe a matriz (empresa) que será inicializada como padrão.</td></tr>
<tr><td>Site</td><td>Informe o site (loja/filial) que será inicializado como padrão.</td></tr>
<tr><td>Hostname</td><td>Deve ser informado o endereço IP da máquina onde está instanciado o `SimplificAção Server` (aplicativo ou serviço). Também pode ser informado o nome da máquina ou alias resolvido pelo servidor DNS.</td></tr>
<tr><td>Hostname Alternativo</td><td>Informe o endereço de IP secundário da máquina onde está instanciado o `SimplificAção Server`. Se os dispositivos móveis forem utilizados fora do ambiente da rede interna, pode ser informado como hostname Alternativo o endereço ou IP público ou ainda o IP fornecido por uma VPN que permitirão o acesso externo.</td></tr>
<tr><td>Porta TCP</td><td>Informe a porta TCP que está em uso pelo `SimplificAção Server`.</td></tr>
<tr><td>Timeout</td><td>Informe o tempo máximo (em segundos) que a aplicação aguardará por uma conexão com o `SimplificAção Server`. Ao tentar efetuar logon no `SimplificAção Smart`, será efetuada uma tentativa de conexão com o `SimplificAção Server` através do Hostname e Porta informadadas nesta configuração. Se após o tempo estabelecido no timeout não for realizada a conexão, será feita uma nova tentativa de conexão utilizando o Hostname Alternativo. Se após o tempo estabelecido no timeout não for estabelecida a conexão será gerada uma mensagem de indisponibilidade de conexão.</td></tr>
<tr><td>Tipo Interface</td><td>	Informe o tipo de interface do dispositivo (`Tablet` ou `Smartphone`). Este parâmetro define quais os sistemas estarão disponíveis para o dispositivo de acordo com as configurações aplicadas no cadastro de Sistemas para `Dispositivos Móveis`.</td></tr>
</table>

!>O endereço IP e a porta TCP em uso pelo servidor podem ser obtidos na própria interface do SimplificAção Server. Caso o SimplificAção Server esteja configurado para executar como serviço, estas informações poderão ser obtidas através do SimplificAção Monitor.

<figure>
    <img src="./_assets/img/configuracoes_dispositivosmoveis_servidor.png" alt='missing' />
    <figcaption>Dispositivos móveis servidor</figcaption>
</figure>

>Configurações Locais

Na guia configurações locais permite informar os parâmetros de definições locais para o `SimplificAção Smart`.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Logon sem Servidor</td><td>Ativa a opção de logar na plataforma caso o servidor não esteja disponível.</td></tr>
<tr><td>Som de Seleção</td><td>Com esta opção marcada, a cada seleção de itens será utilizado um som de clique.</td></tr>
<tr><td>Qtde Ações Offline</td><td>Define a quantidade de registros que serão acumulados em sistemas com menu do tipo WorkFlow antes do envio das ações para o servidor. Caso o valor seja 0 (zero) a cada ação realizada será será feito o seu envio ao servidor imediatamente.</td></tr>
<tr><td>Tempo Notificação</td><td>Define em segundos qual o intervalo de tempo será mostrado as notificações.</td></tr>
<tr><td>Tipo Teclado</td><td>Define se será utilizado o teclado nativo, físico ou virtual.</td></tr>
<tr><td>Tipo Leitor Código Barras</td><td>Define qual forma de leitura de código de barras será utilizada.</td></tr>
</table>

!>O endereço IP e a porta TCP em uso pelo servidor podem ser obtidos na própria interface do SimplificAção Server. Caso o SimplificAção Server esteja configurado para executar como serviço, estas informações poderão ser obtidas através do SimplificAção Monitor.

<figure>
    <img src="./_assets/img/configuracoes_dispositivosmoveis_servidor.png" alt='missing' />
    <figcaption>Dispositivos móveis servidor</figcaption>
</figure>