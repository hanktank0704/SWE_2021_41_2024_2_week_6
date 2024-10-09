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

* description of my code\
 코드는 주어진 숫자가 행복한 수인지 확인하는 코드이다. 행복한 수란 각 자릿수의 제곱을 반복적으로 더할 경우 1에 도달할 수 있는 수를 의미한다. squares 함수는 입력된 숫자의 각 자릿수를 제곱하고, 그 합을 구한다. isHappy 함수는 특정 숫자가 행복한 수인지 판단하는데, 반복 과정에서 숫자가 1에 도달하면 True를 반환하고, 그렇지 않고 이미 나온 숫자가 다시 등장하면 False를 리턴한다. isHappy 함수는 이를 위해 set를 사용해 이미 나온 숫자들을 기록한다.

---

## Week 5 Assignment
![스크린샷 2024-10-02 191711](https://github.com/user-attachments/assets/e6740819-648e-41e3-b2e0-9b5f6ba32c6a)
1. docker exec <container_name> cat /etc/os-release\
이 명령어는 ossp-container 컨테이너 내부의 운영체제 정보를 출력합니다.\
컨테이너가 Ubuntu 24.04.1 LTS를 사용하고 있으며, 지원, 버그 신고, 개인정보 정책에 대한 URL도 함께 표시됩니다.

3. docker exec <container_name> git --version\
컨테이너에 설치되어 있는 git의 버전에 대한 정보를 출력합니다.\
컨테이너에 git 2.43 버전이 설치되어있습니다.

4. docker exec <container_name> python3 --version\
컨테이너 내부에 설치되어 있는 python의 버전에 대한 정보를 출력합니다.\
python 3.12.3 버전을 설치했습니다.

5. docker inspect --format="{{ .HostConfig.Binds }}" <container_name>\
컨테이너의 bind 설정에 대한 정보를 출력합니다. 호스트와 컨테이너 사이에 바인딩이 되어 있는 지 확인합니다.\
결과에서는 ossp host dir, ossp container dir와 바인딩이 되어 있어 컨테이너가 호스트의 파일에 접근할 수 있습니다.


