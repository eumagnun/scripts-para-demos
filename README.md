# scripts-para-demos

## oracle

* 1 - Rodar imagem docker oficial do Oracle XE:

```
sudo docker run --name myoracledb \
-p 1521:1521 -p 5500:5500 \
-e ORACLE_PWD=Demo123% \
container-registry.oracle.com/database/express:21.3.0-xe
```
* 2 - criar novo usuário/schema
```
CREATE USER c##demo IDENTIFIED BY demo123;
/
GRANT ALL PRIVILEGES TO c##demo;
/
```
* 3 - Logar com o novo usuário e executar o scripts conforme abaixo:
```
@2_create_objects.sql
@3_load_data.sql
commit;
```
