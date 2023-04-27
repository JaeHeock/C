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

7. 3주차 mini project 태양빛 도달 시간

#include <stdio.h>
int main()
{
    double ls, dist, time;
    ls = 300000.0;
    dist = 149600000.0;
    time = dist / ls;
    
    printf("빛의 속도는 %lf\n", ls);
    printf("태양과 지구와의 거리 %lf\n", dist);
    printf("도달 시간은 %lf\n",time);
    
    return 0; }
    
8. 4주차 Lab: 거스름돈 계산하기

#include <stdio.h>
int main(void)
{
    int money, change;
    int price, c5000, c1000, c500, c100;
    
    printf("물건 값을 입력하시오: ");
    scanf("%d", &price);
    
    printf("투입한 금액을 입력하시오: ");
    scanf("%d", &money);
    
    change = money - price;
    c1000 = change / 1000;
    
    change = change % 1000;
    c500 = change / 500;
    change = change % 500;
    c100 = change;
    printf("\n천원권: %d장\n", c1000);
    printf("오백원 동전: %d개\n", c500);
    printf("백원 동전: %d개\n", c100);
    return 0; }
    
9. 4주차 Lab: 윤년

#include <stdio.h>
int main()
{
    int year, result;
    
    printf("연도를 입력하시오: ");
    scanf("%d", &year);
    
    result = ((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0);
    printf("result=%d \n", result);
    
    return 0; }

10. 4주차 mini project: 화씨 온도를 섭씨 온도로 바꾸기

#include <stdio.h>
int main(void)
{
    double f_temp;
    double c_temp;
    
    printf("화씨온도를 입력하시오");
    scanf("%lf", &f_temp);
    
    c_temp = 5.0 / 9.0 * (f_temp - 32);
    
    printf("섭씨온도는 %f입니다", c_temp);
    
    return 0; }


