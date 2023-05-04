# 9주차 C언어 내용

<h3><b>● 백준 2439번</b></h3>

```
[문제]
첫째 줄에는 별 1개, 둘째 줄에는 별 2개, N번째 줄에는 별 N개를 찍는 문제

하지만, 오른쪽을 기준으로 정렬한 별(예제 참고)을 출력하시오.

[입력]
첫째 줄에 N(1 ≤ N ≤ 100)이 주어진다.

[출력]
첫째 줄부터 N번째 줄까지 차례대로 별을 출력한다.
```

```
#include <stdio.h>

int main() {
    int n;
    printf("별의 개수를 입력하세요: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```
→ 별의 갯수 n에 숫자를 입력하면, n번째줄까지 별이 나옴

<hr>

```
#include <stdio.h>

int main() {
    int n;
    
    for (int i = 1; i <= 5; i++) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```
→ 별의 갯수 5개

<hr>

```
#include <stdio.h>

int main() {
    int n;
    
    for (int i = 4; i >= 0; i--) {
        for (int j = 0; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

```
#include <stdio.h>

int main() {
    int n;
    
    for (int i = 5; i > 0; i--) {
        for (int j = 0; j < i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```
→ for문 첫번째 줄은 자유롭게 수정 가능

```
*****
****
***
**
*
```
→ 결과

<hr>

```
#include <stdio.h>

int main(void) {
    int a=0;
    for(int i=1; i<6; i++) 
    {
        for(int j=1; j<=i; j++) 
        {
          printf("%d", j);
        }
        printf("\n");
    }

    return 0;
}
```

```
1
22
333
4444
55555
```
→ 결과

<hr>

```
#include <stdio.h>

int main(void) {
    
    int a=0;
    int j=0;
    
    for(int i=1; i<=5; i++) 
    {
        for(j=1; j<=5-i; j++) 
        {
          printf(" ");
        }
        for(j=0; j<i; j++)
        {
        printf("*");
        }
        printf("\n");
    }

    return 0;
}
```


![image](https://user-images.githubusercontent.com/128660870/236097526-045efdcf-a4a3-46f9-bb37-9e8c3cdc6e75.png)


→ 결과

<hr>

<h3><b> ● 팩토리얼 함수 </b></h3>

```
#include <stdio.h>

int factorial(int n){
    if(n==0)
        return 1;
    else
        return n*factorial (n-1);
}

int main(){
    int n;
    printf("수를 입력하세요: ");
    scanf("%d", &n);
    printf("%d", factorial(n));
    
    return 0;
}
```

```
n에 4를 입력하면
답 : 24
```
→ 시험문제 출제 가능성 多


