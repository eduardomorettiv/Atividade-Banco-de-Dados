# Atividade — Banco de Dados da Turma
# Objetivo
Criar um banco de dados para representar os alunos de uma turma, aplicando os conhecimentos de **modelagem de dados e SQL.**

### Situação-problema

A escola deseja organizar as informações dos alunos de uma determinada turma em um banco de dados.
Sua equipe deverá criar uma representação dos dados da turma e, posteriormente, transformar essa representação em um banco de dados utilizando MySQL.

# Tabela de Dados

Crie uma tabela de dados contendo pelo menos 3 alunos da turma.

A tabela deverá conter: 

<div>
  <img src = ""
</div>
  
# MER — Modelo Entidade-Relacionamento

Com base na tabela criada, desenvolva o MER do sistema.
O modelo deverá apresentar:

. **Entidade**: Aluno

. **Atributos**: Número , Nome, Idade, Data de Nascimento, E-mail

. Identificação da **chave primária**

. Relacionamentos, caso sejam criados mais elementos no modelo

# DER Conceitual

A partir do MER, desenvolva o DER Conceitual, representando graficamente a estrutura do banco de dados.

O diagrama deverá apresentar:

**ALUNO**

. Número;

. Nome;

. Idade;

. Data de Nascimento;

. E-mail.

Identifique claramente a **chave primária (PK).**

# Código MySQL

Por último, transforme o modelo criado em **código SQL.**

O banco deverá se chamar:

**SQL** ->
turma

**SQL** ->
aluno

**O código deverá conter:**

. criação do banco;

. criação da tabela;

. definição dos campos;

. chave primária;

. inserção de no **mínimo** 3 alunos e no **máximo** 10 alunos.

**Exemplo:**
```
CREATE DATABASE turma;

USE turma;

CREATE TABLE turmas (
    id INT PRIMARY KEY,
    nome VARCHAR(50)
);

CREATE TABLE alunos (
    numero INT PRIMARY KEY,
    nome VARCHAR(100),
    idade INT,
    data_nascimento DATE,
    email VARCHAR(100),
    id_turma INT
);

ALTER TABLE alunos ADD CONSTRAINT pertence FOREIGN KEY (id_turma) REFERENCES turmas(id);
```
# Entrega

**Cada aluno deverá entregar:**

**1.** Tabela de dados

**2.** MER

**3.** DER Conceitual

**4.** Código MySQL


