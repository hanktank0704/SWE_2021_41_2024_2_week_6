# SWE_2021_41_2024_2_week_6
## Week 4 Assignment
__link to my repository__
https://github.com/hanktank0704/SWE_2021_41_2024_2_week_4
```
def squares(num):
    total = 0
    while num > 0:
        digit = num % 10
        total += digit * digit
        num = num // 10
    return total

def isHappy(n):
  check = set()
  while n != 1:
      if n in check:
          return False
      check.add(n)
      n = squares(n)
  return True

# n = int(input("Input: "))
# result = isHappy(n)
# print("Output:", result)
```
---

## Week 5 Assignment

