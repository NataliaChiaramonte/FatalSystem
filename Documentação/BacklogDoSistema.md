## Backlog do Sistema
### 1. Gerenciamento de chamados
<pre>1.a) Criar chamado:
O sistema deve permitir que o usuário crie um novo chamado, informando título, descrição, categoria e prioridade.
O usuário deve poder revisar os dados preenchidos antes de confirmar o envio do chamado.
O sistema deve permitir anexar um ou mais arquivos ao chamado antes do envio e também após o chamado ter sido criado (enquanto estiver em aberto).<br>
1.a.a) Checar chamado:
Antes de enviar o chamado, o sistema realiza uma primeira checagem para garantir que todos os campos obrigatórios estejam preenchidos. 
Se o sistema identificar um campo em branco, o chamado não é enviado e o funcionário é informado para preencher os dados. 
Caso a dupla checagem seja concluída com sucesso, o funcionário envia o chamado para a equipe de suporte.<br>
1.a.b) Anexar mais arquivos:
Sistema permite anexar mais arquivos em um chamado já existente.<br>
  
1.b) Visualizar chamado:
O sistema deve permitir que o usuário visualize os chamados criados, de acordo com o seu nível de acesso.<br> </pre>

### 2. Gerenciamento de Usuário
<pre>2.a) Cadastrar usuário:
Admin cadastra novo usuário.
Sistema gera matrícula.
Admin cadastra senha.<br>
  
2.b) Editar Usuario:
Adm pode editar usuários já criados<br>
  
2.c)Visualizar usuários
Adm pode visualizar funcionários cadastrados.
Adm vai denominar quais permissões os usuários possuem</pre>

### 3. Gerenciamento de Relatórios

<pre>3.a) Gerar relatórios:
De acordo com o nível de acesso pode gerar relatórios anuais, mensais e semanais.
Gerar relatórios baseado em prioridades.
Gerar relatórios de acordo com o tipo de chamado mais requisitado.<br>

3.b) Buscar relatórios:
Filtrar os relatórios de acordo com data, prioridade e tipo.<br>

3.c) Visualizar relatórios:
Admin pode visualizar os relatórios gerados.</pre>
</pre>

### 4. Gerenciamento de IA

<pre>4.a) Priorizar e categorizar chamados:
A IA deve classificar automaticamente os chamados em níveis de prioridade (alta, média, baixa) com base no conteúdo e na urgência relatada.
A IA vai identificar o chamado e agrupar na sua respectiva categoria.
A IA também deve encaminhar o chamado para o setor responsável com base na análise feita.
O administrador poderá revisar e alterar a prioridade, se necessário.<br>
  
4.b) Aplicar solução inteligente:
IA recebe o chamado.
IA analisa palavras chaves do chamado.
IA concede solução para setor responsável de TI de acordo com o sugerido pelas palavras chaves.<br>

</pre>
</pre>

<br>

## Requisitos Funcionais

### 1. Gerenciamento de chamados

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :------------------: | :----: |
|   1  |    Alta    | O sistema deve permitir que o usuário crie um novo chamado, informando título, descrição, categoria e prioridade.                                                                                              |      10      |          R01         |    ❌   |
|   2  |    Alta    | O usuário deve poder revisar os dados preenchidos antes de confirmar o envio do chamado.                                                                                                                       |      10      |          R04         |    ❌   |
|   3  |    Media    | O sistema deve permitir anexar um arquivo ao chamado antes do envio.                                                                                                                                 |      10      |          R02         |    ❌   |
|   4  |    Alta    | Antes de enviar o chamado, o sistema realiza uma primeira checagem para garantir que todos os campos obrigatórios estejam preenchidos.                                                                         |      10       |          R02         |    ❌   |
|   5  |    Alta    | Se o sistema identificar um campo em branco, o chamado não é enviado e o funcionário deverá ser informado para preencher os dados.                                                                              |      10      |          R02         |    ❌   |
|   6  |    Baixa    | Sistema permite anexar mais arquivos em um chamado já existente.                                                                                                                                               |       10       |          R03         |    ❌   |
|   7  |    Alta    | O sistema deve permitir que o usuário visualize os chamados criados, de acordo com o seu nível de acesso.                                                                                                      |       10       |          R05         |    ❌   |
|   8  |    Alta   | A equipe de TI deverá analisar os chamados encaminhados pela IA, de acordo com a prioridade definida e atualizar o status do chamado.                                                                            |      10       |          R09         |    ❌   |
|   9  |    Alta   | O Admin pode alterar a prioridade do chamado após sua abertura e classificação pela IA.                                                                                                                        |      10       |          R10         |    ❌   |


### 2. Gerenciamento de Usuário

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :------------------: | :----: |
|  10  |    Alta   | Administrador poderá cadastrar novos usuários na plataforma, para que somente pessoas autorizadas possam acessá-la.                                                                                    |      10       |          R01         |    ❌   |
|  11  |    Alta   | Usuário deverá  acessar a aplicação através de uma interface de login, para que somente usuários autorizados possam utilizar o sistema.                                                                 |      10       |          R01         |    ❌   |
|  12  |    Alta   | Usuário autorizado deverá acessar o sistema através de um login, para utilizar a aplicação.                                                                                                            |      10       |          R01         |    ❌   |
|  13  |    Alta   | Usuário autenticado poderá fazer o logout da aplicação de forma segura, para que seus dados não fiquem acessíveis a terceiros.                                                                          |      10       |          R01         |    ❌   |
|  14  |    Média   | Administrador poderá editar os dados dos usuários, caso os mesmos solicitem.                                                                                                                             |       7       |          R06         |    ❌   |
|  15  |    Média   | Administrador poderá visualizar a lista de usuários cadastrados, para que possa gerenciar quem tem acesso ao sistema.                                                                                     |      7       |          R05         |    ❌   |
|  16  |    Media   | Administrador poderá redefinir a senha de um usuário, para que possa ajudá-lo caso ele não consiga acessar a conta.                                                                                       |      10       |          R06         |    ❌   |
|  17  |    Alta   | Administrador poderá revogar acesso de usuários cadastrados.                                                                                                                                                |      10       |          R06         |    ❌   |
|  18  |    Alta   | O sistema deve garantir a proteção dos dados dos usuarios conforme as diretrizes da LGPD.                                                                                                                     |       10      |          R12         |    ❌   |



### 3. Gerenciamento de Relatórios

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :------------------: | :----: |
|  19  |    Media   | Usuário, de acordo com o nível de acesso, poderá gerar relatórios anuais, mensais e semanais.                                                                                                              |       7       |          R11         |    ❌   |
|  20  |    Baixa   | Usuário poderá gerar relatórios baseado em prioridades.                                                                                                                                                   |       5       |          R11         |    ❌   |
|  21  |    Baixa   | Usuário poderá gerar relatórios de acordo com o tipo de chamado mais requisitado.                                                                                                                         |      5       |          R11         |    ❌   |
|  22  |    Baixa   | Usuário poderá filtrar os relatórios de acordo com data, prioridade e tipo.                                                                                                                               |      5       |          R11         |    ❌   |
|  23  |    Baixa   | Administrador poderá visualizar os relatórios gerados.                                                                                                                                                     |      5       |          R11         |    ❌   |

### 4. Gerenciamento de IA

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :------------------: | :----: |
|  24  |    Alta   | A IA deverá classificar automaticamente os chamados em níveis de prioridade (alta, média, baixa) com base no conteúdo e na urgência relatada.                                                                    |      10       |          R07         |    ❌   |
|  25  |    Alta   | A IA irá identificar o chamado, agrupar na sua respectiva categoria.                                                                                                                                                     |      10      |          R08         |    ❌   |
|  26  |    Alta   | A IA irá sugerir uma solução e encaminhar para o setor responsável de TI.                                                                                                                                                |      10      |          R08         |    ❌   | 
|  27  |    Media   | O Admin poderá atualizar o banco de dados da IA baseado no historico de chamados resolvidos.                                                                                                                             |      10     |          R10         |    ❌   |
