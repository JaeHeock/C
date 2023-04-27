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
int main()
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
int main()
{
    double f_temp;
    double c_temp;
    
    printf("화씨온도를 입력하시오");
    scanf("%lf", &f_temp);
    
    c_temp = 5.0 / 9.0 * (f_temp - 32);
    
    printf("섭씨온도는 %f입니다", c_temp);
    
    return 0; }

11. 5주차 예제 #1 - 홀수 짝수

#include <stdio.h>
int main()
{
    int number;
    
    printf("정수를 입력하시오:");
    scanf("%d", &number);
    
    if( number % 2 == 0 )
    printf("입력된 정수는 짝수입니다.\n");
    
    else
    printf("입력된 정수는 홀수입니다.\n");
    return 0; } 

12. 5주차 예제 #2 - 분모 0인지 검사

#include <stdio.h>
int main()
{
    int n, d, result;
    printf("분자와 분모를 입력하시오: ");
    scanf("%d %d", &n, &d);
    if( d == 0 ){
    printf("0으로 나눌 수는 없습니다.\n"); }
    else {
    result = n / d;
    printf("결과는 %d입니다.\n", result); }
    
    return 0; }
    
13. 5주차 예제 #3 - 윤년 판단

#include <stdio.h>
int main()
{
    int year;
    printf("연도를 입력하시오: ");
    scanf("%d", &year);
    if((year % 4 == 0 && year % 100 != 0) || year % 400 == 0){
    printf("%d년은 윤년입니다.\n", year); }
    else{
    printf("%d년은 윤년이 아닙니다.\n", year); }
    return 0; } 
    
14. 5주차 학점 결정 예제

#include <stdio.h>
int main()
{
    int score;
    
    printf("성적을 입력하시오: ");
    scanf("%d", &score);
    
    if (score >= 90){
    printf("합격: 학점A\n");}
    
    else if (score >= 80){
    printf("합격: 학점B\n");}
    
    else if (score >= 70){
    printf("합격: 학점C\n");}
    
    else if (score >= 60){
    printf("합격: 학점D\n");}
    
    else{
    printf("불합격: 학점F\n");}
    
    return 0; } 
    
15. 5주차 Lab : 산술 계산기

#include <stdio.h>
int main()
{
    char op;
    int x, y, result;
    
    printf("수식을 입력하시오(예: 2 + 5) >> ");
    scanf("%d %c %d", &x, &op, &y);
    
    if( op == '+' ){
    result = x + y;}
    
    else if( op == '-' ){
    result = x - y;}
    
    else if( op == '*' ){
    result = x * y;}
    
    else if( op == '/' ){
    result = x / y;}
    
    else if( op == '%' ){
    result = x % y;}
    
    else
    printf("지원되지 않는 연산자입니다. ");
    printf("%d %c %d = %d \n", x, op, y, result);
    return 0; } 
    
16. 5주차 예제 #1 - 달의 일수 계산 프로그램(switch)

#include <stdio.h>
int main()
{
    int month, days;
    
    printf("달을 입력하시오: ");
    scanf("%d", &month);
    switch(month){
    case 2:
        days = 28;
        break;
    case 4:
    case 6:
    case 9:
    case 11:
        days = 30;
        break;
    default:
        days = 31;
        break;
                }
    
    printf("%d월의 일수는 %d입니다.\n", month, days);
    
    return 0;}
    
17. 5주차 mini project: 소득세 계산기 만들기

#include <stdio.h>
int main()
{
    double tax_base, tax, deduction, cal_tax;
    
    tax_base = 35000000
    tax = tax_base * 15%;
    deduction = 1080000;
    cal_tax = tax - deduction;
    
    printf("과세 표준: %lf", tax_base);
    printf("소득세율: 15%");
    printf("(공제전)소득세: %lf"),tax);
    printf("누진공제액 : %lf", deduction);
    printf("산출세액 : %lf", cal_tax);
    
    return 0; }

18. 6주차 예제 #1 - while문을 이용한 구구단 출력 프로그램

#include <stdio.h>
int main()
{
    int n;
    int i = 1;
    
    printf("출력하고 싶은 단: ");
    scanf("%d", &n);
    
    while (i <= 9){
    printf("%d*%d = %d \n", n, i, n*i);
    i++;}
    
    return 0; }
    
19. 6주차 예제 #2 - while문을 이용한 제곱값 출력 프로그램

#include <stdio.h>
int main()
{
    int n;
    
    printf("====================\n");
    printf("  n    n의 제곱 \n");
    printf("====================\n");
    
    n=1;
    while ( n<=10 ){
    printf("%5d    %5d",n, n*n);
    n++;
    
    return 0; }
    
20. 6주차 예제 #3 - 1부터 n까지의 합 계산하는 프로그램

#include <stdio.h>
int main()
{
    int i,n,sum;
    
    printf("정수를 입력하시오:");
    scanf_s("%d", &n);
    i = 1;
    sum = 0;
    while(i <= n){
    sum += i;
    i++; }
    printf("1부터 %d까지의 합은 %d입니다\n", n, sum);
    return 0; }
    
21. 6주차 예제 #4 - n 이하의 모든 짝수의 합 구하기

#include <stdio.h>
int main()
{
    int i, n, sum;
    
    printf("정수를 입력하시오:");
    scanf_s("%d", &n);
    
    i = 0;
    sum = 0;
    
    while(i <= n){
    sum += i;
    i = i + 2; }
    
    printf("1부터 %d까지의 짝수합은 %d입니다\n", n, sum);
    return 0; }
    
22. 6주차 예제 #5 - while문을 이용한 합계 프로그램

#include <stdio.h>
int main()
{
    int i, n, sum;
    
    i = 0;
    sum = 0;
    while (i<5){
    printf("값을 입력하시오: ");
    scanf("%d", &n);
    sum = sum + n ;
    i++;}
    
    printf("합계는 %d입니다.\n",sum);
    
    return 0; }
    
    
