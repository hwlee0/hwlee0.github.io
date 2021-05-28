---
layout: single
title: "조건문"
toc: true
toc_sticky: true
toc_label: "조건문 문제풀이 목차"
---

### 01. 사주보기
![saju](/assets/images/사주보기 최종.png)
~~~c
#include <stdio.h>
int main() {
int year, month, day, res;
printf("당신의 사주를 봐드립니다\n 그니까 얼른 연도, 월, 일을 순서대로 입력해봐^^:");
scanf("%d %d %d", &year, &month, &day);
res= (year-month+day)%10;
if(res==0)
printf("축하드려요! 당신은 오늘 아무 일도 일어나지 않아요");
else
printf("아쉽네요ㅠㅠㅠ");
return 0;
}
~~~

### 02. 터널 높이
![tunnel](/assets/images/터널 최종.png)
~~~c
#include <stdio.h>
int main() {
 float a, b, c;
 scanf("%f %f %f", &a, &b, &c);
 if(a<170)
 printf("으악");
 else if(b<170)
 printf("으아악");
else if(c<170)
printf("으아아악");
else
printf("무사통과");
return 0;
}
~~~

### 03. 달력
![callender](/assets/images/달력 최종.png)
~~~c
#include <stdio.h>
int main() {
int y, m;
printf("연도와 달을 입력하시오:");
scanf("%d %d", &y, &m);
 
if(y%4==0){
 if(m==1 || m==3 || m==5 || m==7 || m==8 || m==10 || m==12)
{
 printf("%d년 %d월의 마지막 날은 31일입니다", y, m);
 }
 else if(m==2) {
   printf("%d년 %d월의 마지막 날은 29일입니다", y, m);
 }
   else {
     printf("%d년 %d월의 마지막 날은 30일입니다", y, m);
   }
 }
 
 
else {
 if(m==1 || m==3 || m==5 || m==7 || m==8 || m==10 || m==12) {
   printf("%d년 %d월의 마지막 날은 31일입니다", y, m);
 }
 
 else if(m==2) {
   printf("%d년 %d월의 마지막 날은 28일입니다", y, m);
 }
  else {
    printf("%d년 %d월의 마지막 날은 30일입니다", y, m);
  }
}
}
 ~~~
