## Criando Nosso Primeiro Banco de Dados

Para acessar os bancos de dados no Moba, usamos o seguinte comando:
```bash
sudo -u postgres psql
```
---
Criando nosso Banco de dados no moba (usuario: postgres):

>Para criar o Banco de dados, usamos esse comando:
```sql
CREATE DATABASE cidades;
```
![alt text](<Captura de tela 2026-08-13 101329.png>)

Para verificar os Bancos de dados existentes:
```sql
\l
```
Após isso, sairemos do postgres e reiniciamos ele com o codigo:
```sql
sudo systemctl restart postgresql
```
---
Agora abrimos o VScode e instalamos esta extensão:

![alt text](<Captura de tela 2026-08-06 112458.png>)

Abrimos ela e clicamos no botão de + para fazer a conexão e executamos o seguinte comando:

>ip do servidor; postgresql; senha do postgres; 5432; standart connection; show all database.

---
Agora, faremos seguintes comandos:

![alt text](<Captura de tela 2026-08-13 105339.png>)

> F5 para vizualizar a tabela.
---
**No final ficará assim:**
![alt text](image.png)



 




