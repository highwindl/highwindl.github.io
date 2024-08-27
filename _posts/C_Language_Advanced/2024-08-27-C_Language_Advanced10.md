---
layout: post
categories: posts
title: "C언어 심화 10강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: Aug 27, 2024
---

## C언어 심화 - 10.배열

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/r9t0fbp68Nk?si=2gkzTqYZsNWdzFDC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</center>

C언어 배열에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/master/C%EC%96%B8%EC%96%B4%20%EC%8B%AC%ED%99%94%2010%EA%B0%95)

**과제**
<hr/>

아래의 코드는 난수를 생성하여 출력하는 프로그램입니다.
```c++
#include<stdio.h>
#include<stdlib.h>
#include<time.h>


int main()
{
	int random = 0;	
	srand(time(NULL)); //난수 생성용 시드값 생성 
	
	random = rand() % 9; //0에서 9사이의 난수 생성
	
	printf("생성된 난수는 %d 입니다.", random); 
	
	return 0;
}
```

**Q1.**  
위의 코드를 실행해보고 매번 실행될 때 마다 값이 다르게 나오는지 확인해 봅시다.

**Q2.**  
위의 코드에서 random 변수를 10개의 배열 random[10]으로 변경후,<br>
10개의 난수를 생성하여 출력하는 프로그램을 만들어 봅시다.

**Q3.**  
Q2의 프로그램을 수정하여 10개의 난수의 합과, 평균, 나머지를 구하는 프로그램을 만들어 봅시다.

<hr/>