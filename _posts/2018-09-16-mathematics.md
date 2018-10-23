---
title: "고등학교 입학부터 대학교 졸업까지, 수학 압축서"
date: 2018-09-16 16:05:25 -0400
categories: posts
classes: wide
use_math: true
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
* 명제는 참/거짓을 내릴 수 있는 문장이며, 조건은 변수 $ x $에 값을 대입하면 명제가 되는 문장.
* $p \rightarrow q$, $p \Rightarrow q$, $P \subset Q \Rightarrow (p \Rightarrow q)$

{% capture context1 %}
#### 조건
* 조건에 포함된 변수 $x$는 $U \neq \varnothing$ 을 정의역으로 함.
* 전체집합 $U$에서의 조건 $p(x)$를 간단히 조건 $p$라고 표기함.
* $U$의 원소 $a$를 대입한 $p(a)$가 참인 명제라면, 명제 $p(a)$가 성립한다, $a$는 조건 $p(x)$를 만족한다 라고 함.

#### 부정
* 명제 $p$ 혹은 조건 $p(x)$에 대해 $p(x)$가 아니다 를 $p(x)$의 부정이라 하고, $\sim p(x)$$로 표기함.

<p> $$ \sim (p \vee q) \Leftrightarrow (\sim p \wedge \sim q), \sim (p \wedge q) \Leftrightarrow (\sim p \vee \sim q) $$ </p>
<p> $$ \sim (\forall x, p(x)) \Leftrightarrow (\exists x, \sim p(x)), \sim (\exists x, p(x)) \Leftrightarrow (\forall x, \sim p(x))$$ </p>

#### 진리집합
* $p(x)$를 만족하는 $x$ 전체의 집합 $P$를 조건 $p(x)$의 진리집합이라고 한다.<br/>
* $P = \{ x \mid x \in U, p(x) \}$. 표기시 전체집합 $U$를 씹으려는 경향이 강하므로 $P=\{ x \mid p(x) \}$로도 표기.

#### 조건과 집합
* 집합 $P$, $Q$를 조건 $p$, $q$의 진리집합이라고 둘 때,

<p> $$ P \subset Q \Leftrightarrow (p \Rightarrow q), P \nsubseteq Q \Leftrightarrow (p \nLeftarrow q), \\
p \vee q \Leftrightarrow P \cup Q, p \wedge q \Leftrightarrow P \cup Q, \sim p \Leftrightarrow P^c $$ </p>

#### 필요 · 충분 조건
* $p \Rightarrow q$일 때, $p$는 $q$이기 위한 충분조건이고 $q$는 $p$이기 위한 필요조건이 된다.
* $p \Leftrightarrow q$ 면 서로 필요충분조건(동치).
* 집합과의 관계는 $P \subset Q \Rightarrow (p \Rightarrow q) $

#### 귀류법
* 어떤 명제 $p \rightarrow q$임을 증명하려 할 때, 대우 $\sim q \rightarrow \sim p$를 증명하는 방법
* 명제의 결론을 부정하여 공리, 정리, 가정 등에 모순이 됨을 이끌어내면 된다.
{% endcapture %}

{% capture context2 %}

* 두 **조건** $p$, $q$를 $p \rightarrow q$ 꼴로 연결하면 명제가 되어버림. <br/>
 '4의 약수는 8의 약수이다' 를 풀어서 '$x$가 4의 약수이면 $x$는 8의 약수이다' 로 명제와 같이 표현가능.
* $(P \subset Q) \Rightarrow (x \in P \Rightarrow x \in Q) \Rightarrow (p \Rightarrow q)$
* $ \sim (p \vee q) \Rightarrow (P \cup Q)^c \Rightarrow P^c \cup Q^c \Rightarrow \sim p \wedge \sim q $
* $ \sim$ (모든 $x$에 대하여 $p(x)$이다) $\Rightarrow \sim (p(x_1) \; and \; p(x_2) \; and \; \cdots \; and \; p(x_n))$ <br/>
  $ \Rightarrow \sim p(x_1) \; or \; \sim \; p(x_2) \; or \; \cdots \; or \; \sim p(x_n) \Rightarrow$ 어떤 $x$에 대하여 $\sim p(x) $ <br/>
  비슷한 방법으로 모두 증명 가능
* 귀류법이 옳다는 것을 증명하는 방법 : <br/>
  $(p \rightarrow q) \Leftrightarrow (p \wedge \sim q) \rightarrow c$ 임을 보이면 됨 ($c$는 항상 False) <br/>
  가장 쉬운 방법으로는 진리표가 있음 <br/>
  [귀류법 증명](https://m.blog.naver.com/PostView.nhn?blogId=da91love&logNo=220375037913&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F) 참조

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="명제" %}

### 실수 체계
* 일반적 연산에 대한 닫혀 있다(closed under) 의 개념
* 항등원과 역원

{% capture context1 %}
#### 일반적 연산
* 집합 $M$의 두 원소 $a$, $b$의 순서쌍 $(a, b)$에 대응하는 $M$의 원소 $c$가 하나 정해질 때,
이 대응을 집합 $M$의 이항연산 또는 연산이라고 함.
* 기호 $\circ$ 등을 써서 $a \circ b = c$ 등으로 표기.
* 연산 $\circ$이 정의되어 있는 집합 $M$의 부분집합 $N$에 대하여, <br/>
  $a \in N, b \in N \Rightarrow a \circ b \in N$ 이면 $N$은 $\circ$에 관하여 닫혀 있다라고 함.

#### 교환, 결합법칙
* 교환법칙이 성립 $ \Leftrightarrow a \circ b = b \circ a $
* 결합법칙이 성립 $ \Leftrightarrow (a \circ b) \circ c = a \circ (b \circ c) $

#### 항등원, 역원
* $\forall a \in N, \exists e \in N, a \circ e = e \circ a = a$ 일 때 $e$를 $\circ$에 대한 항등원이라고 함
* $\forall a \in N, \exists x \in N, a \circ x = x \circ a = e$ 일 때 $x$를 $\circ$에 대한 역원이라고 함
{% endcapture %}

{% capture context2 %}
할말없워요
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="실수체계" %}

### 정수 문제
* 최대공약수(GCD)와 최소공배수(LCM), 유클리드 호제법
* 기수법(p진법)의 정의

{% capture context1 %}
#### GCD, LCM
* 두 개 이상의 정수의 공통인 약수를 공약수라 하고, 그 중 가장 큰 수를 최대공약수라 함
* 두 개 이상의 정수의 공통인 배수를 공배수라 하고, 그 중 가장 큰 수를 최소공배수라 함

* $\gcd(A, B) = G, \mathrm{lcm}(A, B) = L$이라 두면, <br/>
  $A = Ga, B = Gb$ (단, $\gcd(a, b) = 1$) <br/>
  $L = Gab, LG = AB$ 를 만족함.

#### 다항식의 GCD, LCM
* 다항식 $A$, $B$, $Q$ 사이에 $A=B \cdot Q$이면 $B$를 $A$의 약수라고 표현한다.
* 2개 다항식 사이 공통인 약수를 공약수, 가장 차수가 높은 것을 최대공약수라고 함.
* 배수도 똑같
* 정수에서와 똑같은 성질을 가짐

#### 유클리드 호제법 (Euclidean algorithm)
* 맨날까먹음
* $A > B$인 임의의 자연수 $A$, $B$가 있을 때, $A = B \cdot Q + R$로 몫과 나머지를 분리하면 </br>
  <p> $$\gcd(A, B) = \gcd(B, R)$$ </p>
  임이 성립한다는 것

* 이를 확장한 Extended Euclidian Algorithm은 다음과 같다 <br/>
  <p align="center"> $as + bt=\gcd(a,b)$ 인 정수쌍 $s$, $t$가 존재함 </p>
  모듈러 연산의 역원을 구하는데 우려먹힌다.

#### 기수법
* 양의 정수 $N_p = a_n p^n + a_{n-1} p^{n-1} + \cdots + a_1 p + a_0$
* 양의 소수 $N_p = \frac{a_1}{p} + \frac{a_2}{p^2} + \cdots + \frac{a_n}{p^n}$
{% endcapture %}

{% capture context2 %}
#### Euclidean algorithm으로 gcd 찾기
<p> $$r_0 \leftarrow a, r_1 \leftarrow b \\
r_{i+1}=r_{i−1}−q_i r_i, \quad q_i=\frac{r_{i−1}}{r_i} $$ </p>

만약 $r_{i+1}=0$ 이라면 $r_i$ 가 바로 $\gcd(a,b)$ 이다.

#### Euclidean algorithm 증명
$A=Ga, B=Gb$ ($a$, $b$ 는 서로소) 를 $A=BQ+R$에 대입해보면
<p> $$Ga=Gb \cdot Q + R, \quad R=G(a-Qb) $$ </p>
이제 $b$와 $a-Qb$가 서로소임을 보이면 되는데, $b=mk$, $a-bQ=mk'$으로 두자($k$, $k'$는 서로소) <br/>
$a=bQ+mk'=m(kQ+k')$이므로 $m$은 $a$, $b$의 공약수인데, 서로소이므로 1임 <br/>
따라서 $m=1$이 되며 $b$와 $a-Qb$는 서로소가 되서 $\gcd(B, R)=G$가 되어버림

#### Extended Euclidean algorithm 증명
$r_0 \leftarrow a, r_1 \leftarrow b$ <br/>
초기값들을 넣으면 $as_i+bt_i=r_i \quad for \; i=0,1$ <br/>
이제 $i>1$일 때 참이라고 가정하고 수학적 귀납법을 쓰면

<p> $$r_{i+1}=r_{i−1}−r_i q_i=(as_{i−1}+bt_{i−1})−(as_i+bt_i)q_i=a(s_{i−1}−s_i q_i)+b(t_{i−1}−t_i q_i)=as_{i+1}+bt_{i+1} $$ </p>

따라서 $r_{i+1}=0$ 일 때 $as_i+bt_i=r_i$ 는 $as+bt=\gcd(a,b)$ 가 된다. <br/>

[Extended Euclidean algorithm 증명](https://codeonwort.tistory.com/295) 참조

{% endcapture %}
{% include blocks.html context1=context1 context2=context2 topic="유클리드" %}

{% comment %}

### 다항식의 사칙연산, 인수분해, 항등식과 미정계수법
(a-b)(a^2+ab+b^2)=a^3-b^3같은 공식을 처음 수십개씩 마주하면서 패닉상태에 빠졌던 기억이 새록새록 난다.
하지만 여기다 적을 의향은 없다
조립제법은 x의 다항식 F(x)를 x-a로 나누었을 때 몫과 나머지로 분리하는 방법임.

{% capture context1 %}
#### 조립제법
그림
{% endcapture %}

{% capture context2 %}
ㄴ
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="" %}

### 나머지정리
x의 다항식 f(x)를 x-a로 나누었을 때 나머지는 f(a)이다.

{% capture context1 %}
f(a)=0인 것과 f(x)가 x-a로 나누어떨어진다는 동치이다.
보통 f(a)=0인 a를 찾아서 f(x)를 인수분해하려고 쓴다.
f(x)=ax^n+ ... + b일 때, x= +-(b의 약수)/(a의 약수) 를 대입해본다.
{% endcapture %}

{% capture context2 %}
f(x) = (x-a)Q(x) + R는 항등식이므로, R = f(a)
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="" %}

### 이차방정식
ax^2 + bx + c = 0 => x = (-b +- root(b^2-4ac))/2a
ax^2 + 2bx + c = 0 => x = (-b +- root(b^2-ac))/a
D(Determinant) = B^2 -4ac
가끔씩 가물가물해서 빡친다
{% endcomment %}

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
