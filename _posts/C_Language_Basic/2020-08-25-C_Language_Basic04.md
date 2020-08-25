---
layout: post
categories: posts
title: "C언어 기초 4강"
tags: [C, C언어, C언어 강의, C언어 강좌, DEV C++]
date-string: AUGUST 25, 2020
---

## C언어 기초 - 04.변수

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/6MLP2YdPq30" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

C언어 변수에 대한 설명입니다.

[<u>과제 정답 링크 입니다.</u>](https://github.com/highwindl/homework/tree/master/C%EC%96%B8%EC%96%B4%20%EA%B8%B0%EC%B4%88%204%EA%B0%95)

**과제**
<hr/>

아래의 링크는 영상에 나온 프로그램 코드 입니다. 

[<u>프로그램 코드 링크</u>](https://github.com/highwindl/homework/blob/master/C%EC%96%B8%EC%96%B4%20%EA%B8%B0%EC%B4%88%204%EA%B0%95/homework4-1.c)

<hr/>

**Q1.**  
해당 코드를 실행해 보고 왜 이런 결과가 나오는지 생각 해 봅시다.  
<hr/>

**Q2.**  
DEV C++에서 해당 코드의 6번째 줄은 다음과 같습니다.  

	char c = 'a';  

이 코드의 아랫줄에 다음과 같은 코드를 한줄 추가하고, 결과를 확인해 봅시다.  

	printf("int=%d, char=%c\n", a, c);  
<hr/>

**Q3.**  
2번문항에 추가된 printf함수의 내용을 아래와 같이 고쳐보고, 결과를 확인해 봅시다.  

	printf("int=%d, char=%c\n", a+4, c+2);  
<hr/>

**Q4.**  
변수에 값을 넣을때 16진수의 값을 넣을수 있습니다.  
16진수 값을 넣는 방법은 해당 값의 앞에 0x를 붙여주면됩니다.  
예를들어 16진수 값 1a를 넣을 때는 다음과 같이 넣어줍니다.  

	char c = 0x1a;  

이 내용과 아스키 코드 포스팅을 참고하여 아래 코드의 char 변수c 에 해당하는 값을 16진수로 입력해 봅시다.

	char c = 0x4b; //'K'
	
	printf("%c", c);
	c = 0x6F; //'o'
	printf("%c", c);
	c = ?; //?에 정답 입력('r'에 해당하는 16진수 아스키 코드)
	printf("%c", c);
	c = ?; //?에 정답 입력('e'에 해당하는 16진수 아스키 코드)
	printf("%c", c);
	c = ?; //?에 정답 입력('a'에 해당하는 16진수 아스키 코드)
	printf("%c\n", c);

결과는 다음과 같이 나와야 합니다.  

	Korea
<hr/>

**Q5.**  
아래의 printf문은 Abc12가 출력됩니다.  
	
	printf("%c%c%c%c%c\n", 'A', 'b', 0x63, 0x31, 0x32);

해당 printf를 수정하여 Korea가 나오도록 수정해 봅시다.  
(단, 문자가 입력된 곳은 문자를, 16진수가 입력된 곳은 16진수 아스키 코드를 이용해서 입력)  
<hr/>

**Q6.**  
scanf함수와 printf함수를 입력해서 다음과 같은 프로그램을 작성 해 봅시다.  

	1.int 현 변수 a, b를 생성한다.  
	2.a,b의 값을 키보드로 입력 받는다.  
	3.a,b의 입력 값을 사칙연산으로 출력한다.  

출력예  

	숫자 두 개를 입력하세요: 6 2  
	6 + 2 = 8 입니다.  
	6 - 2 = 4 입니다.  
	6 * 2 = 12 입니다.  
	6 / 2 = 3 입니다.  

**scanf 함수 사용방법**  
printf문은 모니터에 입력한 값을 보여주기 위함 함수입니다.  
이와 반대로 입력을 받기 위한 scanf라는 함수가 존재합니다.  
아래코드는 scanf함수의 사용 예시 입니다.  

	int a;

	printf("숫자를 입력하세요:");
	scanf("%d", &a);
	
	printf("입력된 값은 = %d 입니다.\n", a);

위의 코드는 다음과 같이 실행됩니다.  

	1."숫자를 입력하세요:" 문구가 출력  
	2.scanf함수에서 숫자 입력을 대기  
	3.숫자 입력후 엔터를 입력하면, 입력된 숫자가 출력  
	4.5를 입력할 경우 "입력한 값은 = 5 입니다." 라는 문구가 출력  

scanf의 입력 규칙은 다음과 같습니다.  

	1.""안에는 입력할 변수의 서식 지정자를 넣어 줍니다.  
	2.서식 지정자에 대입하는 변수를 입력합니다.  
	3.이때 주의할 사항은 서식 지정자 대입 변수를 입력 할때 변수앞에 '&'를 반드시 붙여줍니다.  

scanf의 입력값은 다음과 같이 여러개를 입력 할 수도 있습니다.  

	int a;
	char c;

	printf("숫자를 입력하세요:");
	scanf("%d %c", &a, &c);
	
	printf("입력된 값은 = %d %c 입니다.\n", a, c);

여러개의 값을 입력할때는 값 입력 사이에 엔터, 또는 스페이스로 구분합니다.  
위의 코드를 예로 3 과 'c'를 입력할때는  
1.3 입력후 엔터 또는 스페이스
2.'c'입력후 엔터를 입력하면 됩니다.


