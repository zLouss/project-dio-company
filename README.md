# project-dio-company

## Passos realizados

- Criação de uma instancia na Azure para MySQL;
- Criar banco de dados com base disponível no GitHub: https://github.com/julianazanelatto/power_bi_analyst/tree/main/M%C3%B3dulo%203/Desafio%20de%20Projeto;
- Integração do POwer BI com MySQL no Azure;
- Verificar problemas na base  afi de realizar a transformação de dados;

Diretrizes para transformação dos dados:

1. Verifique os cabeçalhos e tipos de dados;

2. Modifique os valores monetários para o tipo double preciso;

3. Verifique a existência dos nulos e analise a remoção;

4. Os employees com nulos em Super_ssn podem ser os gerentes. Verifique se há algum colaborador sem gerente;

5. Verifique se há algum departamento sem gerente;

6. Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas;

7. Verifique o número de horas dos projetos;

8. Separar colunas complexas;

9. Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção;

10. Neste processo elimine as colunas desnecessárias;

11. Realize a junção dos colaboradores e respectivos nomes dos gerentes . Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo;

12. Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores;

13. Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro;
   Utilizamos o mesclar neste caso pois temos uma tabela com os devidos códigos dos departamentos e seus locais, logo trazemos uma informação de uma tabela para outra com o "join" ou "mesclar"
15. Agrupar os dados a fim de sebaer quantos colaboradores existem por gerente
16. Eliminar as colunas desnecessárias;
