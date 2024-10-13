# SWE_2021_41_2024_2_week_6

## Week 4 Assingnment 
---
__unordered list__
* Link of your repository
<pre>
'''python
def isHappy(n):

  stor = []

  while n != 1 and n not in stor:
    stor.append(n)
    new = 0
    for i in str(n):
      new += int(i)**2
    n = new

  return n == 1
'''
</pre>
* Description of your code
