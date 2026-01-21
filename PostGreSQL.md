  
  
  
  
Depois de baixa-lo, ele ficara nesse caminho( caso for o diretorio padrao) :  
**==C:\Program Files\PostgreSQL\18\==**  
  
ele tera um  (.exe) que usamos para acessa-lo, o psql fica nesse diretorio:   
**==C:\Program Files\PostgreSQL\18\bin\psql.exe==**  
  
Depois de baixado temos que verificar se está rodando   
  
Powershell  
Get-Service -Name 'postgres*'  
  
Para iniciar o serviço  
  
Powershell  
Start-Service -Name 'postgresql-x64-18'  
ou ir no services.msc do windows e startar ele por la  
  
Agora vamos começar a usa-lo  
  
no powershell ou cmd digite  'C:\Program Files\PostgreSQL\18\bin\psql.exe' -U postgres  
  
ele irá pedir a senha que foi configurada na hora da instalação   
após digita-la o aminho mudará para "postgres=#"  
  
![{1970053E-AA69-451A-A196-B3D1DECEBC89}.png](./Estudo/Banco%20de%20dados/%7B1970053E-AA69-451A-A196-B3D1DECEBC89%7D.png)  
  
