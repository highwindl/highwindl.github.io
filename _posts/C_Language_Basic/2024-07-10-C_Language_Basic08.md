---
layout: post
categories: posts
title: "C언어 기초 8강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: July 10, 2024
---

## C언어 기초 - 08.함수

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/XXDVvkHEjSc?si=6HE7LK_kwQ0bQnPQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</center>

C언어 함수에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/master/C%EC%96%B8%EC%96%B4%20%EA%B8%B0%EC%B4%88%208%EA%B0%95)

**과제**
<hr/>

**Q1.**  
아래의 코드에서 변수 x, y를 입력받아 두 수의 합과 차를 출력하는 sumXY()함수와 subXY()함수를 제작해 봅시다  
```C++
#include<stdio.h>

int sumXY(int x, int y);
int subXY(int x, int y);

int main()
{
	int x, y;
	
	printf("x, y값 입력:");
	scanf("%d %d", &x, &y);
	
	printf("x와 y를 더한값은 %d입니다.\n", sumXY(x, y));
	printf("x에서 y를 뺀 값은 %d입니다.\n", subXY(x, y));  
	
	
	return 0;
}

int sumXY(int x, int y)
{
	//여기에 코드 작성
}

int subXY(int x, int y)
{
	//여기에 코드 작성
}
```

예시)<br>
프로그램 실행후 x에 4 y에 3을 입력할 경우 아래와 같은 결과가 출력됩니다.<br>
x와 y를 더한값은 7입니다.<br>
x에서 y를 뺀 값은 1입니다.

<hr/>

**Q2.**  
아래의 코드에서 변수 n을 입력받아 *를 순차로 출력하는 triangle()함수를 제작해 봅시다.
```C++
#include<stdio.h>

void triangle(int n)
{
	//여기에 코드 작성
}

int main()
{
	int n;

	printf("반복횟수 입력:"); 
	scanf("%d", &n);

	triangle(n);
	
	return 0;
}
```
예시)<br>
5를 입력할 경우 아래와 같은 결과가 나옵니다.<br> 

	*
	**
	***
	****
	*****
<hr/>