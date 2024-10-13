# SWE_2021_41_2024_2_week_6
---
## Week 4 Assingnment 

* Link of your repository \
  https://github.com/inuuuuuu/SWE_2021_41_2024_2_week_4
  
```python
def isHappy(n):

  stor = []

  while n != 1 and n not in stor:
    stor.append(n)
    new = 0
    for i in str(n):
      new += int(i)**2
    n = new

  return n == 1
```

* Description of your code\
  This code is a function that checks whether a given number is a **"happy number"**. A happy number is a number that eventually becomes 1 after repeating the following process:
  1. Calculate the square of each digit of the number and sum them up.
  2. Repeat this process. If the reselt becomes 1, the number is considered a happy number.
  3. If a number that has already appeared during the process appears again, the number can no longer reach 1, and it is not a happy number. 
  
---
## Week 5 Assignment

> ```
> docker exec <ossp-container> cat /etc/os-release
> ```
> * This command displays the content of the /etc/os-release file inside the ossp-container. The file contains details about the operating system used in the container. According to the output, the container is running Ubuntu 24.04.1 LTS.

> ```
> docker exec ossp-containter git --version
> ```
> * This command runs git --version inside the container to check the installed version of Git. According to the output, Git version 2.43.0 is installed in the container. This confirms that Git is available and shows its version.

> ```
> docker exec ossp-container python3 --version
> ```
> * This command runs python3 --version inside the container to check the installed Python 3 version. The output shows that Python 3 version 3.12.3 is installed in the container, confirming that Python 3 is available and providing the exact version.

> ```
> docker inspect --format="{{ .HostConfig.Binds }}" ossp-container
> ```
> * This command uses docker inspect to check the bind mount configuration of the container. The output shows "[.ossp_host_dir:/mnt/ossp_container_dir]", which means that the directory .ossp_host_dir from the host system is mounted to /mnt/ossp_container_dir inside the container. This setup allows the host and container to share files between these directories.

