<p align="center">
  <img src="https://github.com/faraguti/MSSQL-Server-Agent-Manual-Start/assets/5418256/6cd92d74-4e1a-4331-9b07-78391b69ac3c" height="100%" width="200%">
</p>


## How to Manually Start SQL Server Agent in a MSSQL Docker Container

Follow these steps to manually start the SQL Server Agent within a Docker container.

### Step 1: Check Container Status

First, check the status of your container and retrieve its name by running the following command:

```
docker ps -a
```
- This command lists all containers, including stopped ones.
- The -a flag ensures visibility of stopped containers as well.
> [!NOTE]  
> **Write down the container name for the next steps.**
