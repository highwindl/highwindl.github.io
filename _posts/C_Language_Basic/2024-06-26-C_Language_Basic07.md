---
layout: post
categories: posts
title: "C언어 기초 7강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: June 26, 2024
---

## C언어 기초 - 07.반복문

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/k8tkaF1g59I?si=ZeHFeq4Kyi0sC1wy" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

C언어 반복문에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/880e36ff746a8eb9872731aa679fe93818eec363/C%EC%96%B8%EC%96%B4%20%EA%B8%B0%EC%B4%88%207%EA%B0%95)

**과제**
<hr/>

**Q1.**  
아래의 코드는 한 개의 수 n을 입력받아 1부터 n까지의 합을 출력하는 코드입니다.  
```c++
#include <stdio.h>

int main()
{
	int n, result;
	int i;

	result = 0;

	printf("반복횟수 입력:"); 
	scanf("%d", &n);

	for(i = 1; i <= n; i++)
	{        
		result += i;
	}
	printf("입력받은 값은 %d이며, 1부터 %d까지 더한값은 %d 입니다.\n", n, n, result); 

	return 0;
}
```

해당 코드에 if문을 응용해 짝수는 더하지 않도록 프로그램을 수정해 봅시다  
예시)<br>
프로그램 실행후 4를 입력할 경우<br>
기존결과: 1+2+3+4 = 10<br>
수정된결과: 1+3 = 4

<hr/>

**Q2.**  
아래의 코드는 입력받은 값 n에따라 *를 순차로 출력하는 예제입니다.
```c++
#include<stdio.h>

int main()
{
	int n;
	int i, j;

	printf("반복횟수 입력:"); 
	scanf("%d", &n);
	
	for(i = 1; i <= n; i++)
	{
		for(j = 0; j < i; j++)
		{
			printf("*");
		}      
		printf("\n");
	}
}
```
예시)<br>
5를 입력할 경우 아래와 같은 결과가 나옵니다.<br> 

	*
	**
	***
	****
	*****

위 코드를 분석한후, 입력받은값에 따라 아래와 같은 결과를 나타내는 프로그램을 만들어 봅시다.<br>
5를 입력할 경우 아래와 같은 결과가 나옵니다.<br>

	    *
	   ***
	  *****
	 *******
	*********

<hr/>

**Q3.**<br>
Q2의 예시에 사용된 for문을 전부 while문으로 변경하여 동일한 결과를 보여주는 프로그램을 만들어 봅시다.<br> 

<hr/>

**Q4.**<br>
Q2의 예시는 두개의 for문이 중첩되어 사용되고 있습니다.<br>
해당 예시와 동일한 결과를 보여주는 프로그램을 for문 1개, if문 1개만 사용하여 만들어 봅시다.

<hr/>