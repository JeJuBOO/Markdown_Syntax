---
layout: post
title:  "Markdown Syntax"
---

첫번째 포스팅은 앞으로 꾸준히 블로그를 작성하기 위한 Markdown Syntax에 대해 정리해 둘 것이다.<br><br>


# Markdown Syntax 정리
마크다운(Markdown)은 마크업 언어의 하나의 종류이다.\
마크다운은 읽고 쓰기 쉽도록 설계되었고 무엇보다 가독성을 강조했다.

블로그를 작성하기 위해 필요한 마크다운 문법을 업로드 할 것이다.

### Table of Contents
[0. Paragraphs and Line breaks](#0-paragraphs-and-line-breaks)  
[1. Headers](#1-headers)  
[2. Blockquotes](#2-blockquotes)  
[3. List](#3-list)  
[4. Code Blocks](#4-code-blocks)  
[5. Horizontal Rules](#5-horizontal-rules)  
[6. Links](#6-links)  
[7. Emphasis](#7-emphasis)  
[8. Images](#8-images)  
[9. Backslash Escapes](#9-backslash-escapes)  
[10. 수식 작성 LaTax](#10-수식-작성-latax)
<br><br><br>

---
## 0. Paragraphs and Line breaks
* 문단의 구분은 하나이상의 빈 줄
* 줄을 바꾸기 위해서는 `스페이스 두번 + 엔터`을 사용한다.
* HTML의 태그인 <br>은 엔터의 기능을 한다.

**markdown syntax**
```
문단을 구분하기 위해서는 다음과 같이 한다.

줄바꿈을 위해서는 다음과 같이 한다. 줄바꿈을  
위해서는 다음과 같이 한다.

줄바꿈을 위해서는 다음과 같이 한다. 줄바꿈을 <br>
위해서는 다음과 같이 한다.
```
**result**

문단을 구분하기 위해서는 다음과 같이 한다.

줄바꿈을 위해서는 다음과 같이 한다. 줄바꿈을  
위해서는 다음과 같이 한다.

줄바꿈을 위해서는 다음과 같이 한다. 줄바꿈을 <br>
위해서는 다음과 같이 한다.


<br><br><br>

---
## 1. Headers
* 문단을 크게 나누기 위해 사용된다.
* `#`을 이용하여 사용된다.
* `#`가 많아질수록 소문단으로 사용되며 6개까지 가능하다.
* 작성한 제목 아래에 `===`은 `#`와 같은 역할을 하고, `---`은 `##`와 같다.

**markdown syntax**
```
# H1 가장 큰 제목
## H2 두번째로 큰 제목
### H3 세번째이고 이후로 여섯개까지 가능

H1 아래에 `===`로 제목 가능
===
H2 또한 `---`로 가능
---
```
**result** 

# H1 가장 큰 제목
## H2 두번째로 큰 제목
### H3 세번째이고 이후로 여섯개까지 가능

H1 아래에 `===`로 제목 가능
===
H2 이또한 `---`로 가능
---
<br><br><br>

---
## 2. Blockquotes
* 블록 인용은 문장앞에 `>`을 이용한다.
* 인용문 안에 인용문은 `>>`을 이용하고 3개까지 가능하다.
* 모든 줄 앞에 `>`을 넣으면 가장 보기가 좋다.
* 단락의 첫 줄 앞에만 넣어도 된다.

**markdown syntax**
```
 > 일하는 시간과 노는 시간을 뚜렷이 구분하라. 시간의 중요성을 이해하고 
 > 매순간을 즐겁게 보내고 유용하게 활용하라. 그러면 젋은 날은 유쾌함으로 
 > 가득찰것이고 늙어서도 후회할 일이 적어질것이며 비록 가난할 때라도 
 > 인생을 아름답게 살아갈수있다 – Louisa May Alcott
 
 > 문제는 지적인 기계가 어떤 감정을 가질 수 있느냐가 아니라, 기계가 
   아무런 감정 없이 지능을 가질 수 있느냐 하는 것이다. 
 > > - Marvin Lee Minsky
 
```
**result**
> 일하는 시간과 노는 시간을 뚜렷이 구분하라. 시간의 중요성을 이해하고 
> 매순간을 즐겁게 보내고 유용하게 활용하라. 그러면 젋은 날은 유쾌함으로 
> 가득찰것이고 늙어서도 후회할 일이 적어질것이며 비록 가난할 때라도 
> 인생을 아름답게 살아갈수있다 – Louisa May Alcott

> 문제는 지적인 기계가 어떤 감정을 가질 수 있느냐가 아니라, 기계가 
  아무런 감정 없이 지능을 가질 수 있느냐 하는 것이다. 
> > - Marvin Lee Minsky

<br><br><br>

---
## 3. List
* 숫자가 없는 목록(Unordered lists)은 `*`, `-`, `+`을 이용한다.
* 숫자로 표현된 목록(Ordered lists)은 `1.`숫자 다음 마침표로 이용한다.
* 들여쓰기(띄어쓰기 3번)를 이용해 모양을 바꿀 수 있다.

**markdown syntax**
```
* Red
   * dark red
      * darkdark red
- Blue
+ Green

1. 색깔
   1. 빨강
   2. 노랑
2. 동물
   1. 강아지
   3. 고양이 
```
**result**

* Red
   * dark red
      * darkdark red
- Blue
+ Green

1. 색깔
   1. 빨강
   2. 노랑
2. 동물
   1. 강아지
   3. 고양이 
<br><br><br>

---
## 4. Code Blocks
* 간단한 한줄의 코드를 나타내려면 역따옴표 `` ` ``을 사용한다.
* 코드 블록의 경우는 각 줄에 띄어쓰기 4개를 사용한다.
* 또는 코드 블록의 시작과 끝에  ```` ``` ````을 사용한다.
* 위와 같이 역따옴표를 표시하기 위해서는 표시할 역따옴표 
  개수보다 많은 수의 역따옴표로 묶어준다. 
* 다양한 언어를 역따옴표 뒤에 적으면 문법을 강조할 수 있다.

**markdown syntax**
````
    앞의 4개의 공백은 표시되지 않는다.
        또한 코드블럭 전 한줄을 띄어야 한다.
    각각 띄어쓰기 하기보다 작성 후에 드래그하고 탭을 눌러 보세요.
```
역따옴표 3개를 위 아래로 배치
```

```python
def print_text():
    print("Hello Wolrd!!")
```
```` 

**result**

    앞의 4개의 공백은 표시되지 않는다.
        또한 코드블럭 전 한줄을 띄어야 한다.
    각각 띄어쓰기 하기보다 작성 후에 드래그하고 탭을 눌러 보세요.
```
역따옴표 3개를 위 아래로 배치
```

```python
def print_text():
    print("Hello Wolrd!!")
```
<br><br><br>

---
## 5. Horizontal Rules
* 아래의 문법들로 똑같은 수평선을 만들 수 있다.

**markdown syntax**
```
* * *

***

*****

- - -

----------------------------

```
**result**

* * *

***

*****

- - -

----------------------------

<br><br><br>

---
## 6. Links
* 링크의 텍스트는 [대괄호]로 구분한다.
* 링크 삽입 : 대괄호 뒤로 (중괄호)안에 링크를 삽입한다.
* id룰 통한 링크 삽입 : 또한 대괄호 뒤로 [id]을 적고 문서의 아무 곳에서 링크 레이블을 정의
* 내부 링크 : 내부의 텍스트를 따라 이동하는 링크를 만들 수 있다.
   * 내부의 텍스트는 유일해야 한다.(여러개일 경우 가장 근접한 텍스트 이용)
   * 목차명에 점, 반점, 특수문자, 괄호는 무시한다.
   * `#`로 제목 처리된 곳으로 이동, 이동할 `#`의 개수는 상관없이 하나만 작성한다.


**markdown syntax**
```
[Google](http://www.google.com "구글") \
[Naver](http://www.naver.com "네이버") \
구글 www.google.com; 꺽쇠없음 \
네이버 <www.naver.com>; 꺽쇠있음 \
유튜브 <youtube.com>

[Google][1]을 누르면 페이지로 이동합니다. \
[네이버][2]를 누르면 이동합니다.

[1]: http://www.google.com
[2]: http://www.naver.com

[보여지는 내용](#이동할-텍스트) \
괄호 안에 텍스트의 띄어쓰기는 `-`로 연결하고, 영어는 소문자로 작성한다.

[6. Links](#6-links)
[맨 위로 이동](#)
```
**result**

[Google](http://www.google.com "구글") \
[Naver](http://www.naver.com "네이버") \
구글 www.google.com; 꺽쇠없음 \
네이버 <www.naver.com>; 꺽쇠있음 \
유튜브 <youtube.com>

[Google][1]을 누르면 페이지로 이동합니다. \
[네이버][2]를 누르면 이동합니다.

[1]: http://www.google.com
[2]: http://www.naver.com

[보여지는 내용](#이동할-텍스트) \
괄호 안에 텍스트의 띄어쓰기는 `-`로 연결하고, 영어는 소문자로 작성한다.

[6. Links](#6-links) \
[목차](#table-of-contents)

<br><br><br>

---
## 7. Emphasis
* 굵게(Bold), 기울임꼴(Italic), 취소선(Strikethrough) 세가지 강조 문법이 있다.
* Bold : `**`, `__`
* Italic : `*`, `_`
* Strikethrough : `~~`

**markdown syntax**
```
굵게 하고 싶을때는 양쪽에 `**`나 `__`을 넣기 \
**굵게** \
__굵게__

기울임꼴은 양쪽에 `*`나 `_`을 넣기 \
*기울임꼴* \
_기울임꼴_

취소선은 양쪽에 `~~`을 넣기 \
~~취소선~~

***굵은 기울임*** \
___굵은 기울임___

**~~굵은 취소선~~**
```
**result**

굵게 하고 싶을때는 양쪽에 `**`나 `__`을 넣기\
**굵게**\
__굵게__

기울임꼴은 양쪽에 `*`나 `_`을 넣기 \
*기울임꼴* \
_기울임꼴_

취소선은 양쪽에 `~~`을 넣기 \
~~취소선~~

***굵은 기울임*** \
___굵은 기울임___

**~~굵은 취소선~~**
<br><br><br>

---
## 8. Images
* 링크와 비슷하지만 앞에 `!`가 븥는다.
* 인라인 이미지 `![alt text](/path/to/img.jpg)`
* 링크 이미지 `![alt text](/path/to/img.jpg "Optional title")`

**markdown syntax**
```
![alt pooh](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQW0Z94iqO01RBz7uaesVFC5hG-J4y-ldNCHg&usqp=CAU)

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQW0Z94iqO01RBz7uaesVFC5hG-J4y-ldNCHg&usqp=CAU" width="100">
```
**result**

![alt pooh](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQW0Z94iqO01RBz7uaesVFC5hG-J4y-ldNCHg&usqp=CAU)

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQW0Z94iqO01RBz7uaesVFC5hG-J4y-ldNCHg&usqp=CAU" width="50%">

<br><br><br>

---
## 9. Backslash Escapes
* 특수문자를 표현하고 싶을때 이용한다.
* 표시할 특수문자 앞에 `\`를 쓴다.

**markdown syntax**
```
\\   backslash \
\`   backtick \
\*   asterisk \
\_   underscore \
\{\}  curly braces \
\[\]  square brackets \
\(\)  parentheses \
\#   hash mark \
\+   plus sign \
\-   minus sign (hyphen) \
\.   dot \
\!   exclamation mark
\$   dollar sign
```
**result**

\\   backslash \
\`   backtick \
\*   asterisk \
\_   underscore \
\{\}  curly braces \
\[\]  square brackets \
\(\)  parentheses \
\#   hash mark \
\+   plus sign \
\-   minus sign (hyphen) \
\.   dot \
\!   exclamation mark
\$   dollar sign

이것으로 [Markdown Syntax][daring fireball] 홈페이지의 설명된 목차를 정리했다.<br>
추가로 필요한 문법은 작성 할 것이다.

## 10. 수식 작성 LaTaX
* 텍스트 사이에 `$`로 수식의 앞 뒤를 감싸 수식을 표현한다.(`$ x $` 띄어 쓰면 인식이 안됨.)
* `$$`을 이용하면 수식을 블록으로 중앙 정렬할 수 있다.
* Github markdown에서 LaTaX 형식을 지원한다.
* 따라서 [LaTaX문법][wiki latax math]을 알아 봐야겠다.
* 수식 내에서 중괄호를 쓰기 위해 `\\{` 다음과 같이 작성

[wiki latax math]: https://en.wikibooks.org/wiki/LaTeX/Mathematics

**markdown syntax**
```
$y = x+1$
$x$가 $4$일때 $y$는 $5$이다.

$$
y = 3x^2 + x + 1
$$
```
**result**

$y = x+1$  
$x$가 $4$일때 $y$는 $5$이다.

$$
y = 3x^2 + x + 1
$$
