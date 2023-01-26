# scripts-para-demos

## oracle
* 1 - Rodar imagem docker oficial do Oracle XE:

```
sudo docker run --name myoracledb \
-p 1521:1521 -p 5500:5500 \
-e ORACLE_PWD=Demo123% \
container-registry.oracle.com/database/express:21.3.0-xe
```
* 2 - Executar scripts para criação de usuário, criação de objetos e carga de dados:
```
https://github.com/eumagnun/scripts-para-demos/tree/main/oracle
```
