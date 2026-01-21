  
**Depois de conseguimos conectar no postgree iremos começar a fazer algumas configurações por linha de comando**  
  
*==nesse comando nos criamos um usuário com login e senha==*  
C:\Program Files\PostgreSQL\18\bin\psql.exe' -U postgres -c "CREATE USER meu_usuario WITH PASSWORD 'MinhaSenhaSegura123!';"  
  
*==nesse comando nós criamos um banco de dados ==*  
C:\Program Files\PostgreSQL\18\bin\psql.exe' -U postgres -c "CREATE DATABASE meu_banco OWNER meu_usuario;"  
  
  
# Comandos  
```  
-U postgres -c "CREATE USER Pato WITH PASSWORD 'Pato2469';"  
```  
```  
-U postgres -c "CREATE DATABASE banco_login OWNER Pato;"  
  
```  
'C:\Program Files\PostgreSQL\18\bin\psql.exe' -U postgres -c "CREATE USER Pato WITH PASSWORD 'pato2469';"  
```