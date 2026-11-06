---
layout: post
title: 마크다운 연습 겸 포스팅 연습
subtitle: 
categories: markdown
tags: [test]
---

## 강조 emphasis
기울이기  : \*글자\* or \_글자\_ -> _글자_\
굵게  : \*\*글자\*\* or \_\_글자\_\_ -> __글자__\
\* 앞에 \를 넣으면 \*만 표시 가능\

## 문단 줄바꿈 paragraph
문단 : 문장 사이에 enter x 2 -> 문단 나누기\
줄바꿈 : 문장 끝에 \ 추가 하고 enter x 1 -> 줄바꾸기

## 헤딩 heading
글자 앞에 \#를 붙이면 됨. 6단계까지 존재. (secondary heading부터 toc로 들어감.)

## 인용문 blockquote
\> 를 문장 앞에 넣으면 인용. 인용문 사이에 > 빈칸 넣으면 두 문장을 한꺼번에 인용

> "Boys, be ambitious!" -William S. Clark-

> "꿈은 없고요. 그냥 놀고 싶습니다."
>
> "티끌 모아 티끌" -박명수-

## 리스트 list
순서 없는 리스트 unordered list : \- 글자 or \* 글자 or \+ 글자\
순서 있는 리스트 ordered list : 1/. 글자\
들여쓰는 리스트 nested list : 띄어쓰기 x 3~4 + 리스트 (글자, 인용문도 들여쓸 수 있음)\
&ensp;※리스트의 종류를 섞어쓰면 구별이 되어버림
체크박스 리스트 checklist : \- [ ] or \- [x] (\*, \+도 가능)
- 리스트1
    1. 들여쓰기 리스트1
- 리스트2
    1. 들여쓰기 리스트2
    2. 들여쓰기 리스트3
- [ ] 독서하기
- [x] 운동하기

## 링크 link

\<주소> <https://wsdominance.github.io/blog>\
\[이름]\(주소) [blog](https://wsdominance.github.io/blog)\
한 문단 안에서 \[이름1][1]...\[이름2][2]...\[이름1][1]... 문단 다음줄에 \[1]:주소1 ...

처음 페이지는 [HOME][1] 아카이브는 [ARCHIVES][2] 작성자에 대한 건 [ABOUT][3] 이름을 바꿔도 처음으로 [HOME2][1]. 감사합니다.

[1]:https://wsdominance.github.io/blog
[2]:https://wsdominance.github.io/blog/archives
[3]:https://wsdominance.github.io/blog/about

## 사진 image

\!\[alt_text](사진_경로)

## 코드블록 code

## 표 table



테이블을 만들 때는 | 로 구분하면 알아서 됨\
:-----로 된 행을 넣어서 머리와 구분

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |

코드청크를 넣을 때는 코드 윗줄 아랫줄에 ~~~을 넣으면 된다

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
