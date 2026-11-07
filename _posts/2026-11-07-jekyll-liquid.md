---
layout: post
title: Jekyll Liquid
subtitle: 
categories: Markdown
tags: [Jekyll, Study]
---

## 실행 방지 raw

liquid 코드를 그대로 보여주려면 

```
{% raw %}{%{% endraw %} raw %}
  {보여 주고 싶은 liquid code}
{% raw %}{%{% endraw %} endraw %}
```

{% raw %}
  {보여 주고 싶은 liquid code}
{% endraw %}

## 코드블럭 code

__markdown을 사용한 코드블럭__

> \`\`\`python\
> a = 1\
> b = 2\
> print(a + b)\
> \`\`\`

```python
a = 1
b = 2
print(a + b)
```

__jekyll liquid를 사용한 코드블럭__

{% raw%}
&emsp;{% highlight python %}\
&emsp;a = 1\
&emsp;b = 2\
&emsp;print(a + b)\
&emsp;{% endhighlight %}
{% endraw%}

{% highlight python %}
a = 1
b = 2
print(a + b)
{% endhighlight %}

liquid에서는 코드 줄 개수를 나타낼 수도 있다.

{% raw%}
&emsp;{% highlight python linenos%}\
&emsp;a = 1\
&emsp;b = 2\
&emsp;print(a + b)\
&emsp;{% endhighlight %}
{% endraw%}

{% highlight python linenos%}
a = 1
b = 2
print(a + b)
{% endhighlight %}