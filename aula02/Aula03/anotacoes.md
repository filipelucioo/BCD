##
Para apagar um Banco de Dados, ultilizamos o comando:

```sql
DROP DATABASE cidades;
```
 >não esquecer do ";"

 ---

 **Modelagem do banco de dados**
```mermaid
erDiagram
PRODUTOS {
    int id PK "Gerado Automaticamente"
    varchar nome "Nome do produto"
    numeric valor "Preço do produto em R$"
    estoque 
}
```
Apos modelar, iremos executar as etapas de criação e inserção de dados.
---
Para criar a primeira tabela, usamos os comandos:
```sql
CREATE TABLE produtos(
    id INT GENERATED ALWAYS AS IDENTITY PRIMARY KEY, 
    nome VARCHAR(100) NOT NULL,
    valor NUMERIC(10,2) NOT NULL,
    estoque INT NOT NULL DEFAULT 0 
);
```

Para consultar todos elementos da tabela, uso o comando:

```sql
SELECT * FROM produtos;
```
---
Para inserir dados na tabela, usamos o segu te comando:
```sql
INSERT INTO produtos(nome,valor,estoque)
VALUES('Caneta','1.50','100');
```