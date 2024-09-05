---
layout: post
categories: posts
title: "C언어 심화 11강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: Sep 05, 2024
---

## C언어 심화 - 11.포인터

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/pVWnrYr1de0?si=z_L9howc8fOhyala" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</center>

C언어 포인터에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/master/C%EC%96%B8%EC%96%B4%20%EC%8B%AC%ED%99%94%2011%EA%B0%95)

**과제**
<hr/>

아래의 코드는 int형 변수 a에 저장된 값을 포인터 변수 p를 이용해 불러오는 코드입니다.
```c++
#include<stdio.h>

int main()
{
	int *p;
	int a = 3;
	
	p = &a;
	
	printf("a의 주소값: %d\n", p);
	printf("a의 주소에 저장된 값: %d\n", *p);
	
	return 0;
}
```

**Q1.**  
위의 코드를 실행해보고 결과를 확인해 보고 왜 그런지 생각해 봅시다.

**Q2.**  
위의 코드에서 마지막 prtinf함수 아래에 *p=15라는 값을 저장후 변수 a의 값을 출력해 봅시다.
<br>
<br>
<br>
아래의 코드는 10개의 배열변수를 포인터를 이용해 출력하는 예제 입니다.

```c++
#include<stdio.h>


int main()
{
	int *p;
	int i; 
	int a[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
	
	p = a;
	
	for(i = 0; i < 10; i++)
	{
		printf("p + %d에 저장된 주소값: %d\n", i, p + i);
		printf("p + %d의 주소에 저장된 값: %d\n\n", i, *(p + i));		
	}
	
	return 0;
}
```

**Q3.**  
위의 코드를 실행해보고 결과를 확인해 보고 왜 그런지 생각해 봅시다.

**Q4.**  
위의 코드에서 int변수 a와 int 포인터 변수 p를 char형으로 변경후 결과를 비교해 봅시다.

**Q5.**  
Q4의 내용처럼 변수를 float, double등으로 바꿔보고 결과를 확인해 봅시다.


<hr/>