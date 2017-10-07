## Banco de dados Oracle

!> A instalação do banco de dados Oracle e a sua configuração devem ser realizadas por um profissional qualificado.

### Criação das tablespaces

As seguintes tablespaces devem ser disponibilizadas para instalação a instalcão da Plataforma SimplificAção:

<table>
<thead>
<td>Tablespace</td><td>Tamanho Inicial (Mb)</td><td>Incremento (Mb)</td>
<tr><td>SIMPLIFICACAO_D</td><td>100</td><td>50</td></tr>
<tr><td>SIMPLIFICACAO_I</td><td>100</td><td>50</td></tr>
</thead></table>

<p>Script para criação das tablespaces:<p>

```script
sqlplus system/senha
create tablespace SIMPLIFICACAO_D datafile '<DIRETORIO_ORADATA>\simplificacao_d01.dbf' size 100m autoextend on next 50m maxsize 2g extent management local autoallocate segment space management auto;
create tablespace SIMPLIFICACAO_I datafile '<DIRETORIO_ORADATA>\simplificacao_i01.dbf' size 100m autoextend on next 50m maxsize 2g extent management local autoallocate segment space management auto;
```

Para a utilização da versão Express Edition (XE) do SGBD Oracle, utilizar charset **AL16UTF16**.

```script
A verificação do charset em uso pode ser feita através do seguinte comando com a ferramenta SQLPlus:
  select name,value$ from sys.props$ where name='NLS_NCHAR_CHARACTERSET';
```

?> Para garantir que o charset correto seja utilizado pelo schema a ser criado, utilize a orientação de um DBA.


A partir da criação das tablespaces, a ferramenta de instalação se encarrega de criar todos os objetos do banco de dados.

### Criação do usuário

A criação do usuário **SIMPLIFICACAO** (nome sugerido) no banco de dados Oracle, pode ser realizada com o auxílio de um profissional especializado (DBA) ou durante o processo de instalação da plataforma.

Caso a criação do usuário for realizada por um DBA, as seguintes permissões devem ser concedidas:	

```grants
- RESOURCE
- CREATE VIEW
- SELECT ANY DICTIONARY
- SELECT ON SYS.V_$DATABASE
```

Se optar por criar o usuário durante o processo de instalação, será solicitado a senha do usuário SYS para a criação do usuário SIMPLIFICACAO. Certifique-se que você possua a senha do usuário SYS, caso contrário não será possível efetuar a criação do usuário pelo instalador.

## Dispositivos Android

<p>Antes de adquirir um dispositivo móvel Android para utilização do app SimplificAção, você deve saber que duas características de hardware são necessárias para garantir a compatibilidade com o aplicativo.<p>
![processador][processador-ARMv7] ![acelerador][acelerador-NEON]

Verifique estas características com o seu fornecedor do hardware antes da aquisição. Caso você já possua o dispositivo é possível verificar estas caraterísticas através do aplicativo SysCheck que pode ser adquirido através da Play Store.
Após o download o aplicativo, ao executá-lo será carregada a tela com as configurações do seu dispositivo. Verifique os itens destacados na figura abaixo:

<figure>
    <img src="./_assets/img/requisitos_android.png" alt='missing' />
    <figcaption>Tela do Applicativo SysCheck </figcaption>
</figure>


[processador-ARMv7]: https://img.shields.io/badge/processador-ARMv7-red.svg
[acelerador-NEON]: https://img.shields.io/badge/acelerador&nbsp;gr&aacute;fico-NEON-red.svg
