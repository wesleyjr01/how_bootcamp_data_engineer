# how_bootcamp_data_engineer

How Bootcamps - Data Engineering, by Andre Sionek (2021/03).

### Redshift

- O Redshift e um servico de armazenamento de dados em escala. O Redshift eh criado em cima do PostgresSQL e ele serve pra voce fazer bancos de dados analyticos. Ele eh um banco escalavel horizontalmente. Voce consegue ao inves de aumentar o tamanho da maquina, aumentar a quantidade de nos disponiveis pra computar. (O RDS nao eh escalavel horizontalmente)
- O Redshift eh um banco de dados colunar, ou seja, voltado para operacoes de select, melhor performance para fazer select nos dados.

### IAM

- **Role (funcao)**:
  - Uma funcao e uma entidade do IAM que define um conjunto de permissoes para efetuar solicitacoes de servicos da AWS. Os Roles nao sao associados a um usuario ou grupo especifico. Em vez disso, entidades de confianca assumem funcoes, como usuaros do IAM, aplicativos ou servicos da AWS, como o EC2. O Role pode ser atribuido tanto para um usuario quanto para um servico, o Role eh basicamento um conjunto de permissoes que deixa a gente acessar determinados recursos da AWS.
- **Policy**:

  - Uma politica e uma entidade que, quando anexada a uma identidade ou recurso, define suas permissoes.
  - Dentro do Role eu posso associar varias politicas, e eh dentro da politica que a gente define que servico ou que recurso o usuario consegue acessar.

- **Boas Praticas com IAM:**
  - Conceda privilegio minimo aos usuarios recem criados
  - Use grupos para atribuir permissoes para usuarios do IAM. Dentro do grupo nos teremos Roles que atribuem permissoes, e ai nos inserimos usuarios nos Grupos.

### AWS Kinesis (2:32min)

- Facilita coleta, processamento e analise de dados de streaming em tempo real.
- Vamos simular eventos chegando no Kinesis e vamos salvar estes eventos no bucket no S3. Vamos usar na verdade o Kinesis Firehose.
