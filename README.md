<h1>Backup Camunda</h1>
Script desenvolvido para facilitar processo de backup do software Camunda, o script atualmente recupera dados do banco de dados (Postgres/MariaDB/Mysql), e também recupera os Jars customizados adicionados pelo usuário.

<h2>Informações importantes</h2>
O script te da a possibilidade de realizar backups incrementais do Jars utilizados no Camunda. No entanto, o backup do Jars é realizado recuperando os arquivos criados por meio de "Volumes" específicos. Ele não pegará diretamente os arquivos do Container. Para que o script funcione corretamente, é necessário criar volumes para a pasta "lib" do Camunda.

<h2>Pré-requisitos</h2>
Antes de executar certifique-se que o ambiente "Camunda" esteja  configurado.

<h2>Como utilizar o script</h2>

- Primeiro, certifique-se de ter criado os volumes necessários para a pasta "lib" do Camunda:

- Agora, você pode executar o script de backup usando o seguinte comando:
```
./backup-camunda-docker.sh
```
