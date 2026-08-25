## Parte 01
Criação e inserção de dados, Realizando algumas consultas avançadas

Criando tabelas
```sql
CREATE TABLE produtos(
    id SERIAL PRIMARY KEY,
    nome VARCHAR(60) NOT NULL,
    valor DECIMAL(10,2) NOT NULL,
    categoria VARCHAR (30) NOT NULL,
    estoque INTEGER NOT NULL
)
```
Filtrando registos:
```sql
SELECT * FROM produtos LIMIT 5
```
 Para filtrar colunas:
```sql
SELECT nome,valor,categoria FROM produtos;
```
Para vizualizar só as categorias:
```sql
SELECT DISTINCT categoria FROM produtos ORDER BY categoria;
```

## Parte 02 
Filtro de dados. 

Para filtrar um dado da categoria:
```sql
SELECT nome,estoque FROM produtos WHERE categoria = 'Monitores';
```
Para filtrar por valor:
```sql
SELECT nome,estoque FROM produtos WHERE valor > 1000;
```
ou
```sql
SELECT nome,estoque FROM produtos WHERE valor > BETWEEN 100 and 500;
```
Para filtrar pro nome:
```sql
SELECT nome,estoque FROM produtos WHERE nome LIKE 'Mouse%';
```

