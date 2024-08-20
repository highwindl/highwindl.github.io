---
layout: post
categories: posts
title: "C언어 기초 5강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: September 20, 2020
---

## C언어 기초 - 05.연산자

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/8ApZesJwCbs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

C언어 연산자에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/master/C%EC%96%B8%EC%96%B4%20%EA%B8%B0%EC%B4%88%205%EA%B0%95)

**과제**
<hr/>

**Q1.**  
아래의 코드는 두 개의 수 x, y를 입력받아 x + y 연산을 출력하는 코드입니다.  
```c++
#include<stdio.h>

int main()
{
	int x, y;

	printf("x, y의 값을 입력하십시오:\n");
	scanf("%d %d", &x, &y);

	printf("입력받은 값 x = %d, y = %d 입니다.\n", x, y);
	printf("%d + %d = %d 입니다.\n", x, y, x + y);

	return 0;
}
```
해당 코드를 이용해 +, -, *, /, %연산을 출력하는 코드를 만들어 봅시다.

<hr/>

**Q2.**  
아래의 코드는 입력받은 값 x, n을 입력받아 출력하는 예제입니다.
```c++
#include<stdio.h>

int main()
{
	int x, n;

	printf("x, n의 값을 입력하십시오:\n");
	scanf("%d %d", &x, &n);

	printf("입력받은 값 x = %d, n = %d 입니다.\n", x, n);

	return 0;
}
```

해당 예제에 이번강의 내용의 비트연산자를 이용해서 x * (2의 n승)을 출력하기 위한 프로그램을 만들어 봅시다.   
출력예시: x = 4, n = 3를 입력할때 결과
->4 * (2의3승) = 64 입니다.
<hr/>


