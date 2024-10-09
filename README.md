# SWE_2021_41_2024_2_week_6
## Week 4 Assignment
* __link to my repository__\
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

* description of my code
 코드는 주어진 숫자가 행복한 수인지 확인하는 코드이다. 행복한 수란 각 자릿수의 제곱을 반복적으로 더할 경우 1에 도달할 수 있는 수를 의미한다. squares 함수는 입력된 숫자의 각 자릿수를 제곱하고, 그 합을 구한다. isHappy 함수는 특정 숫자가 행복한 수인지 판단하는데, 반복 과정에서 숫자가 1에 도달하면 True를 반환하고, 그렇지 않고 이미 나온 숫자가 다시 등장하면 False를 리턴한다. isHappy 함수는 이를 위해 set를 사용해 이미 나온 숫자들을 기록한다.
---

## Week 5 Assignment

