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
> * This command runs cat /etc/os-release inside the running container named ossp-container. The /etc/os-release file contains details about the operating system in the container, such as the OS name, version, and other related metadata. This command is used to inspect which Linux distribution is running inside the container.

> ```
> docker exec ossp-containter git --version
> ```
> * This command runs git --version inside the ossp-container container to check the installed version of Git. It is useful to verify whether Git is installed in the container and which version is present.

> ```
> docker exec ossp-container python3 --version
> ```
> * This command runs python3 --version inside the ossp-container container to check the installed version of Python 3. It ensures that Python 3 is installed and lets you know the exact version.

> ```
> docker inspect --format="{{ .HostConfig.Binds }}" ossp-container
> ```
> * This command uses docker inspect to retrieve the configuration details of the ossp-container container. The --format="{{ .HostConfig.Binds }}" part formats the output to specifically show the bind mounts, i.e., directories or files from the host system that are mounted into the container. This is helpful to check how the container’s file system is linked to the host system.

