> Plataforma &#10145; Permissões

Neste menu você encontra as funções disponíveis para manipulação de usuários, grupos e seus direitos de acesso.

## Grupos

O primeiro passo para utilização da Plataforma SimplificAção é a criação dos grupos de usuários.

Nos grupos é possível definir as permissões de acesso dos usuários além de outras permissões específicas o *app* SimplificAção Smart e da própria Plataforma.

As liberações de acesso aos `Sistemas para Dispositivos Móveis`, `Dashboards` e `Processos` também são feitas através do Grupos.

Os grupos deverão ser incluídos de acordo com a política de acesso de cada cliente, sendo obrigatório haver, no mínimo, um grupo de usuários.

> Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único do grupo gerado automaticamente.</td></tr>
<tr><td>Nome</td><td>Descrição do grupo.</td></tr>
</table>

> Guia Usuários

Nesta guia estão disponíveis todos os usuários já cadastrados. Para adicionar um usuário existente no grupo basta selecionar o usuário através da seleção [:white_medium_small_square:] na grid de usuários. 

!> Todos os usuários existentes são mostrados na tela, mas somente os usuários marcados fazem parte do grupo.


<figure>
    <img src="./_assets/img/permissoes_grupos_inclusao.png" alt='missing' />
    <figcaption>Inclusão novo grupo</figcaption>
</figure>


> Guia Perfil do Grupo

Nesta guia é possível definir o acesso às telas e níveis de permissão de manutenção dos cadastros, além de permissões específicas para a Plataforma e Dispositivos Móveis.

!> Para que o usuário consiga efetuar logon na Plataforma SimplificAção ou no *app* Smart, indiferentemente das permissões de acesso definidas, as seguintes permissões são necessárias:

`Permissões de Logon \ Logon em Dispositivos Móveis` Para liberar o logon no *app* Smart.

`Permissões de Logon \ Logon na Plataforma SimplificAção` Para habilitar o logon na Plataforma SimplificAção.

?> Para conceder permissão de Supervisor ao grupo, basta marcar a opção `Permissão Supervisor (Acesso Irrestrito)`.

!> A permissão de Supervisor habilita acesso irrestrito às funções administrativas da Plataforma, contudo para que o grupo tenha acesso aos Sistemas de Dispositivos Móveis, Dashboards e Processos é necessário conceder as permissões de acesso a cada um dos itens.

<figure>
    <img src="./_assets/img/permissoes_grupos_perfil.png" alt='missing' />
    <figcaption>Perfil do grupo</figcaption>
</figure>

> Permissões

Nesta guia são definidas as permissões de acesso aos Sistemas de Dispositivos Móveis, Dashboards e Processos criados na Plataforma SimplificAcão.

`Sistemas` Para liberar acesso aos Sistemas para Dispositivos Móveis basta selecionar quais os itens serão liberados para o grupo de usuários.

`Dashboards` Para liberar acesso à visualização dos Dashboards basta selecionar quais os itens serão liberados para o grupo de usuários.

Além do acesso é possível definir as seguintes permissões para cada dashboard:

- **Proprietário**: Indica que os usuáiros do grupo poderão editar informações das colunas (descrição, máscara, posição).
- **Imprimir**: Indica que os usuários do grupo poderão efetuar a impressão dos elementos do dashboard quando disponível.
- **Exportar**: Indica que os usuários do grupo poderão exportar os elementos do dashboard para o Excel quando disponível.

`Processos`: Para liberar acesso aos usuários do grupo iniciar novos casos dos processos liberados.

<figure>
    <img src="./_assets/img/permissoes_grupos_permissoes.png" alt='missing' />
    <figcaption>Permissões para Sistemas, Dashboards e Processos</figcaption>
</figure>


## Usuários

Cadastro destinado ao cadastramento dos usuários da Plataforma SimplificAção e do *app* Smart.

Recomenda-se a criação de usuários nomeados e evitar, sempre que possível, a utilização de usuários genéricos ou que não identifique a pessoa relacionada ao usuário.

>Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único do usuário gerado automaticamente.</td></tr>
<tr><td>Nome</td><td>Nome completo do usuário.</td></tr>
<tr><td>Nome Logon</td><td>Nome utilizado para logon do usuário.</td></tr>
<tr><td>Superior Imediato</td><td>Indica o superior imediato do usuário.</td></tr>
<tr><td>E-mail</td><td>Endereço de e-mail do usuário. Caso o e-mail informado esteja vinculado à uma conta do [Gravatar](https://br.gravatar.com/) ao clicar no botão `Gravatar` o avatar do usuário será carregado automaticamente.</td></tr>
<tr><td>Celular</td><td>Telefone celular do usuário. Recomenda-se informar o código DDD com dois dígitos.</td></tr>
<tr><td>Botão Definir Senha</td><td>Define a senha do usuário.</td></tr>
<tr><td>Imagem</td><td>Permite carregar uma imagem/foto para o usuário.</td></tr>
</table>

<figure>
    <img src="./_assets/img/permissoes_usuarios_inclusao.png" alt='missing' />
    <figcaption>Inclusão novo usuário</figcaption>
</figure>

>Grupos do usuário

Assim como no cadastro de grupos é possível vincular os usuários ao grupo, no cadastro de usuários é possível vincular os grupos ao usuário.

Os grupos selecionados nesta tela são atribuídos ao usuário.

?> As permissões do usuário são cumulativas, ou seja, se o usuário faz parte de vários grupos com permissões distintas, todas as permissões dos grupos são herdadas para o usuário.

<figure>
    <img src="./_assets/img/permissoes_usuarios_grupos.png" alt='missing' />
    <figcaption>Grupos do usuário</figcaption>
</figure>

> Integrações

Na guia integrações é possível definir valores para os tipos de integração existentes.

Por padrão, a Plataforma SimplificAção já possui algumas integrações pré-definidas:

`ERP`: Permite vincular o código do usuário no sistema de gestão do cliente.

`Mobile`: Permite definir um logon alternativo para o usuário utilizar no *app* Smart.

Os códigos de integração informados para os usuários ficam disponíveis nas [Ações](\Comuns\acoes.md) e outras interfaces da Plataforma. É comum que o código do usuário SimplificAção seja diferente da identificação do usuário nos sistemas de gestão. É possível informar a identificação do usuário no sistema de gestão na integração ERP e sempre que for necessário acessar esta informação poderemos utilizar as [Macros](\Introducao\macros.md) ou fazer referência à integração através dos parâmetros existentes na Plataforma. 

?>Além das integrações disponibilizadas por padrão na Plataforma, é possível criar novas integrações de acordo com a necessidade de cada cliente.

<figure>
    <img src="./_assets/img/permissoes_usuarios_integracoes.png" alt='missing' />
    <figcaption>Integrações do usuário</figcaption>
</figure>

>Permissões

Na guia permissões, o administrador pode conceder acesso aos dashboards e processos exclusivamente ao usuário.

!> As liberações concedidas nos grupos e as liberações concedidas diretamente ao usuário são cumulativas.

<figure>
    <img src="./_assets/img/permissoes_usuarios_permissoes.png" alt='missing' />
    <figcaption>Permissões do usuário</figcaption>
</figure>

>Token

O token é utilizado para automatizar o processo de logon do usuário através de chamadas via linha de comando. Este recurso está disponível para ser utilizado em conjunto com os seguintes aplicativos:

`Simplificacao.exe` Permite efetuar o logon automático na Plataforma SimplificAção.

`SimplificacaoDashboard.exe` Permite efetuar o logon automático no visualizador de Dashbaords.

Para gerar o token do usuário é necessário a digitação da senha do usuário e clicar no botão `Gerar Token`. Será gerado uma string (token) que identificará o usuário. Com o token é possível efetuar a chamada dos aplicativos mencionados acima através da linha de comando conforme o exemplo a seguir:

```</>
C:\Simplificacao\Simplificacao.exe token:MTEzMjp1c3VhcmlvMDY6MDI0MDFGMjI2NA==
```
O conteúdo informado após `token:` é o token gerado pelo sistema para o usuário.

<figure>
    <img src="./_assets/img/permissoes_usuarios_token.png" alt='missing' />
    <figcaption>Token do usuário</figcaption>
</figure>


## Integrações

Através do cadastro de integrações de usuários é possível definir o relacionamento do usuário da plataforma SimplificAção com os cadastros dos sistemas de gestão (usuários, colaboradores, representantes, clientes, fornecedores, etc).

Os itens de integração desta tela são disponibilizados no cadastro de usuários onde é feito o relacionamento do usuário com o item de integração, e os valores destes itens ficam disponíveis através dos parâmetros das queries do tipo Integração.

>Campos disponíveis

<table>
<thead>
<td>Campo</td>
<td>Descrição</td>
</thead>
<tr><td>Código</td><td>Identificador único da integração.</td></tr>
<tr><td>Nome</td><td>Nome da integração.</td></tr>
<tr><td>Não permitir valores repeditos</td><td>Caso este parâmetro esteja marcado não será permitido definir o mesmo valor de integração para mais de um usuário.</td></tr>
</table>


<figure>
    <img src="./_assets/img/permissoes_integracoes_inclusao.png" alt='missing' />
    <figcaption>Cadastro de Integrações</figcaption>
</figure>

