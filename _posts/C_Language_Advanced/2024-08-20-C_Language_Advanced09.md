---
layout: post
categories: posts
title: "C언어 기초 9강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: Aug 20, 2024
---

## C언어 기초 - 08.함수

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/veT-mtaDbI4?si=SL_WQ3nJz6YyTXSp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</center>

C언어 전역변수와 지역변수에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/master/C%EC%96%B8%EC%96%B4%20%EC%8B%AC%ED%99%94%209%EA%B0%95)

**과제**
<hr/>

아래의 코드는 1~100까지의 합을 구하는 프로그램입니다.
```C++
#include<stdio.h>

int accX(int x)
{
	int returnValue = 0;
	returnValue += x;
	
	return returnValue;
}

int main()
{
	int i, y;
	
	for(i = 1; i <= 100; i++)
	{
		y = accX(i);
	}
	
	printf("1~100의 합: %d", y);
	
	return 0;
}
```
1~100까지의 합은 5050 입니다.<br/>

**Q1.**  
위의 코드를 실행해보고 실제로 5050이 나오는지 확인해 봅시다.

**Q2.**  
위의 코드가 5050이 나오지 않는다면 그 이유를 확인해 봅시다.

**Q3.**  
위의 코드의 accX 함수의 returnValue를 static int형으로 변경하고 결과를 확인해 봅시다.

**Q4.**  
위의 코드의 accX 함수의 returnValue를 전역변수로 변경후 결과를 확인해 봅시다.

<hr/>