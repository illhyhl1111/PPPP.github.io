---
title: "고등학교 입학부터 대학교 졸업까지, 수학 압축서"
date: 2018-09-16 16:05:25 -0400
categories: posts
classes: wide
excerpt: "!아직 작성이 완료되지 않았습니다"
header:
  show_overlay_excerpt: true
  overlay_image: /pictures/mathematics.png
  overlay_filter: 0.3
  caption: "Photo credit: [**3Blue1Brown**](https://www.youtube.com/watch?v=mvmuCPvRoWQ&t=1288s)"
author_profile: false
sidebar:
  title: "목차"
  nav: sidebar-math

---

# 들어가기 앞서
[머릿글](https://illhyhl1111.github.io/posts/first-post/)에서 설명했듯이, <br/>
이 글은 읽는이가 해당 내용을 한번쯤은 공부해봤다는 가정 하에, 회고를 위하여 작성한 요약글입니다. <br/>
모르는 부분은 '이런 개념이 있구나' 정도로만 이해하시고, 링크된 글을 읽으시거나 구글링하여 직접 찾아보십시오. <br/>
기본적으로 목차는 **책 기준**으로 분류됩니다. 책 밖에껀 싸그리 기타 항목에 넣을거임ㅎㅎ

아직 작성이 많이많이많이많이매우많이 덜 되었습니다. <br/>
과연 우리의 예비노예는 노예(대학원생)가 되기 전에 초본을 다 쓸 수 있을 것인가

-----------------------------

# 고등학교 수학
2년간 매일같이 쳐다보던 고등학교 수학도 안쓰다보면 결국 까먹는다. 하느님 <br/>
본인이 12년도 고등학교 입학이라 그 당시 교육과정을 따른다. 책이 그거밖에 없음

## 고등수학

### 명제와 조건
명제는 참/거짓을 내릴 수 있는 문장이며, 조건은 변수 $$ x $$에 값을 대입하면 명제가 되는 문장. <br/>
$$p \rightarrow q$$, $$p \Rightarrow q$$,\ $$P \subset Q \Rightarrow (p \Rightarrow q)$$

{% capture context1 %}
#### 조건
조건에 포함된 변수 $$x$$는 $$U \neq \varnothing$$ 을 정의역으로 함. <br/>
전체집합 $$U$$에서의 조건 $$p(x)$$를 간단히 조건 $$p$$라고 표기함. <br/>
$$U$$의 원소 $$a$$를 대입한 $$p(a)$$가 참인 명제라면, 명제 $$p(a)$$가 성립한다, $$a$$는 조건 $$p(x)$$를 만족한다 라고 함.

#### 부정
명제 $$p$$ 혹은 조건 $$p(x)$$에 대해 $$p(x)$$가 아니다 를 $$p(x)$$의 부정이라 하고, $$\sim p(x)$$로 표기함. <br/>
<p> $$ \sim (p \vee q) \Leftrightarrow (\sim p \wedge \sim q), \sim (p \wedge q) \Leftrightarrow (\sim p \vee \sim q) $$ </p>
<p> $$ \sim (\forall x, p(x)) \Leftrightarrow (\exists x, \sim p(x)), \sim (\exists x, p(x)) \Leftrightarrow (\forall x, \sim p(x))$$ </p>

#### 진리집합
$$p(x)$$를 만족하는 $$x$$ 전체의 집합 $$P$$를 조건 $$p(x)$$의 진리집합이라고 한다. <br/>
$$P = \left\{ x | x \in U, p(x) \right\}$$. 표기시 전체집합 $$U$$를 씹으려는 경향이 강하므로 $$P=\left\{ x | p(x) \right\}$$로도 표기.

#### 조건과 집합
집합 $$P$$, $$Q$$를 조건 $$p$$, $$q$$의 진리집합이라고 둘 때, <br/>
<p> $$ P \subset Q \Leftrightarrow (p \Rightarrow q), P \nsubseteq Q \Leftrightarrow (p \nLeftarrow q), \\
p \vee q \Leftrightarrow P \cup Q, p \wedge q \Leftrightarrow P \cup Q, \sim p \Leftrightarrow P^c $$ </p>

#### 필요 · 충분 조건
$$p \Rightarrow q$$일 때, $$p$$는 $$q$$이기 위한 충분조건이고 $$q$$는 $$p$$이기 위한 필요조건이 된다. <br/>
$$p \Leftrightarrow q$$ 면 서로 필요충분조건(동치). <br/>
집합과의 관계는 $$P \subset Q \Rightarrow (p \Rightarrow q) $$임.

#### 귀류법
어떤 명제 $$p \rightarrow q$$임을 증명하려 할 때, 대우 $$\sim q \rightarrow \sim p$$를 증명하는 방법 <br/>
명제의 결론을 부정하여 공리, 정리, 가정 등에 모순이 됨을 이끌어내면 된다.
{% endcapture %}

{% capture context2 %}

* 두 **조건** $$p$$, $$q$$를 $$p \rightarrow q$$ 꼴로 연결하면 명제가 되어버림. <br/>
 '4의 약수는 8의 약수이다' 를 풀어서 '$$x$$가 4의 약수이면 $$x$$는 8의 약수이다' 로 명제와 같이 표현가능.
* $$(P \subset Q) \Rightarrow (x \in P \Rightarrow x \in Q) \Rightarrow (p \Rightarrow q)$$
* $$ \sim (p \vee q) \Rightarrow (P \cup Q)^c \Rightarrow P^c \cup Q^c \Rightarrow \sim p \wedge \sim q $$
* $$ \sim$$ (모든 $$x$$에 대하여 $$p(x)$$이다) $$\Rightarrow \sim (p(x_1) \; and \; p(x_2) \; and \; ... \; and \; p(x_n))$$ <br/>
  $$ \Rightarrow \sim p(x_1) \; or \; \sim \; p(x_2) \; or \; ... \; or \; \sim p(x_n) \Rightarrow$$ 어떤 $$x$$에 대하여 $$\sim p(x) $$ <br/>
  비슷한 방법으로 모두 증명 가능
* 귀류법이 옳다는 것을 증명하는 방법 : <br/>
  $$(p \rightarrow q) \Leftrightarrow (p \wedge \sim q) \rightarrow c$$ 임을 보이면 됨 ($$c$$는 항상 False) <br/>
  가장 쉬운 방법으로는 진리표가 있음 <br/>
  [귀류법 증명](https://m.blog.naver.com/PostView.nhn?blogId=da91love&logNo=220375037913&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F) 참조

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="명제" %}

## 수학 1
TBD

## 수학 2
TBD

## 적분과 통계
TBD

## 기하와 벡터
TBD

# 미적분학
TBD

# TO BE DONE!
