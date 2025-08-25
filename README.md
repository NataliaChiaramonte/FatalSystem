# Gerenciamento de chamados

Esse trabalho é referente ao Projeto Integrado Multidisciplinar da Faculdade UNIP de São José dos Campos, criado em equipe.
<br>
    
<br>

<h2 align="center"> Fatal System</h2>
<br>
<p align="center">
      <img src="Logotipo/FatalSystemSemMargem.jpg" alt="logo da Fatal System" width="400">
<br>

## Desafio <a id="desafio"></a>
O desafio proposto é desenvolver um sistema de gestão de chamados, apoiado por Inteligência Artificial (IA), capaz de otimizar o atendimento interno.
Nesse sistema, os chamados registrados pelos usuários serão analisados automaticamente pela IA, que sugerirá soluções inteligentes à equipe de TI. Caberá à equipe validar essas recomendações, podendo aprová-las, ajustá-las ou descartá-las.

Todas as interações ficam registradas em um repositório centralizado, assegurando rastreabilidade e alimentando o processo de aprendizado contínuo da IA. Esse histórico poderá ser consultado tanto pela equipe técnica quanto pelo administrador e pela própria inteligência artificial, servindo de base para análises e apoio em decisões futuras.

O propósito central é tornar o fluxo de atendimento mais ágil, diminuir a carga de trabalho da equipe de TI e aumentar a eficiência na resolução de chamados dentro da organização.

<br>

## Solução Proposta
* Classificação e priorização automática de chamados por Inteligência Artificial.
* Sugestão de soluções pela IA para apoio à equipe de TI.
* Emissão de relatórios periódicos (semanais, mensais e anuais) sobre os chamados.
* Gerenciamento de usuários pelo administrador.

<br>

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
|  9  |    Alta    | Como Administrador, eu gostaria de ser o primeiro usuário do sistema, já devidamente pré inserido no banco de dados, para que possa acessar a aplicação.                                                       |             |       |          R09         |    ❌   |
|  10  |    Média   | Como Administrador, eu quero cadastrar novos usuários na plataforma, para que somente pessoas autorizadas possam acessá-la.                                                                                    |            |       |          R10         |    ❌   |
|  11  |    Média   | Como usuário, eu quero acessar a aplicação através de uma interface de login, para que somente usuários autorizados possam utilizar o sistema.                                                                 |            |       |          R11         |    ❌   |
|  12  |    Média   | Como usuário autorizado, eu quero acessar o sistema através de um login, para utilizar a aplicação.                                                                                                            |            |       |          R12         |    ❌   |
|  13  |    Média   | Como usuário autenticado, eu quero poder fazer o logout da aplicação de forma segura, para que meus dados não fiquem acessíveis a terceiros.                                                                   |            |       |          R13         |    ❌   |
|  14  |    Média   | Como Administrador, quero poder editar os dados dos usuarios, caso os mesmos solicitem.                                                                                                                        |            |       |          R14         |    ❌   |
|  15  |    Média   | Como Administrador, eu quero visualizar a lista de usuários cadastrados, para que eu possa gerenciar quem tem acesso ao sistema.                                                                               |            |       |          R15         |    ❌   |
|  16  |    Média   | Como Administrador, eu quero redefinir a senha de um usuário, para que eu possa ajudá-lo caso ele não consiga acessar a conta.                                                                                 |            |       |          R16         |    ❌   |
|  17  |    Média   | Como Administrador, eu quero excluir usuários do sistema, para que possa revogar o acesso de usuários a aplicação.                                                                                             |            |       |          R17         |    ❌   |
|  18  |    Baixa   | Como Administrador, ter a capacidade de denominar niveis de acesso ao sistema de acordo com a função do funcionario.                                                                                           |            |       |          R18         |    ❌   |



### 3. Gerenciamento de Relatórios

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  19  |    Baixa   | Como usuário, De acordo com o nível de acesso, gerar relatórios anuais, mensais e semanais.                                                                                                                    |             |       |          R19         |    ❌   |
|  20  |    Baixa   | Como usuário, Poder gerar relatórios baseado em prioridades.                                                                                                                                                   |             |       |          R20         |    ❌   |
|  21  |    Baixa   | Como usuário, Gerar relatórios de acordo com o tipo de chamado mais requisitado.                                                                                                                               |             |       |          R21         |    ❌   |
|  22  |    Baixa   | Como usuario, poder Filtrar os relatórios de acordo com data, prioridade e tipo.                                                                                                                               |             |       |          R22         |    ❌   |
|  23  |    Baixa   | Como Admnistrador, poder visualizar os relatórios gerados.                                                                                                                                                     |             |       |          R23         |    ❌   |

### 4. Gerenciamento de IA

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  24  |    Baixa   | A IA deve classificar automaticamente os chamados em níveis de prioridade (alta, média, baixa) com base no conteúdo e na urgência relatada.                                                                    |            |       |          R24         |    ❌   |
|  25  |    Baixa   | A IA vai identificar o chamado e agrupar na sua respectiva categoria.                                                                                                                                          |            |       |          R25         |    ❌   |
|  26  |    Baixa   | IA recebe o chamado e analisa as palavras chaves.                                                                                                                                                              |            |       |          R26         |    ❌   |
|  27  |    Baixa   | A IA também deve encaminhar o chamado para o setor responsável com base na análise feita.                                                                                                                      |            |       |          R27         |    ❌   |
|  28  |    Baixa   | IA concede solução para setor responsável de TI de acordo com o sugerido pelas palavras chaves.                                                                                                                |            |       |          R28         |    ❌   |

<br>

## Tecnologias Utilizadas
* [Figma](https://www.figma.com/)
* [Astah](https://astah.net/)
* [Br Modelo](https://www.brmodeloweb.com/lang/pt-br/index.html)
* [SQL Server](https://www.microsoft.com/pt-br/sql-server/sql-server-downloads)
<br>

## DoR - Definition of Ready
* Design no <strong>Figma</strong>
* Diagramas e modelagem do sistema no <strong>Astah</strong>
* Diagrama de estruturação do Banco de Dados no <strong>Br Modelo</strong>
* Modelagem do Banco de Dados no <strong>SQL Server</strong>
<br>

## Integrantes do grupo

| Nome                          | Papel         | GitHub                                    |
| ----------------------------- | ------------- |------------------------------------------ |
| Natália Chiaramonte Fernandes     | Desenvolvedora |[GitHub](https://github.com/NataliaChiaramonte) |
