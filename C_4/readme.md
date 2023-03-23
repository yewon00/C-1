# 4주차 C언어 실습
 - 4주차 복습
   
   https://codingadinga.tistory.com/11 <br>
   ++i : 선위연산자 : 증가
   
 - 4주차 실습

```
#include <stdio.h>

int main() {
    
    double x, y, result;

    printf ("두 개의 실수를 입력하시오: ");
    scanf("%lf %lf" &x, &y);

    result = x + y;
    printf("%f / %f = %f", x, y, result);

    result = x / y;
    printf("%f / %f = %f", x, y, result);

return 0;
}
```

```

#include <stdio.h>

int main(void)
{
    int x=10, y=10;

    printf("x=%d\n",x);
    printf("++x의 값=%d\n", ++x);
    printf("x=%d\n\n", x);

    printf("x=%d\n",y);
    printf("y++의 값=%d\n", y++);
    printf("y=%d\n\n", y);


    return 0;
}

```
