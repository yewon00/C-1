# C언어 7주차

- C언어 7주차 실습

https://www.acmicpc.net/problem/10952 << 문제

```
#include <stdio.h>

int main() {
    int a, b;
    scanf("%d %d", &a, &b);
    printf("%d\n", a + b);
    return 0;
}
```

ㄴ 문제 답 : 위 코드에서 scanf() 함수를 통해 두 정수 A와 B를 입력받고, printf() 함수를 이용하여 A+B의 결과를 출력합니다.<br> 
             코드의 마지막으로 return 0;을 통해 프로그램이 정상적으로 종료되었음을 알립니다.
 
```
#include <stdio.h>

int add(int a, int b); // a + b 값을 반환해줌

int a = 10;

int main() {
  int result = add(a, 5);
  printf("%d\n", result);
  return 0;
}

int add(int a, int b) 
{ 
  a = 20;
  return a + b; 
}
```
→정답 ![image](https://user-images.githubusercontent.com/128660870/231633061-3be56c68-7f07-4a39-836a-c53f1c451de6.png)


```
#include <stdio.h>

void print_stars() 
{
  for (int i = 0; i < 30; i++)
      printf("*");
}

int main(void)
{
  print_stars();
  printf("\nHello World!\n");
  
  print_stars();
  printf("\n");

  return 0;
}
```
→결과 ![image](https://user-images.githubusercontent.com/128660870/231632504-fdbaf824-9231-4508-95c0-d8612868dfbb.png)
