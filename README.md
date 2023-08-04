<p align="center">
  <img src="https://github.com/faraguti/MSSQL-Server-Agent-Manual-Start/assets/5418256/6cd92d74-4e1a-4331-9b07-78391b69ac3c" height="100%" width="100%">
</p>


## How to Manually Start SQL Server Agent in a MSSQL Docker Container

Follow these steps to manually start the SQL Server Agent within a Docker container.

### Step 1: Check Container Status

First, check the status of your container and retrieve its name by running the following command:

```
docker ps -a
```
- This command lists all containers, including stopped ones.
- The `-a` flag ensures visibility of stopped containers as well.
> [!NOTE]  
> **Write down the container name for the next steps.**
> 
<br></br>
<img src="https://github.com/faraguti/MSSQL-Server-Agent-Manual-Start/assets/5418256/5a9a622d-85b3-415a-a3d2-f1bd2557341b" height="90%" width="90%">

![image]()


<br></br>
### Step 2: Connect to the Container

Now, connect to the container using the root account with this command:
```
docker exec -it -u root <container-name> bash
```
> [!IMPORTANT]
> **Breakdown of each part of the command:**
    
- `docker exec`: This is the command used to execute a command inside a running container.
- `-it`: These flags indicate that the session should be interactive and allocate a pseudo-TTY (terminal).
- `-u root`: This flag specifies that the command should be executed as the "root" user inside the container.
- `<container-name>`: This is a placeholder for the actual name of the Docker container you want to connect to.
- `bash`: This is the command that will be executed within the container, which opens an interactive shell (the Bash shell in this case).
