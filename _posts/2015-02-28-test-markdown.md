---
layout: post
title: 마크다운 연습 겸 포스팅 연습
subtitle: 
categories: markdown
tags: [test]
---

링크는 대괄호로 단어를 묶고 이어서 소괄호로 링크주소
예시[https://naver.com]

볼드체는 **양옆에 별을 두개 넣기**

## secondary heading은 앞에 해시태그를 두개 넣기

테이블을 만들 때는 | 로 구분하면 알아서 됨
:-----로 된 행을 넣어서 머리와 구분

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


사진은 링크를 넣을때 앞에 물음표를 넣으면 된다

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg)

It can also be centered!

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg){: .center-block :}

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
