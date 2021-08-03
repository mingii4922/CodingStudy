# Problem

다음과 같이 Encoding 을 한다.

1. 우선 24비트 버퍼에 위쪽(MSB)부터 한 byte씩 3 byte의 문자를 집어넣는다.

2. 버퍼의 위쪽부터 6비트씩 잘라 그 값을 읽고, 각각의 값을 아래 [표-1] 의 문자로 Encoding 한다.

![image](https://user-images.githubusercontent.com/79297596/128028641-90023dba-9083-4e23-bc16-722680113efe.png)

입력으로 Base64 Encoding 된 String 이 주어졌을 때, 해당 String 을 Decoding 하여, 원문을 출력하는 프로그램을 작성하시오.

-------------------------

# Solution

```
import base64
t = int(input())
for i in range(1,t+1):
    org = input()
    org_base = base64.b64decode(org).decode('utf-8')
    print('#{} {}'.format(i,org_base))
```

---------------------------

https://swexpertacademy.com/main/code/problem/problemDetail.do?contestProbId=AV5PR4DKAG0DFAUq&categoryId=AV5PR4DKAG0DFAUq&categoryType=CODE&problemTitle=Base64&orderBy=FIRST_REG_DATETIME&selectCodeLang=ALL&select-1=&pageSize=10&pageIndex=1
