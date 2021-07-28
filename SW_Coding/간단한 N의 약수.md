# Problem

입력으로 1개의 정수 N 이 주어진다.

정수 N 의 약수를 오름차순으로 출력하는 프로그램을 작성하라.

-------------------

# Solution

```
t = int(input())
for i in range(1,t+1):
    if(t%i==0):
        print(i, end=' ')
```

-----------------------

https://swexpertacademy.com/main/code/problem/problemDetail.do?contestProbId=AV5PhcWaAKIDFAUq&categoryId=AV5PhcWaAKIDFAUq&categoryType=CODE&problemTitle=%EA%B0%84%EB%8B%A8%ED%95%9C&orderBy=FIRST_REG_DATETIME&selectCodeLang=ALL&select-1=&pageSize=10&pageIndex=1
