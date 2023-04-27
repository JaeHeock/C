# 0427 C프로그래밍

1. 2주차 교안 84페이지(사칙 연산)

#include <stdio.h>
int main()
{
    int x, y;
    int sum, diff, mul, div;
    
    x = 20;
    y = 10;
    
    sum = x + y;
    diff = x - y;
    mul = x * y;
    div = x / y;
    
    printf("두 수의 합: %d\n", sum)
    printf("두 수의 차: %d\n", diff)
    printf("두 수의 곱: %d\n", mul)
    printf("두 수의 몫: %d\n", div)
    
    return 0; }
    
2. 2주차 교안 97페이지(덧셈 프로그램)

#include <stdio.h>
int main()
{
    int x, y, sum;
    
    printf("첫번째 숫자를 입력하시오:");
    scanf_s("%d", &x);
    
    printf("두번째 숫자를 입력하시오:");
    scanf_s("%d", &y);
    
    sum = x + y;
    
    printf("두 수의 합: %d", sum);
    
    return 0; }

3. 2주차 교안 99페이지(원의 면적 계산 프로그램)

#include <stdio.h>
int main()
{
    float radius, area;
    printf("반지름을 입력하시오:");
    scanf_s("%f", &radius);
    
    area = 3.14 * radius * radius;
    
    printf("원의 면적: %f", area);
    
    return 0; }
    
4. 2주차 교안 101페이지(환율 계산 프로그램)

#include <stdio.h>
int main()
{
    double rate;
    double usd;
    int krw;
    
    printf("환율을 입력하시오: ");
    scanf_s("%lf", &rate);
    printf("원화 금액을 입력하시오: ");
    scanf("%d", &krw);
    
    usd = krw / rate;
    printf("원화 %d 원은 %lf 달러입니다.", krw, usd);
    return 0; }
    
5. 2주차 교안 103페이지(평균 계산하기 프로그램)

#include <stdio.h>
int main()
{
    double x, y , z;
    double sum, avg;
    
    printf("3개의 실수를 입력하시오: ");
    scanf_s("%lf %lf %lf", &num1, &num2, &num3);
    
    sum = num1 + num2 + num3;
    avg = sum / 3.0;
    printf("합계=%.2lf\n", sum);
    printf("평균=%.2lf\n", avg);
    
    return 0; }
    
6. 2주차 mini project 사각형의 둘레와 면적

#include <stdio.h>
int main()
{
    double w, h, area, perimeter;
    
    printf("사각형의 가로 길이를 입력하시오: ");
    scanf_s("%lf", &w);
    printf("사각형의 세로 길이를 입력하시오: ");
    scanf_s("%lf", &h);
    
    area = w * h;
    perimeter = 2 * (w+h);
    
    printf("사각형의 넓이: %lf\n", area);
    printf("사각형의 둘레: %lf\n", perimeter);
