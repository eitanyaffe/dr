<<<<<<< HEAD
# dckr

1. Run make install.

2. Add /etc/docker/tools to your path.

3. Add to the end of /etc/sudoers this line:
ALL	ALL=(ALL) NOPASSWD: /usr/bin/dckr

4. See examples in /etc/docker/tools.
=======
# dckr: A docker wrapper

```
Usage: ./dckr <command> [-p <profile>] [-i <image>] [-n <name>] [-k <key>] <container_commands>
Commands:
  run: Run a container command on an docker image
  up: Create a singleton container and associate with a key
  down: Remove a singleton container associated with a key
  exec: Execute commands on singleton container associated with key
  ps: Show all running containers
Options:
  -i <image>: Docker image
  -p <file>: Profile file (default: '')
  -k <key>: Singleton key (Required only for up/down/exec commands)
  -n <name>: Specify container name for non-singlton container (default: none)
  -h: Create mounts for /home (default: false)
  -d: Print command line without executing (dry run)
  ```
>>>>>>> e4d6216581fe3c95cd01e7cb429865c5a46adfe2
