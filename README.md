# Avaliação de Banco de Dados

### PDF para a realização da Avaliação de Banco de dados

[Clique aqui para acessar o PDF](AtividadeAvaliativa.pdf)

## Mapa conceitual:
![](Avaliacaobd_conceitual.png)

## Mapa Lógico:
![](AvaliacaoBD_logico.png)

## Descrição da Avaliação 
## Tabela alunos
#### Tabela alunos se refere aos dados dos alunos cadastrados nesta escola. Nela possuímos os atributos/colunas:

- mat: matricula do aluno/chave primária da tabela
- nome: nome do aluno cadastrado
- endereco: endereço do aluno cadastrado nesta escola
- cidade: informação importante referente ao aluno e onde se localiza sua residencia
## Tabela turma
#### Table turma se refere a turma em que as disciplinas e professores foram atribuidos a ela. Nela possuímos os atributos/colunas:

- cod_turma: chave primária
- cod_disc: chave estrangeira
- cod_prof: chave estrangeira
- ano: ano em que a turma está
- horario: harario em que cada turma irá ter, referente as aulas

## Tabela disciplinas
#### Tabela disciplinas se refere as disciplinas em que a turma que o aluno foi atribuido irá ter. Nela possuímos os atributos/colunas:

- cod_disc: chave primária da tabela
- nome_disc: o nome das disciplinas
- carga_hor: a carga horaria de cada disciplina

## Tabela professores
#### Tabela professores se refere ao professores que irá ter em cada turma. Nela possuímos os atributos/colunas:

- cod_prof: chave primária da tabela
- nome: nome do professor
- endereco: endereço do professor
- cidade: informação importante referente ao professor e onde se localiza sua residencia

## Tabela historico
#### Tabela historico se refere a todas as outras tabelas tornando suas chaves primária para cheves estrangeira. Nela possuímos os atributos/colunas:

- cod_disc: chave estrangeira
- disc_turma: chave estrangeira
- cod_prof: chave estrangeira
- ano: ano da tabela historico
- mat: chave estrangeira

## Tabela turma_disc 
- Ela faz o relaciomento entre as tabelas: disciplina e turma
-fk_disciplina_cod_disc: chave estrangeira que faz referência a tabela disciplina

## Tabela turma_prof
- Ela faz relacionamento entre as tabelas: turma e professores 
- fk_professores_cod_prof: chave estrangeira que faz referência a tabela professores

 ## Tabela historico_aluno
 - é a junção das tabelas historico e aluno

 # Inspirações
https://github.com/caffeine-squad/modelagem_bd
