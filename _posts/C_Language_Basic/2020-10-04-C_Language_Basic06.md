---
layout: post
categories: posts
title: "C언어 기초 6강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: October 04, 2020
---

## C언어 기초 - 06.분기문

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/Jdi_rzxx0qE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

C언어 연산자에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/master/C%EC%96%B8%EC%96%B4%20%EA%B8%B0%EC%B4%88%206%EA%B0%95)

**과제**
<hr/>

**Q1.**  
아래의 코드는 두 개의 수 a, b를 입력받아 각각의 값을 출력하는 코드입니다.  

	#include<stdio.h>

	int main()
	{
		int a, b;
	
		printf("a,b 입력:");
		scanf("%d %d", &a, &b);
	
		printf("a=%d, b=%d입니다.\n", a, b);	
	
		return 0;	
	}

해당 코드에 if문을 응용해 a와 b를 비교하는 프로그램을 만들어봅시다.  
예시)
1. a>b 이면 "a는 b보다 큽니다."
2. a<b 이면 "a는 b보다 작습니다."
3. a==b 이면 "a와 b는 같습니다."

<hr/>

**Q2.**  
아래의 코드는 입력받은 값 a를 출력하는 예제입니다.

#include<stdio.h>

	int main()
	{
		int a;
	
		printf("a 입력:");
		scanf("%d", &a);
	
		printf("a=%d입니다.\n", a);	
	
		return 0;	
	}


해당 코드에 switch문을 이용해 짝수, 홀수를 판별하는 프로그램을 만들어 봅시다.  
예시)
1. a%b == 1 이면 "홀수입니다."
2. a%b == 0 이면 "짝수입니다."

<hr/>


