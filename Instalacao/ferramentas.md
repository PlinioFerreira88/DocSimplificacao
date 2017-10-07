## Instalador

A ferramenta SimplificAção Instalador permite realizar de forma simples e ágil a instalação de todos os componentes da Plataforma SimplificAção.

Conheça abaixo as etapas que guiarão o usuário no processo de instalação.

<figure>
    <img src="./_assets/img/ferramentas_instalador_boasvindas.png" alt='missing' />
    <figcaption>Tela de boas-vindas</figcaption>
</figure>

>Tipo de Instalação

Ao executar a ferramenta de instalação, o usuário poderá escolher o tipo de instalação:

<h4>Instalação do Servidor SimplificAção</h4>
É a instalação propriamente dita da Plataforma. Nesta opção será criado e configurado a estrutura do banco de dados para a Plataforma SimplificAção e a instalação do Servidor SimplificAção e demais componentes da plataforma.

Na instação do servidor, temos disponível as seguintes opções:

 `Executar SimplificAção Server como serviço` Permite efetuar a instalação e configuração do componente SimplificAção Server como um serviço do Windows. Neste modo de configuração não é necessário executar manualmente a aplicação SimplificAcaoServer.exe.

 `Executar SimplificAção Monitor ao iniciar` Inclui a aplicação SimplificAcaoMonitor.exe para ser iniciado automaticamente com o Windows.

<h4>Instalação da Estação de Trabalho</h4> 
Selecione esta opção para efetuar a instalação da Plataforma SimplificAção nos desktops dos usuários. Somente efetue este tipo de instalação após a instalação do servidor SimplificAção.

A opção `Utilizar launcher.exe a partir do servidor de arquivos`, quando marcada fará a configuração dos atalhos a partir do compartilhamento do servidor de arquivos, ou seja, para executar os aplicativos no desktop (client) este servidor de arquivos deverá estar disponível ao executar os componentes da plataforma.

<figure>
    <img src="./_assets/img/ferramentas_instalador_tipoinstalacao.png" alt='missing' />
    <figcaption>Tipo de instalação</figcaption>
</figure>

>Banco de Dados

A Plataforma SimplificAção requer a utilização do banco de dados Oracle e no processo de instalação serão oferecidas duas opções para criação/configuração da base de dados SimplificAção:

`Criar usuário e base de dados SimplificAção` Fará a criação e configuração do usuário e da base de dados. Neste modo de instalação, o usuário (owner) da plataforma será criado automaticamente pelo instalador. Será requirido a senha do usuário SYS do Oracle para efetuar a criação do usuário com todas as permissões requeridas.

`O usuário SimplificAção já foi criado. Desejo apenas criar a base de dados` Neste modo de instalação, o usuário (owner) da plataforma já deve existir com as permissões necessárias. Caso exista algum objeto pertencente a este usuário, eles serão excluídos.

!> Antes de iniciar a instalação da plataforma verifique com o seu DBA Oracle se as tablespaces requeridas pela plataforma foram criadas e se o charset do banco de dados está configurado corretamente. Clique [aqui](/Instalacao/requisitos) para acessar as configurações necessárias.

<figure>
    <img src="./_assets/img/ferramentas_instalador_bancodados.png" alt='missing' />
    <figcaption>Banco de dados</figcaption>
</figure>

>Acesso ao Banco de Dados

Serão solicitadas as informações de acesso ao banco de dados para a criação dos objetos da plataforma SimplificAção.

?> Para o caso do usuário ter optado por criar o usuário (owner) SimplificAção via instalador, neste momento será solicitado o usuário e senha do SYS do Oracle.

<figure>
    <img src="./_assets/img/ferramentas_instalador_configuracaoacesso.png" alt='missing' />
    <figcaption>Configuração de acesso ao banco de dados</figcaption>
</figure>

> Validação da Licença

Nesta etapa será feita a validação da instalação. O ID da Instalação gerado deverá ser informado para a área Administrativa da **SMP Mobilidade** para que seja feita a liberação do uso da plataforma. Após efetuado a liberação poderá ser feita a validação da licença e prosseguir com o processo de instalação.

!> Para a verificação da licença é necessário que a porta `TCP/1311` esteja liberada para o endereço `cloud.simplificacao.com`.

<figure>
    <img src="./_assets/img/ferramentas_instalador_licenca.png" alt='missing' />
    <figcaption>Validação da licença</figcaption>
</figure>

>Mídia de Instalação

O usuário deverá informar o diretório onde será instalado a Plataforma SimplificAção.

Também será solicitado o local onde foram baixados os arquivos da versão ou a seleção da instalação on-line.

!> Para efetuar a instalação on-line é necessário que a porta `TCP/21` esteja liberada para o endereço `ftp.simplificacao.com.br`.

?> Somente será habilitada a instalação da versão que estiver em uso na Cloud SimplificAção.

<figure>
    <img src="./_assets/img/ferramentas_instalador_midia.png" alt='missing' />
    <figcaption>Seleção da mídia de instalação</figcaption>
</figure>

>Informações da Instalação

Apresenta a versão que será instalada (versão disponível na Cloud SimplificAção)

<figure>
    <img src="./_assets/img/ferramentas_instalador_confirmacao.png" alt='missing' />
    <figcaption>Informações da instalação</figcaption>
</figure>

>Download

Caso o usuário tenha optado por efetuar a instalação on-line será iniciado o processo de download dos componentes da plataforma. Nesta momento será feito o acesso ao endereço `ftp.simplificacao.com.br` através da porta `TCP/21`.

<figure>
    <img src="./_assets/img/ferramentas_instalador_download.png" alt='missing' />
    <figcaption>Download da instalação</figcaption>
</figure>

>Instalação

A instalação dos componentes da plataforma será executada neste momento conforme as opções definidas nas etapas anteriores. O acesso à `cloud.simplificacao.com` pela porta `TCP/1311` será necessário neste momento para carregar o dicionário de dados e efetuar a criação da estrutura de banco de dados.

<figure>
    <img src="./_assets/img/ferramentas_instalador_instalacao.png" alt='missing' />
    <figcaption>Início da instalação</figcaption>
</figure>

>Parâmetros Iniciais

Após a instalação dos componentes, será realizada a configuração de acesso ao banco transacional. Deverá ser informado os dados de acesso ao sistema de gestão que será mais utilizado nas consultas SQL.

Também será possível efetuar a configuração dos parâmetros de inicialização da plataforma.

<figure>
    <img src="./_assets/img/ferramentas_instalador_parametros.png" alt='missing' />
    <figcaption>Parâmetros iniciais</figcaption>
</figure>

Para finalizar a instalação, deverá ser informado os dados do usuário `Supervisor`.

>Dados do Supervisor

<figure>
    <img src="./_assets/img/ferramentas_instalador_supervisor.png" alt='missing' />
    <figcaption>Dados do supervisor</figcaption>
</figure>

Após a conclusão das etapas anteriores, a Plataforma SimplificAção estará instalada.


## Atualizador

A ferramenta Atualizador permite manter sua instalação da Plataforma SimplificAção atualizada e com acesso a todos os recursos disponíveis nas versões mais recentes.

!> Antes de executar o Atualizador, garanta que seu firewall permite conexão com os seguintes endereços: `ftp.simplificacao.com.br` porta `TCP/21` e `cloud.simplificacao.com` porta `TCP/1311`.

Ao executar SimplificAcaoAtualizador.exe (disponível na pasta de instalação da plataforma) você será guiado pelo processo de atualização.

<figure>
    <img src="./_assets/img/ferramentas_atualizador_boasvindas.png" alt='missing' />
    <figcaption>Tela de boas-vindas</figcaption>
</figure>

>Tipo Atualização

Após informar o diretório de instalação da Plataforma Mobilidade, informe qual o tipo de atualização será realizado:

`Atualização on-line` Através do modo de atualização on-line é possível efetuar a atualização da plataforma para a versão em uso Cloud SimplificAção (versão estável mais recente). Caso a versão instalada localmente seja anterior a versão da Cloud SimplificAção, o Atualizador se encarregará de efetuar o download de todos os arquivos necessários, fará a atualização dos executáveis bem como a atualização dos componentes do banco de dados quando necessário.

`Informar pasta com arquivos para atualização` Através deste movo de atualização, deve-se informar a pasta onde encontram-se os arquivos da atualização da nova versão obtidos através da atualização online ou por outra forma de download.

`Atualização do banco de dados SimplificAção` Permite efetuar apenas a atualização do banco de dados, sem efetuar a atualização dos arquivos da versão.

<figure>
    <img src="./_assets/img/ferramentas_atualizador_tipoatualizacao.png" alt='missing' />
    <figcaption>Tipo de atualização</figcaption>
</figure>

>Informações da Versão

Nesta tela é informada a versão instalada localmente e a versão disponível para a atualização. Também é possível definir se os arquivos temporários da atualização deverão ser removidos ao término com sucesso da atualização.

<figure>
    <img src="./_assets/img/ferramentas_atualizador_informacao.png" alt='missing' />
    <figcaption>Informações da versão</figcaption>
</figure>

>Download

Na tela de download é possível acompanhar o progresso da transferência dos arquivos que serão utilizados na atualização. No processo de atualização através da pasta com arquivos para atualização esta etapa é ignorada.

<figure>
    <img src="./_assets/img/ferramentas_atualizador_download.png" alt='missing' />
    <figcaption>Download</figcaption>
</figure>

>Atualização

Ao clicar no botão Atualizar nesta tela, terá início o processo de atualização da plataforma. Serão realizados todos os passos para a atualização da versão. A partir deste ponto, todos os componentes da Plataforma Mobilidade não poderão ser executados até o fim do processo, caso contrário não será possível seguir com a atualização.

<figure>
    <img src="./_assets/img/ferramentas_atualizador_atualizacao.png" alt='missing' />
    <figcaption>Atualização</figcaption>
</figure>

Após a conclusão das etapas anteriores, a Plataforma SimplificAção estará atualizada.

<figure>
    <img src="./_assets/img/ferramentas_atualizador_conclusao.png" alt='missing' />
    <figcaption>Conclusão</figcaption>
</figure>

## Configurador

Antes de efetuar o primeiro acesso aos aplicativos da Plataforma SimplificAção é necessário efetuar a configuração de inicialização dos aplicativos através do SimplificAção Configurador.

Neste aplicativo você terá acesso aos parâmetros gerais e de conexão com o banco de dados. 

<figure>
    <img src="./_assets/img/ferramentas_configurador_inicio.png" alt='missing' />
    <figcaption>Tela inicial</figcaption>
</figure>

?>O aplicativo SimplificAção Configurador está disponível no diretório de instalação definido no momento da instalação dos componentes da Plataforma SimplificAção (usualmente c:\Simplificação).


A partir da tela inicial, clicando no botão de pesquisa de arquivos será possível localizar o arquivo `SIMPLIFICACAO.INI` na pasta de instalação da plataforma. 

Após selecionar o arquivo e clicar em OK na caixa de diálogo, será possível editar todas as configurações existentes, bem como criar novas configurações quando necessário.

Caso não exista o arquivo, também é possível gerar um novo arquivo a partir do botão `Criar Novo`.

As configurações de inicialização estão dispostas em duas guias:

`Banco de Dados` Com as configurações de acesso ao banco de dados SimplificAção (Oracle) e as configurações de acesso ao banco de dados transacional (execução) do cliente. Para o caso de existir mais de um banco de dados transacional, deve ser definido aqui o banco que será mais acessado pela plataforma Mobilidade.

<table>
<thead>
<td>Seção</td><td>Parâmetros</td><td>Descritivo</td>
</thead>
<tr><td rowspan="5">SimplificAção</td>
	<td>Banco de dados</td>
	<td>SGBD utilizado para a base de dados da plataforma SimplificAção. Atualmente somente Oracle é suportado.</td>
</tr>
<tr>
	<td>Database</td>
	<td>Nome do serviço conforme configuração do TNS Oracle.</td>
</tr>
<tr>
	<td>Usuário</td>
	<td>Nome do usuário de banco de dados da plataforma SimplificAção.</td>
</tr>
<tr>
	<td>Senha</td>
	<td>Senha do usuário do banco de dados da plataforma SimplificAção.</td>
</tr>
<tr>
	<td>Botão Testar Conexão</td>
	<td>Permite validar a conexão com o banco de dados conforme os parâmetros SimplificAção.</td>
</tr>
<tr><td rowspan="7">Execução</td>
	<td>Nome</td>
	<td>Descritivo do sistema transacional default a ser utilizado.</td>
</tr>
	<td>Banco de dados</td>
	<td>SGBD utilizado pelo sistema transacional default.</td>
</tr>
<tr>
	<td>Server</td>
	<td>Nome do servidor de localização do Database. Utilizado apenas para SQL Server.</td>
</tr>
<tr>
	<td>Database</td>
	<td>Nome do serviço/base de dados do sistema transacional default.</td>
</tr>
<tr>
	<td>Usuários</td>
	<td>Nome do usuário de banco de dados para conexão no sistema transacional default. O usuário informado deverá ter privilégio mínimo de leitura de tabelas, execução de Stored Procedures.</td>
</tr>
<tr>
	<td>Senha</td>
	<td>Senha do usuário do banco de dados do sistema transacional.</td>
</tr>
<tr>
	<td>Botão Testar Conexão</td>
	<td>Permite validar a conexão com o banco de dados conforme os parâmetros Execução.</td>
</tr>
</table>

?> Não existe limitação quanto a quantidade de conectores que serão utilizados na Plataforma SimplificAção, contudo a conexão com o principal banco de dados a ser acessado deve ser informado como banco Execução. As demais conexões serão definidas nas configurações de Conectores na Plataforma.

<figure>
    <img src="./_assets/img/ferramentas_configurador_bancodados.png" alt='missing' />
    <figcaption>Configuração de acesso ao banco de dados</figcaption>
</figure>


`Parâmetros Gerais` Demais configurações da plataforma.

<table>
<thead>
<td>Seção</td><td>Parâmetros</td><td>Descritivo</td>
</thead>
<tr><td rowspan="7">server</td>
	<td>SGBD</td>
	<td>Define qual o SGBD será conectado. Esta conexão refere-se ao banco SimplificAção.</td>
</tr>
<tr>
	<td>banco</td>
	<td>Determina o nome do banco de dados a ser conectado.</td>
</tr>
<tr>
	<td>usuário</td>
	<td>Nome do usuário do banco de dados.</td>
</tr>
<tr>
	<td>senha</td>
	<td>Senha do usuário (criptograda).</td>
</tr>
<tr>
	<td>port</td>
	<td>Porta TCP utilizada pelo servidor SimplificAção. Porta default `211`</td>
</tr>
<tr>
	<td>trace</td>
	<td>Indicativo se habilita a geração de trace das rotinas. `SIM`/`NAO`.</td>
</tr>
<tr>
	<td>recover</td>
	<td>Indicativo se o server tentará recuperar a conexão com o banco de dados em caso de falhas. `SIM`/`NAO`</td>
</tr>

<tr><td rowspan="6">execucao</td>
	<td>SGBD</td>
	<td>Define qual o SGBD será conectado. Os dados desta conexão refer-se ao banco Execução.</td>
</tr>
<tr>
	<td>nome</td>
	<td>Nome para identificação da conexão.</td>
</tr>
<tr>
	<td>servidor</td>
	<td>Nome ou IP do servidor do banco de dados.</td>
</tr>
<tr>
	<td>banco</td>
	<td>Nome do banco de dados a ser conectado.</td>
</tr>
<tr>
	<td>usuario</td>
	<td>Nome do usuário do banco de dados.</td>
</tr>
<tr>
	<td>senha</td>
	<td>Senha do usuário do banco de dados (criptografada).</td>
</tr>

<tr><td rowspan="2">client</td>
	<td>hostname</td>
	<td>Nome do hostname ou IP do servidor de aplicativo onde está rodando o servidor SimplificAção.</td>
</tr>
<tr>
	<td>port</td>
	<td>Porta TCP utilizada pelo servidor SimplificAção através da qual o cliente irá se conectar.</td>
</tr>

<tr><td rowspan="2">cloud</td>
	<td>hostname</td>
	<td>Nome do host da cloud SimplificAção. O hostname da cloud é `cloud.simplificacao.com`</td>
</tr>
<tr>
	<td>port</td>
	<td>Porta TCP utilizada para se conectar na cloud SimplificAção. A porta utilizada pela cloud é `1311`.</td>
</tr>

<tr><td rowspan="5">parametros</td>
	<td>aparencia</td>
	<td>Nome do skin utilizado na plataforma SimplificAção. O skin padrão é o `Windows10 Green`</td>
</tr>
<tr>
	<td>empresa</td>
	<td>Identificação do cliente. O código da empresa é gerado no momento da instalação.</td>
</tr>
<tr>
	<td>timerAuditorias</td>
	<td>Tempo em segundos que define o intervalo de processamento das Auditorias e Persistências.</td>
</tr>
<tr>
	<td>timerWorkFlow</td>
	<td>Tempo em segundos que define o intervalo de processamento das ações.</td>
</tr>
<tr>
	<td>timeMensageiro</td>
	<td>Tempo em segundos que define o intervalo de envio de mensagens/alertas.</td>
</tr>
</table>


<figure>
    <img src="./_assets/img/ferramentas_configurador_parametros.png" alt='missing' />
    <figcaption>Parâmetros gerais da plataforma</figcaption>
</figure>

!> A configuração do parâmetro parametros.empresa é mandatório para conseguir se conectar e visualizar as informações na plataforma SimplificAção. A falta deste parâmetro ou a digitação incorreta do valor não permitirá o login em nenhum dos componentes da Plataforma.

?> Na guia Parâmetros Gerais é possível incluir e excluir parâmetros através dos botões + e - localizados à esquerda da grid de parâmetros.

Após finalizar a manutenção dos parâmetros, para salvar as configurações você tem as seguintes opções:

`Salvar` Atualiza o arquivo INI de acordo com as novas configurações. A configuração anterior será gravada no arquivo com o mesmo nome mas com extensão .nnn, onde nnn indica uma numeração sequencial dos diversos arquivos salvos, iniciando em .001.

`Salvar Como` Permite gerar um novo arquivo INI com as configurações alteradas.

!> É possível criar vários arquivos de configuração, contudo a Plataforma SimplificAção utiliza o arquivo `SIMPLIFICACAO.INI` localizado na mesma pasta do executável **SimplificacaoServer.exe**.


## Monitor

![versaoinicial][versao-liberacao-monitor]

A ferramenta SimplificAção Monitor permite acompanhar o status do SimplificAção Server quando estiver rodando como um serviço do Windows.

Através do Monitor é possível, é possível:

- Instalar e desinstalar o serviço SimplificAção Server (SimplificAcaoServerSRV.exe).

- Iniciar e parar o serviço SimplificAção Server.

?> Durante o processo de instalação da Plataforma SimplificAção é possível definir a utilização do Server como serviço e a inicialização automática do Monitor ao carregar o sistema operacional.

Caso o usuário opte por utilizar o Server como serviço deverá executar o seguinte procedimento:

Executar o prompt de comandos como Administrador.

A partir do diretório de instalação da plataforma SimplificAção (padrão C:\SimplificAcao) executar o seguinte comando:

```</>
   SimplificAcaoServerSRV.exe /install
 ```
Ainda na prompt de comandos execute o comando abaixo para iniciar o serviço:

```</>
   net start SimplificAcaoServer
```

!>A utilização do servidor SimplificAção como serviço elimina a utilização do aplicativo `SimplificAcaoServer.exe`.



[versao-liberacao-monitor]: https://img.shields.io/badge/dispon%C3%ADvel%20a%20partir%20da%20vers%C3%A3o-1.5.1-red.svg
