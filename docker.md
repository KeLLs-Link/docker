## Managing Containers

You cannot remove or delete a running container. But however, you can use this command to force remove a running container. By introducing the -f flag

```
docker rm -f $(docker ps -aq)
```
**`docker ps:`** This command lists all running containers.

**`-aq:** These are flags used with docker ps.

**`-a`** shows all containers (not just running ones), and 

**`-q`** displays only the IDs of the containers.
So, docker ps -aq will list the IDs of all containers, whether they are running or stopped.

**`docker rm:`** This command removes one or more containers.

**`-f:`** This flag forces the removal of a running container. ***(it's generally safer to stop a container before removing it, but -f bypasses that).***

![image](./screenshots/containerforcedshutdown.png)