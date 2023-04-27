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
    
    ---------------------------------------
    
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
