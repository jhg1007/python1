# python1  
python Learning Repository  

# **ch1 파이썬 문법**  

## 자료형  
#### 숫자형   
* 정수 : 123, -20, 0    
* 실수 : 123.45, -4321.5, 6.08e9     
* 8진수 : 0o456, 0o123   
* 16진수 : 0xFF, 0x0D, 0x0A  

```
a = 10  
b = 20  
c = a + b  
d = b -a  
print(c, d)  
```  

#### 변수 
* 문자 또는 밑줄로 시작( beta, _kim)  
* 대소문자를 구분. (sum, Sum, SUM)  
* 영문자,숫자,밑줄(A-z,0-9,_)  
* 파이썬 키워드는 사용 불가  

```
a = 10  
b = 3  
#나눗셈  
c = a/b #나눗셈  
d = a//b #몫  
e = a%b # 나머지  
#곱셈  
f = a*b   
g = a**b  # 제곱  
print(c,d,e,f,g)  
```

#### 문자열  
* 1. 큰 따옴표 : "Hello world!"  
* 2. 작은 따옴표 : '대한민국'  
* 3. 큰따옴표 3 : """Hello!"""  
* 4. 작은 따옴표3 : '''Life id too short. you need python'''  

```
myName = "Lang Kim" # 나멜  
my_name = "김랑기" # 스네이크  
Myname = "kiki" # 파스칼  
_my_name = "korea"  
MYNAME = "God is love"  
my2name = "12345"  
# 2myname = "9876"  
# my-name = "michle"  
# my name = "kiki"  
myStr = '123' # str  
myNum = 123 # int  


print(myStr, myNum)  
print(type(myStr))  
print(type(myNum))  
```

#### 여러개 변수 할당  

```
x,y,z = "포도","딸기","수박"  
print(x)  
print(y)  
print(z)  
```

```
a = b = c = "오렌지"  
print(a)  
print(b)  
print(c)  
```

```
fruits = ["포도","딸기","수박"]  
x,y,z = fruits  
print(x)  
print(y)  
print(z)  
```

```
x = "life"  
y = "is"  
z = "Beautiful"  
print(x,y,z)  
print(x+y+z)  
```

```
a = 1  
b = 2  
c = 3  
print(a,b,c,)  
print(a+b+c)  
```

#### 데이터 유형  
+ 텍스트  
+ 숫자  
+ 불(bool)  

```
a = 100  
b = 200  
sum = a + b  
print(a, '+' , b, '=', sum)  
```
#### input() 함수 이용한 계산기  

```
a = int (input( "첫번째 숫자를 입력해 주세요: "))
b = int (input( "두번째 숫자를 입력해 주세요; "))
result = a + b
print(a, '+', b, '=', result)
result = a - b
print(a, '-', b, '=', result)
result = a * b
print(a, '*', b, '=', result)
result = a / b
print(a, '/', b, '=', result)
# 제곱, 몫, 나머지
```

```
num1 = input("숫자입력1")
num2 = input("숫자입력2")
result = num1 + num2
print(type(num1))
print(num1, "+", num2, "=", result)
```

#### 전화번호, 이름, 무게를 입력받아 출력 :  
####입력한 내용은 이름 "00", 전화번호 "00"입니다.  
무게는 입력한 g수 x 10원 = 산출 금액 출력

#### 2. print () 서식 출력

```
print( "%d" % 123)
print( "%5d" % 123)
print( "%05d" % 123)

print( "%f" % 123.45)
print( "%7.1f" % 123.45)
print( "%7.3f" % 123.45)

print( "s" % "대한민국")
print( "6s" % "대한민국")
```

#### format 순서 지정 가능

```
print("{0:d} {1:5d} {2:05d}".format(123.456.789))
```

```
print("{2:d} {1:5d} {0:05d}" .format(123.456.789))
```

### 서식 출력

```
print( "\n줄바꿈\n연습입니다.")
```

```
print("\t탭키\t연습")
```

```
print("글자가 \"강조\"되는 효과1")
print("글자가 \'강조\'되는 효과2")
print("역슬레시 3개출력 \\\\\\")
print(r"\n \t \" \\ \' @를 그래로 출력") #그대로 출력됨
```

#### 관계 연산자

```
a,b = 10,20
print(a==b, a!=b, a>b, a<b, a>=b, a<=b)
```

#### 논리 연산자

```
a = 20
print((a>100) and (a<2000))
print((a>100) or (a<200))
print(not(a==100))
```

```
if(123):
  print("참이연 보입니다.")
if(0):
  print("거지싱면 안 보입니다")
```

### 퀴즈2 숫자 입력을 받아 동전으로 바꿔주는 프로그램( 500원, 100원, 50원, 10원)

```
# 변수
bill, c500, c100, c50, c10 = 0,0,0,0,0
bill = int(input("바꿀돈은?"))

c500 = bill // 500 #  몫
bill %= 500 # bill = bill % 500
c100 = bill // 100
bill %= 100
c10 = bill // 10
bill %= 10

print("500원짜리 %d개" % c500)
print("100원짜리 %d개" % c100)
print("10원짜리 %d개" % c10)
print("잔돈 %d개" % bill)
```

### 조건문

```
a = 50
if(a<100):
  print("100보다 작음")
  print("거짓이면 이문장은 보이지 않음")
print("프로그램 끝")
```

```
a = 2000
if(a<100):
  print("100보다 작다")
else : 
  print("100보다 크다")
print("프로그램 끝")
```

```
# 홀짝 구분
a = int(input("정수를 입력하세요 : "))
if(a % 2 == 0):
  print("짝수")
else :
  print("홀수")
```

```
a = 120
if(a > 50):
  if(a<100):
    print("50<a<100")
  else:
    print("a>100")
else:
  print("a<50")
```

```
fruit = ['사과','배','감','포도']
fruit.append('딸기')
if '딸기' in fruit : # "딸기" not in fruit
  print( "딸기가 있읍니다")
print(fruit)
```

```
import random

number = []
for num in range(0, 6) :
  number.append(random.randrange(1,46))
print("생성된 리스트", number)
```

### 반복문

```
for i in range(0,3,1): # 시작값, 끝값+1,증가값
  print("%d 안녕하세요~" % i) # 반복 내용
  #print(i)
print("반갑습니다^^")
```

```
for i in range(1,9,1):
  print("%d" % i, end=" ")
print("\n")
for i in range(1,9,1):
  print("%d " % i, end="")
```

```
sum=0
i=0
for i in range(1,11,1):
  sum = sum + i
print("1~10까지 합계 : %d" % sum)
```

### 퀴즈3 : 숫자 입력을 받아 1부터 입력된 숫자까지의 합을 for문을 할용하여 출력하시오.

```
sum,num=0,0
num = int(input("숫자입력 : "))
for i in range(1,num+1,1):
  sum = sum + i
print("1~n까지 합계 : %d" % sum)
```

### 중첩 for문

```
i,j,k=0,0,0
k = int(input("구구단 단수 입력 :"))
for i in range(1,10,1):
  print("%d x %d = %2d" % (k,i,k*i))
print("")
```

```
i,j,k=0,0,0
for i in range(2,10,1):
  for i in range(1,10,1):
  print("%d x %d = %2d" % (k,i,k*i))
print("")
```

#### 퀴즈 구구단을 2,3,4,5, 출력 후 줄 바꿔서 출력하시오.

```
m,n=0,0
for m in range(1,10,1):
  for n in range(2,10,1):
    print("%d x %d = %2d \t" % (n,m,m*n), end='')
  print("")
```
