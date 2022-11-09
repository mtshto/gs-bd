# gs-bd

## Create table 
CREATE TABLE dept
(deptno NUMBER(2),
dname VARCHAR2(14),
loc VARCHAR2(13),
create_date DATE DEFAULT SYSDATE);

## ALTER TABLE

1. Adicionando uma nova Coluna
ALTER TABLE DEPT ADD Total_sal number(10,2);
2. Modificando uma coluna existente
ALTER TABLE DEPT ADD Total_sal number(10,2);
4. Renomeando uma coluna
ALTER TABLE DEPT RENAME COLUMN total_sal TO Total_Salario;
6. Removendo uma coluna
ALTER TABLE DEPT DROP COLUMN total_Salario;

## Drop TABLE

1. Removendo uma tabela
DROP TABLE EMPREGADOS;
2. Removendo uma tabela sem enviar para lixeira
DROP TABLE EMPREGADOS PURGE;
3. Removendo uma tabela com referência de FK
DROP TABLE DEPT CASCADE CONSTRAINTS;

