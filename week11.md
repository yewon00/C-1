# C언어 11주차

```
#문제2
A 쇼핑몰에서는 회원 등급에 따라 할인 서비스를 제공합니다.
회원 등급에 따른 할인 율은 다음과 같습니다.
(S = 실버, G = 골드, V = vip)

s 등급 = 5%
g 등급 = 10%
v 등급 = 15%
```


```
#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>

int solution (int price, char* grade){
    //write code here
    int answer = 0;
    return answer;
}

//this following is main function to output testcase.
int main(){
    int price1 = 2500;
    char* grade1 = "V";
    int ret1 = solution(price1,grade1);
    
    //Press run button to receive output.
    printf("solution: return value of the function is %d. \n", ret1);
    
    int price2 = 96900;
    char* grade2 ="S";
    int ret2 = solution(price2, grade2);
    
    //Press run button to receive output.
    printf("solution: return value of the function is %d. \n",ret2);
 
}
```

```
solution: return value of the function is 0. 
solution: return value of the function is 0.
```
ㄴ 답 

<hr>


```
#도전문제
1부터 사용자가 입력한 숫자 n 사이의 모든 소수를 찾도록 위의 프로그램을 변경하여 보자
```

```
#include <stdio.h>

int get_integer(void)
{
    int n;
    
    printf("정수를 입력하시오:");
    scanf("%d", &n);
    return n;
}

int is_prime(int n)
{
    int i;
    
    for(i = 2; i < n; i++){
        if (n%i == 0)
            return 0;
    }
    return 1;
}

int main(void)
{
    int n;
    n = get_integer();
    
    if (is_prime(n) == 1)
        printf("%d은 소수입니다.\n", n);
        
    else 
        printf("%d은 소수가 아닙니다.\n", n);
        
    return 0;
}
```
ㄴ 원래 코드 (숫자 입력시, 소수인지 아닌지 알아냄)


<hr>

```
*난수 생성기 p.58
문제)로또 번호 생성기
```
ㄴ 난수도 중복가능성이 多

```
#include <stdlib.h>
#include <stdio.h>
#include <time.h>

#define MAX 45
int main( void )
{
    int i;
    
    srand( (unsigned)time( NULL ) );
    for(i=0; i<6; i++)
        printf("%d\n", 1+rand()%MAX);
    
    return 0;
}
```
ㄴ MAX는 상수로 수정할 수 없다.<br>
ㄴ time 값이 음수가 될 수 없기 때문에 'Unsigned' 필수

<hr>

