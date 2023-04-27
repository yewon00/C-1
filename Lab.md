# LAB 문제

- 2주차 
  
 1) (두 수의 합, 곱, 차, 나누기)
    ```
    #include <stdio.h>

    int main(void) {

      int x;
      int y;
      int sum;

      x = 10;
      y = 20;

      sum = x + y;
      diff = x - y;
      mul = x * y;
      div = x / y;

      printf("두수의 합:%d\n",sum);
      printf("두수의 차:%d\n",diff);
      printf("두수의 곱:%d\n", mul);
      printf("두수의 몫:%d\n", div);

      return 0;
    }
    ```
 
 2) 덧셈 프로그램 

     ```
     첫번째 숫자 입력 : 10
     두번째 숫자 입력 : 20
     두 수의 합 : 30
     ```

     ```
     #include <stdio.h>

          int main(void) {

          int x;
          int y;
          int sum;

          printf("첫번째 숫자를 입력하시오:");
          scanf("%d", &x);

          printf("두번째 숫자를 입력하시오:");
          scanf("%d", &y);

          sum = x + y;
          printf("두수의 합:%d\n", sum);

          return 0;
         }
       ```
 
 3) 원의 면적 계산 프로그램 
 
       ```
       반지름을 입력하시오: 10.0
       원의 면적: 314.000000
       ```
       
       ```
        #include <stdio.h>
        
        int main(void) 
        {
          float radius;
          float area;
          
          printf("원의 반지름을 입력하시오:");
          scanf("%f", &radius);
          
          area = 3.14 * radius * radius
          
          printf("원의면적:%f\n", area);
          
          return 0;
         }
        
        ```
        
 4) 환율 계산 프로그램
   
     ```
     환율을 입력하시오 : 1400
     원화 금액을 입력하시오 : 1000000
     원화 1000000원은 714.285714달러입니다.
     ```

     ```
     #include <stdio.h>

      int main(void) 
      {
        double rate;
        double usd;
        int krw;

        printf("환율을 입력하시오:");
        scanf("%lf", &rate);

        printf("원화 금액을 입력하시오:");
        scanf("%d", &krw);

        usd = krw / rate;

        printf("원화 %d원은 %lf달러입니다.\n", krw, usd);

        return 0;
       }
      ```
    
 
  5) 평균 계산 프로그램
    
      ```
      3개의 실수를  입력하시오 : 10.2 21.5 32.9
      합계 = 64.60
      평균 = 21.53

      ```

      ```
      #include <stdio.h>

      int main(void)
      {
        double num1, num2, num3;
        double sum, avg;

        printf("3개의 실수를 입력하시오:");
        scanf("%lf", "%lf", "%lf", &num1, &num2, &num3);

        sum = num1 + num2 + num3;
        avg = sum / 3.0;

        printf("합계=%.2lf\n", sum);
        printf("평균=%.2lf\n", avg);

        return 0;
      }
       ```
    
   6) 사각형의 둘레와 면적
    
      ```
      필요한 변수는 w, h, area, perimeter
      변수의 자료형은 실수를 저장할 수 있는 double형
      area = w*h;
      perimeter = 2*(W+h)
      ```

      ```
      #include <stdio.h>

        int main(void)
        {
          double w, h, area, perimeter;

          w = 10.0;
          h = 5.0;
          area = w * h;
          perimeter = 2 * (w + h);

          printf("사각형의 넓이:%lf\n", area);
          printf("사각형의 넓이:%lf\n", perimeter);

          return 0;
        }
        ```
        
        
- 3주차
  
  1) 예제
  
  ```
  #include <stdio.h>
    int main(void)
    {
      float x = 1.234567890123456789;
      double y = 1.2345678901234567890;
      
      printf("float의 크기=%d)\n", sizeof(float)); 
      printf("double의 크기=%d\n", sizeof(double)); 
      
      printf("x = %30.25f\n",x); 
      printf("y = %30.25f\n",y);
      
      return 0;
      }
      ```
      
        
    
    
