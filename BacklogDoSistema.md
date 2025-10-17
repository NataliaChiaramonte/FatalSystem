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

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|   1  |    Alta    | O sistema deve permitir que o usuário crie um novo chamado, informando título, descrição, categoria e prioridade.                                                                                              |            |       |          R01         |    ❌   |
|   2  |    Alta    | O usuário deve poder revisar os dados preenchidos antes de confirmar o envio do chamado.                                                                                                                       |            |       |          R02         |    ❌   |
|   3  |    Alta    | O sistema deve permitir anexar um ou mais arquivos ao chamado antes do envio e também após o chamado ter sido criado (enquanto estiver em aberto)                                                              |            |       |          R03         |    ❌   |
|   4  |    Alta    | Antes de enviar o chamado, o sistema realiza uma primeira checagem para garantir que todos os campos obrigatórios estejam preenchidos.                                                                         |            |       |          R04         |    ❌   |
|   5  |    Alta    | Se o sistema identificar um campo em branco, o chamado não é enviado e o funcionário é informado para preencher os dados.                                                                                      |            |       |          R05         |    ❌   |
|   6  |    Alta    | Caso a dupla checagem seja concluída com sucesso, o funcionário envia o chamado para a equipe de suporte.                                                                                                      |            |       |          R06         |    ❌   |
|   7  |    Alta    | Sistema permite anexar mais arquivos em um chamado já existente.                                                                                                                                               |            |       |          R07         |    ❌   |
|   8  |    Alta    | O sistema deve permitir que o usuário visualize os chamados criados, de acordo com o seu nível de acesso.                                                                                                      |            |       |          R08         |    ❌   |


### 2. Gerenciamento de Usuário

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  9  |    Alta    | Administrador deverá ser o primeiro usuário do sistema, já devidamente pré inserido no banco de dados, para que possa acessar a aplicação.                                                       |             |       |          R09         |    ❌   |
|  10  |    Média   | Administrador poderá cadastrar novos usuários na plataforma, para que somente pessoas autorizadas possam acessá-la.                                                                                    |            |       |          R10         |    ❌   |
|  11  |    Média   | Usuário autorizado deverá acessar o sistema através de um login, para utilizar a aplicação.                                                                                                            |            |       |          R11         |    ❌   |
|  12  |    Média   | Usuário autenticado poderá fazer o logout da aplicação de forma segura, para que meus dados não fiquem acessíveis a terceiros.                                                                   |            |       |          R12         |    ❌   |
|  13  |    Média   | Administrador poderá editar os dados dos usuários, caso os mesmos solicitem.                                                                                                                        |            |       |          R13         |    ❌   |
|  14  |    Média   | Administrador poderá visualizar a lista de usuários cadastrados, para que eu possa gerenciar quem tem acesso ao sistema.                                                                               |            |       |          R14         |    ❌   |
|  15  |    Média   | Administrador poderá redefinir a senha de um usuário, para que eu possa ajudá-lo caso ele não consiga acessar a conta.                                                                                 |            |       |          R15         |    ❌   |
|  16  |    Média   | Administrador poderá excluir usuários do sistema, para que possa revogar o acesso de usuários a aplicação.                                                                                             |            |       |          R16         |    ❌   |
|  17  |    Baixa   | Administrador deverá ter a capacidade de denominar níveis de acesso ao sistema de acordo com a função do funcionário.                                                                                           |            |       |          R17         |    ❌   |



### 3. Gerenciamento de Relatórios

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  18  |    Baixa   | Usuário, de acordo com o nível de acesso, poderá gerar relatórios anuais, mensais e semanais.                                                                                                                    |             |      |          R18         |    ❌   |
|  19  |    Baixa   | Usuário poderá gerar relatórios baseado em prioridades.                                                                                                                                                   |             |       |          R19         |    ❌   |
|  20  |    Baixa   | Usuário poderá gerar relatórios de acordo com o tipo de chamado mais requisitado.                                                                                                                               |             |       |          R20         |    ❌   |
|  21  |    Baixa   | Usuário poderá filtrar os relatórios de acordo com data, prioridade e tipo.                                                                                                                               |             |       |          R21         |    ❌   |
|  22  |    Baixa   | Admnistrador poderá visualizar os relatórios gerados.                                                                                                                                                     |             |       |          R22         |    ❌   |

### 4. Gerenciamento de IA

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  23  |    Baixa   | A IA deverá classificar automaticamente os chamados em níveis de prioridade (alta, média, baixa) com base no conteúdo e na urgência relatada.                                                                    |            |       |          R23         |    ❌   |
|  24  |    Baixa   | A IA irá identificar o chamado e agrupar na sua respectiva categoria.                                                                                                                                          |            |       |          R24         |    ❌   |
|  25  |    Baixa   | IA receberá o chamado e analisa as palavras chaves.                                                                                                                                                              |            |       |          R25         |    ❌   |
|  26  |    Baixa   | A IA também deverá encaminhar o chamado para o setor responsável com base na análise feita.                                                                                                                      |            |       |          R26         |    ❌   |
|  27  |    Baixa   | IA concede solução para setor responsável de TI de acordo com o sugerido pelas palavras chaves.                                                                                                                |            |       |          R27         |    ❌   |
