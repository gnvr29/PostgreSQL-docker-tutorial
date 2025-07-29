# PostgreSQL-docker-tutorial
Tutorial used during Levty's backend Journey about creating and running a local PostgreSQL container.

Execute the following to start the container:

```bash
docker compose up -d
```

Once the container is running, execute the following to enter the postgres CLI:

```bash
docker exec -it <container-name> -U <postgres-username> -d <database-name>
```

You can then copy and paste the SQL commands in the terminal and check if everything worked as intented. 

You can also execute one of the following commands to check for DB and connection metadata:

```sql
SELECT version();
```

```sql
\conninfo;
```

Type \q to exit the CLI, use the following command to stop the container:

```bash
docker compose down
```
Add the -v flag to remove the volume as well.
