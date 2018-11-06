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
본인이 12년도 고등학교 입학이라 그 당시 교육과정을 따른다. 책이 그거밖에 없음 <br/>
<br/>
내용 구분은 보통 개념 단위로 정리할 예정이지만, 예외로 고등학교 수학과정은 단원 단위로 정리한다. <br/>
내맘임 <br/>

## 고등수학

### 명제와 조건
* 명제는 참/거짓을 내릴 수 있는 문장이며, 조건은 변수 $ x $에 값을 대입하면 명제가 되는 문장.
* $p \rightarrow q$, $p \Rightarrow q$, $P \subset Q \Rightarrow (p \Rightarrow q)$

{% capture context1 %}
#### 조건
* 조건에 포함된 변수 $x$는 $U \neq \varnothing$ 을 정의역으로 함.
* 전체집합 $U$에서의 조건 $p(x)$를 간단히 조건 $p$라고 표기함.
* $U$의 원소 $a$를 대입한 $p(a)$가 참인 명제라면, 명제 $p(a)$가 성립한다, $a$는 조건 $p(x)$를 만족한다 라고 함.
<br/>

#### 부정
* 명제 $p$ 혹은 조건 $p(x)$에 대해 $p(x)$가 아니다 를 $p(x)$의 부정이라 하고, $\sim p(x)$$로 표기함.

<p> $$ \sim (p \vee q) \Leftrightarrow (\sim p \wedge \sim q), \sim (p \wedge q) \Leftrightarrow (\sim p \vee \sim q) $$ </p>
<p> $$ \sim (\forall x, p(x)) \Leftrightarrow (\exists x, \sim p(x)), \sim (\exists x, p(x)) \Leftrightarrow (\forall x, \sim p(x))$$ </p>
<br/>

#### 진리집합
* $p(x)$를 만족하는 $x$ 전체의 집합 $P$를 조건 $p(x)$의 진리집합이라고 한다.
* $P = \left\\{ x \mid x \in U, p(x) \right\\}$. 표기시 전체집합 $U$를 씹으려는 경향이 강하므로 $P=\left\\{ x \mid p(x) \right\\}$로도 표기.
<br/>

#### 조건과 집합
* 집합 $P$, $Q$를 조건 $p$, $q$의 진리집합이라고 둘 때,

<p> $$ P \subset Q \Leftrightarrow (p \Rightarrow q), P \nsubseteq Q \Leftrightarrow (p \nLeftarrow q), \\
p \vee q \Leftrightarrow P \cup Q, p \wedge q \Leftrightarrow P \cup Q, \sim p \Leftrightarrow P^c $$ </p>
<br/>

#### 필요 · 충분 조건
* $p \Rightarrow q$일 때, $p$는 $q$이기 위한 충분조건이고 $q$는 $p$이기 위한 필요조건이 된다.
* $p \Leftrightarrow q$ 면 서로 필요충분조건(동치).
* 집합과의 관계는 $P \subset Q \Rightarrow (p \Rightarrow q) $
<br/>

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

{% include blocks.html context1=context1 context2=context2 topic="고등수학_명제" %}

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
<br/>

#### 교환, 결합법칙
* 교환법칙이 성립 $ \Leftrightarrow a \circ b = b \circ a $
* 결합법칙이 성립 $ \Leftrightarrow (a \circ b) \circ c = a \circ (b \circ c) $
<br/>

#### 항등원, 역원
* $\forall a \in N, \exists e \in N, a \circ e = e \circ a = a$ 일 때 $e$를 $\circ$에 대한 항등원이라고 함
* $\forall a \in N, \exists x \in N, a \circ x = x \circ a = e$ 일 때 $x$를 $\circ$에 대한 역원이라고 함
{% endcapture %}

{% capture context2 %}
* 이후에 다루겠지만, 어떤 집합 $M$에 포함된 원소들이 어떤 연산 $\circ$에 대하여 교환, 결합법칙이 성립하고 항등원, 역원이 존재하면,
$M$은 $\circ$에 대하여 군(Group)을 이룬다고 한다. <br/>
  여기까지 내용이 넘어가려면 얼마나 걸리려나

{% comment %}
https://m.blog.naver.com/PostView.nhn?blogId=obrigadu&logNo=50098477517&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F
{% endcomment %}

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_실수체계" %}

### 정수 문제
* 최대공약수(GCD)와 최소공배수(LCM),
* 유클리드 호제법 $A=BQ+R \Rightarrow \gcd(A, B) = \gcd(B, R)$

{% capture context1 %}
#### GCD, LCM
* 두 개 이상의 정수의 공통인 약수를 공약수라 하고, 그 중 가장 큰 수를 최대공약수라 함
* 두 개 이상의 정수의 공통인 배수를 공배수라 하고, 그 중 가장 큰 수를 최소공배수라 함

* $\gcd(A, B) = G, \mathrm{lcm}(A, B) = L$이라 두면, <br/>
  $A = Ga, B = Gb$ (단, $\gcd(a, b) = 1$) <br/>
  $L = Gab, LG = AB$ 를 만족함.
<br/>

#### 다항식의 GCD, LCM
* 다항식 $A$, $B$, $Q$ 사이에 $A=B \cdot Q$이면 $B$를 $A$의 약수라고 표현한다.
* 2개 다항식 사이 공통인 약수를 공약수, 가장 차수가 높은 것을 최대공약수라고 함.
* 배수도 똑같
* 정수에서와 똑같은 성질을 가짐
<br/>

#### 유클리드 호제법 (Euclidean algorithm)
* 맨날까먹음
* $A > B$인 임의의 자연수 $A$, $B$가 있을 때, $A = B \cdot Q + R$로 몫과 나머지를 분리하면 </br>
  <p> $$\gcd(A, B) = \gcd(B, R)$$ </p>
  임이 성립한다는 것

* 이를 확장한 Extended Euclidian Algorithm은 다음과 같다 <br/>
  <p align="center"> $as + bt=\gcd(a,b)$ 인 정수쌍 $s$, $t$가 존재함 </p>
  모듈러 연산의 역원을 구하는데 우려먹힌다.
<br/>

#### 기수법
* 양의 정수 $N_p = a_n p^n + a_{n-1} p^{n-1} + \cdots + a_1 p + a_0$
* 양의 소수 $N_p = \frac{a_1}{p} + \frac{a_2}{p^2} + \cdots + \frac{a_n}{p^n}$
{% endcapture %}

{% capture context2 %}
#### Euclidean algorithm으로 gcd 찾기
<p> $$r_0 \leftarrow a, r_1 \leftarrow b \\
r_{i+1}=r_{i−1}−q_i r_i, \quad q_i=\frac{r_{i−1}}{r_i} $$ </p>

만약 $r_{i+1}=0$ 이라면 $r_i$ 가 바로 $\gcd(a,b)$ 이다.
<br/>

#### Euclidean algorithm 증명
$A=Ga, B=Gb$ ($a$, $b$ 는 서로소) 를 $A=BQ+R$에 대입해보면
<p> $$Ga=Gb \cdot Q + R, \quad R=G(a-Qb) $$ </p>
이제 $b$와 $a-Qb$가 서로소임을 보이면 되는데, $b=mk$, $a-bQ=mk'$으로 두자($k$, $k'$는 서로소) <br/>
$a=bQ+mk'=m(kQ+k')$이므로 $m$은 $a$, $b$의 공약수인데, 서로소이므로 1임 <br/>
따라서 $m=1$이 되며 $b$와 $a-Qb$는 서로소가 되서 $\gcd(B, R)=G$가 되어버림
<br/>

#### Extended Euclidean algorithm 증명
$r_0 \leftarrow a, r_1 \leftarrow b$ <br/>
초기값들을 넣으면 $as_i+bt_i=r_i \quad for \; i=0,1$ <br/>
이제 $i>1$일 때 참이라고 가정하고 수학적 귀납법을 쓰면

<p> $$r_{i+1}=r_{i−1}−r_i q_i=(as_{i−1}+bt_{i−1})−(as_i+bt_i)q_i=a(s_{i−1}−s_i q_i)+b(t_{i−1}−t_i q_i)=as_{i+1}+bt_{i+1} $$ </p>

따라서 $r_{i+1}=0$ 일 때 $as_i+bt_i=r_i$ 는 $as+bt=\gcd(a,b)$ 가 된다. <br/>

[Extended Euclidean algorithm 증명](https://codeonwort.tistory.com/295) 참조

{% endcapture %}
{% include blocks.html context1=context1 context2=context2 topic="고등수학_유클리드" %}

### 다항식의 사칙연산, 인수분해, 항등식과 미정계수법
$(a-b)(a^2+ab+b^2)=a^3-b^3$같은 공식 수십개 - 응 안적어 <br/>
조립제법으로 다항식 인수분해

{% capture context1 %}
#### 조립제법
$x$의 다항식 $F(x)$를 $x-a$로 나누었을 때 몫과 나머지로 분리하는 방법.<br/>
![Alt text](/pictures/mathematics/690b6a0d.png)
{% endcapture %}

{% capture context2 %}
ㄴ
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_조립제법" %}

### 나머지정리
$x$의 다항식 $f(x)$를 $x-a$로 나누었을 때 나머지는 $f(a)$이다.

{% capture context1 %}
$f(a)=0$인 것과 $f(x)$가 $x-a$로 나누어떨어진다는 동치이다.
보통 $f(a)=0$인 $a$를 찾아서 $f(x)$를 인수분해하려고 쓴다.
$f(x)=ax^n+ \cdots + b$일 때, $x= \pm \frac{b의 약수}{a의 약수}$ 를 대입해본다.
{% endcapture %}

{% capture context2 %}
$f(x) = (x-a)Q(x) + R$는 항등식이므로, $R = f(a)$
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_나머지정리" %}

### 이차방정식
<p> $$
  \begin{align*}
    ax^2 + bx + c = 0 \Rightarrow & x = \left(-b \pm \frac{\sqrt{b^2-4ac}}{2a}\right) \\
    ax^2 + 2bx + c = 0 \Rightarrow & x = \left(-b \pm \frac{\sqrt{b^2-ac}}{a}\right) \\
    D(\mathrm{Determinant}) = & b^2 -4ac
  \end{align*}
$$ </p>
가끔씩 가물가물해서 빡친다

### 점과 좌표
* 선분의 내분점과 외분점 $\frac{mx_2 \pm nx_1}{m+n}$
* Pappus의 정리, 삼각형의 무게중심 등등 잡다한 것들

{% capture context1 %}
#### 선분의 내분점과 외분점
* $\overline{AB}$를 $m:n$으로 내분하는 점 $P$의 좌표는 $\frac{mx_2+nx_1}{m+n}$
* $\overline{AB}$를 $m:n$으로 외분하는 점 $P$의 좌표는 $\frac{mx_2-nx_1}{m-n}$
<br/>

#### 삼각형의 무게중심, Pappus의 정리
* $A(x_1, y_1), B(x_2, y_2), C(x_3, y_3)$인 $\triangle ABC$의 무게중심은
<p> $$\left(\frac{x_1+x_2+x_3}{3}, \frac{y_1+y_2+y_3}{3}\right)$$ </p>
<br/>
![Alt text](/pictures/mathematics/27755D4256A82ED122.png)
* $\triangle ABC$ 의 변 $\overline{BC}$의 중점을 $M$이라 둘 때,
$\overline{AB}^2 + \overline{BC}^2 = 2(\overline{AM}^2 + \overline{BM}^2)$
{% endcapture %}

{% capture context2 %}
* 삼각형의 무게중심 $G$는 점 $A(x_1, y_1)$와 $\overline{BC}$의 중점 $M\left(\frac{x_2+x_3}{2}, \frac{y_2+y_3}{2}\right)를 $2:1$로 내분하는 점. <br/>
  나머지 변에 대해서도 마찬가지.

* 파푸스 정리는 그냥 위에 넣은 그림대로 좌표넣고 계산때려보면 $2(a^2+b^2+c^2)$로 같다.
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_점과좌표" %}

### 직선의 방정식
* 표준형 $y=ax+b$, 일반형 $ax+by+c=0$, 기울기+점, 두 점, $x$ $y$절편이 주어졌을 때 식 등등
* 점과 직선 사이의 거리 $d=\frac{\left\|ax_1+by_1+c\right\|}{\sqrt{a^2+b^2}}$

{% capture context1 %}
#### 방정식
* 표준형: $y=ax+b$
* 일반형: $ax+by+c=0$
* 기울기+점: $y-y_1=m(x-x_1)$
* 두 점: $y-y_1=\frac{y_2-y_1}{x_2-x_1}(x-x_1)$
* $x$ $y$절편: $\frac{x}{a}+\frac{y}{b}=1$ <br/>
* 두 직선 $ax+by+c=0$, $a'x+b'y+c'=0$의 교점을 지나는 직선들의 방정식 <br/>
  $m(ax+by+c) + (a'x+b'y+c') = 0$
<br/>

#### 수직인 직선
* $y=ax+b$, $y=a'x+b'$이 수직이라면, $aa'=-1$
<br/>

#### 점과 직선 사이의 거리
* 점$(x_1, y_1)$과 직선 $ax+by+c=0$ 사이의 거리 $d=\frac{\left\|ax_1+by_1+c\right\|}{\sqrt(a^2+b^2)}$
{% endcapture %}

{% capture context2 %}
#### 서로 수직인 두 직선
* $y=ax+b, y=a'x+b'$이 수직이라면, <br/>
  $\tan(\theta_1)=a, \tan(\theta_2)=\tan(\theta_1+\frac{\pi}{2})=-\frac{1}{\tan(\theta_1)}=a'$ <br/>
  $ \therefore a'=-\frac{1}{a}, aa'=1 $
<br/>

#### 점과 직선 사이의 거리
* 점 $P$와 직선 $l$ 사이의 거리는, $P$에서 $l$로 내린 수선의 발 $Q(x', y')$과 $P$ 사이의 거리와 같음. <br/>
  <p> $$d^2 = (x'-x_1)^2+(y'-y_1)^2$$ </p>
* $P$를 지나 $l$에 수직인 직선의 방정식은 $y-y_1=\frac{b}{a}(x-x_1), b(x-x_1)-a(y-y_1)=0$ <br/>
  위 식과 $ax+by+c=0$에 $x=x', y=y'$을 대입하고 소거하여 $x'-x_1, y'-y_1$을 구하면 $d^2$을 구할 수 있다.
* 하면된다
* 넌 할수었어
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_직선" %}
 
### 원의 방정식
* 표준형 $(x-a)^2+(y-b)^2=r^2$, 일반형 $x^2+y^2+Ax+By+C=0$
* 접선의 방정식 $(x_1-a)(x-a)+(y_1-b)(y-b)=r^2, y-b=m(x-a)\pm r \sqrt{m^2+1}$
* 원과 직선의 교차, 두 원의 교차판별 등등

{% capture context1 %}
#### 방정식
* 표준형: $(x-a)^2+(y-b)^2=r^2$
* 일반형: $x^2+y^2+Ax+By+C \rightarrow$
  * 중심$\left(-\frac{A}{2}, -\frac{B}{2}\right)$, 반지름 $\frac{\sqrt{A^2+B^2-4C}}{2}$
  * $A^2+B^2-4C<0$ 이면 허원 이라고도 한단다.
* 세 점을 지나는 원: 일반형에 세 좌표 쑤셔넣고 연립
<br/>

#### 원과 직선의 관계
* 직선은 $y=mx+n$이요 원은 $f(x, y)=0$이기 때문에, <br/>
  $y$를 소거하여 $f(x, mx+n)$으로 해버리면 이차방정식이 되어버림. <br/>
  이때 판별식 $D$에 따라서 두 실근, 중근, 두 허근으로 나뉜다. <br/>

* 표준형의 원 위의 점$(x_1, y_1)$에서의 접선의 방정식은
  <p> $$(x_1-a)(x-a)+(y_1-b)(y-b)=r^2$$ </p>
* 기울기가 $m$인 접선의 방정식은
  <p> $$y-b=m(x-a)\pm r \sqrt{m^2+1}$$ </p>
<br/>

#### 두 원의 관계
* 서로 만나는 두 원 $x^2+y^2+Ax+By+C=0$, $x^2+y^2+A'x+B'y+C'=0$ 의 교점을 지나는 원의 방정식은 <br/>
  $(x^2+y^2+Ax+By+C)m + (x^2+y^2+A'x+B'y+C') = 0$ 이며  <br/>
  $m=-1$ 이라서 이차항을 조져버리면 두 원의 공통현의 방정식이 되버린다.
{% endcapture %}

{% capture context2 %}
#### 접선의 방정식
* 접선의 방정식 $y=mx+n$이 우선 $x^2+y^2=r^2$에 접한다고 치자. <br/>
  * $y$에 $mx+n$을 집어넣고 판별식을 구하면 <br/>
    $\frac{D}{4}=m^2 n^2 -(m^2+1)(n^2-r^2)=0, \therefore r^2 m^2-n^2+r^2=0$
  * 접하는 점의 좌표가 $(x_1, y_1)$이므로 <br/>
    $n=y-mx_1, x_1^2+y_1^2=r^2$
  * 열심히 대입하면 $y_1^2 m^2 + 2x_1 y_1 m + x_1^2=(y_1 m + x_1)^2 = 0, m=-\frac{x_1}{y}$ <br/>
  * 그래서 접선의 방정식은 $y-y_1=-\frac{x}{y_1}(x-x_1), x_1x + y_1 y=r^2$가 된당  <br/>

* 원의 방정식이 $(x-a)^2+(y-b)^2=r^2$로 바뀐다고 하면 $(a, b)$만큼 평행이동시키면 <br/>
  접선의 방정식은 $(x_1-a)(x-a)+(y_1-b)(y-b)=r^2$ <br/>

* $x^2+y^2=r^2$에서 기울기가 $m$인 접선을 구하면 <br/>
  * $x^2+(mx+b)^2=r^2, \frac{D}{4} = b^2 m^2-(m^2+1)(b^2-r^2)=0, b^2=(m^2+1)r^2$ <br/>
    $\therefore b=\pm r \sqrt{m^2+1}, y=mx \pm r\sqrt{m^2+1}$ <br/>

* $(x-a)^2+(y-b)^2=r^2$로 일반화하면 $y-b=m(x-a)\pm r \sqrt{m^2+1}$
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_원" %}

### 도형의 이동
* 점과 도형의 평행이동, 대칭이동

{% capture context1 %}
#### 평행이동
* $x$축으로 $a$, $y$축으로 $b$만큼 평행이동시킬 때, $T: (x, y) \rightarrow (x+a, y+b)$로 표기하고
* 점 $P(x, y) \rightarrow Q(x+a, y+b)$
* 도형의 방정식 $f(x-a, y-b)=0 \rightarrow f(x-a, y-b)=0$
<br/>

#### 대칭이동
* $x$축 - $T: (x, y) \rightarrow (x, -y)$
* $y$축 - $T: (x, y) \rightarrow (-x, y)$
* 원점 - $T: (x, y) \rightarrow (-x, -y)$
* $y=x$ - $T: (x, y) \rightarrow (y, x)$

{% endcapture %}

{% capture context2 %}
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_이동" %}

### 함수
* 함수의 정의, 정의역, 공역, 치역
* 일대일 함수, 일대일 대응, 항등함수, 상수함수, 합성함수 등등 잡다한 정의들

{% capture context1 %}
#### 함수의 정의
* 두 집합 $X, Y \neq \varnothing$ 이 있을 때,
$X$의 각 원소에서 $Y$의 원소로의 대응을 $X$에서 $Y$로 가는 함수라고 정의하고 $f: X \longrightarrow Y$로 표기함
* 이때 함수 $f$에 대하여 $x \in X$에 $y \in Y$가 대응되는 것을 $f: x \longrightarrow y$, $y=f(x)$ 등으로 나타냄.
* $x$를 독립변수, $y$를 종속변수라고도 한단다.
* 아무튼 하나의 x에 대해서 반드시 하나의 y가 대응되어야 한다는게 중요함
<br/>

#### 정의역, 공역, 치역
![Alt text](/pictures/mathematics/250F12365368EBE529.jpg)
<br/>

#### 함수의 종류
* 일대일 함수
  * $\forall x_1, x_2 \in X, x_1 \neq x_2 \Rightarrow f(x_1) \neq f(x_2)$
* 일대일 대응
  * 치역과 공역이 같고
  * $\forall x_1, x_2 \in X, x_1 \neq x_2 \Rightarrow f(x_1) \neq f(x_2)$
  * 역함수가 존재함
* 항등함수
  * $X=Y$
  * $\forall x \in X, f(x)=x$
  * $I_x$로 표기
* 상수함수
  * 치역의 원소가 하나뿐임
<br/>

#### 합성함수
* 두 함수 $f: X \longrightarrow Y$, $g: Y \longrightarrow Z$일 때, $g(f(x))$는 정의역이 $X$이고 공역이 $Z$가 된다.
* 함성함수 $g \circ f$는 $g \circ f: x \longrightarrow g(f(x)), \; (g \circ f)(x) = g(f(x))$

{% endcapture %}

{% capture context2 %}
#### 합성함수와 Group의 성질
* 교환법칙: $g \circ f \neq f \circ g$
* 결합법칙: $h \circ (g \circ f) = (h \circ g) \circ f$
* 항등원: $f \circ I = I \circ f = f$
* 함수가 일대일 대응일 경우 역원도 존재하며, 뒤에 역함수로 나옴.
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_함수" %}

### 유리, 무리함수와 역함수
* $y=\frac{k}{x}, \; y=\frac{k}{x-m}+n, \; y=k'x+\frac{k}{x}, \; y^2=ax$의 그래프
* 일대일 대응인 함수 $f:X \longrightarrow Y$ 에 대하여 역함수 $f^{-1}: Y \longrightarrow X$

{% capture context1 %}
#### 유리수
* $k$에 따른 $y=\frac{k}{x}$ <br/>
![Alt text](/pictures/mathematics/캡처2.JPG)

* $n, m$이 주어진 $y=\frac{k}{x-m}+n$ <br/>
![Alt text](/pictures/mathematics/캡처3.JPG)

* $k, k'$에 따른 $y=k'x+\frac{k}{x}$ <br/>
![Alt text](/pictures/mathematics/캡처.JPG)

킹갓구글에서 그래프까지 그려주는줄은 몰랐읍니다 충성충성
<br/>

#### 무리함수
* $y^2=ax, y=\pm \sqrt{\pm ax}$ <br/>
![Alt text](/pictures/mathematics/캡처4.JPG) <br/>
  정의역과 치역을 좀 생각해야된다.

<br/>
#### 역함수
* 역함수의 정의를 위해선, $f:X \longrightarrow Y$에서 $Y$의 임의의 한 원소에 $X$의 원소가 하나씩만 대응되어야 하기 때문에 일대일 대응이어야 함. <br/>
* $y=f(x) \Leftrightarrow x=f^{-1}(y)$
* 함수 $f$가 일대일 대응이면 역함수 $f^{-1}$은 존재한다 (존재성)

<br/>
#### 역함수의 성질
* $(f^{-1})^{-1} = f$
* $f^{-1}(f(x))=x \quad (f^{-1} \circ f = I_x)$
* $f(f^{-1}(y))=y \quad (f \circ f^{-1} = I_y)$
* $f:X \longrightarrow Y, g:Y \longrightarrow X$에서 $g \circ f = I_x, f \circ g = I_y \Leftrightarrow g=f^{-1}$ (유일성)
* 일대일 대응 $f:X \longrightarrow Y, g:Y \longrightarrow Z$에 대하여  $(g \circ f)^{-1} = f^{-1} \circ g^{-1}$

{% endcapture %}

{% capture context2 %}
#### 역함수 증명
* 존재성, 유일성 - TODO <br/>

* $(g \circ f)^{-1} = f^{-1} \circ g^{-1}$ 증명
  <p> $$(f^{-1} \circ g^{-1}) \circ (g \circ f) = f^{-1} \circ (g^{-1} \circ g) \circ f = f^{-1} \circ I \circ f = f^{-1} \circ f = I \\
        (g \circ f) \circ (f^{-1} \circ g^{-1}) = g \circ (f \circ f^{-1}) \circ g^{-1} = g \circ I \circ g^{-1} = g \circ g^{-1} = I \\
        \therefore (g \circ f)^{-1} = f^{-1} \circ g^{-1}$$ </p>
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_유리함수" %}

### 최대와 최소
* 산술평균 $\geq$ 기하평균 $\geq$ 조화평균 ==> $\frac{a+b}{2} \geq \sqrt{ab} \geq \frac{2}{\frac{1}{a}+\frac{1}{b}}$, 등호는 $a=b$
* 코시-슈바르츠 부등식 $(a^2+b^2)(x^2+y^2) \geq (ax+by)^2$, 등호는 $\frac{a}{x}=\frac{b}{y}$

{% capture context1 %}
#### 판별식을 이용한 최대, 최소
* $y=ax^2+bx+c$에서 $y$의 범위는 $0=ax^2+bx+(c-y)$에서 $D>=0$를 사용해도 됨
<br/>

#### 산술기하조화
* 일반적인 형태로,
<p> $$ \frac{x_1 + x_2 + \cdots + x_n}{n} \geq \sqrt[n]{x_1 x_2 \cdots x_n} \geq \frac{n}{\frac{1}{x_1}+\frac{1}{x_2}+ \cdots + \frac{1}{x_n}} $$ </p>
* $n=2$일 때 증명은 쉽다. 하지만 $n$항으로 일반화하면...

![Alt text](/pictures/mathematics/산술기하조화.jpg) {: width="50%" height="50%"}
$n=2$일 때 증명은 너무 쉽다고 심지어 그림으로 농락하는것도 있다...
<br/>

#### 가중 산술-기하 평균 부등식
* 각 항 앞에 가중치를 더한 부등식이다.
* 가중 산술-기하 평균 부등식은
<p> $$ \frac{\alpha_1 x_1 + \cdots + \alpha_n x_n}{\alpha} \geq \sqrt[\alpha]{x_1^{\alpha_1} \cdots x_n^{\alpha_n}} \\
       (x_i>0, \alpha_i>0) $$ </p>
<br/>

#### 코시-슈바르츠 부등식
* 일반식은
  <p> $$ (a_1^2+a_2^2+\cdots+a_n^2)(x_1^2+x_2^2+\cdots+x_n^2) \geq (a_1x_1+a_2x_2+\cdots+a_nx_n)^2 $$ </p>
* 아예 제곱항도 $p$로 일반화시키면 [횔더 부등식](http://mathseodang.com/220450030140)이 된다
  <p> $$ \left(\sum_{i=1}^{n} {a_i^p}\right)^{1/p}\left(\sum_{i=1}^{n} {b_i^q}\right)^{1/q} \geq \sum_{i=1}^{n} {a_i b_i} \\
         p>1, q>1, \frac{1}{p}+\frac{1}{q}=1, \; equality \; iff \; a_i^p=\lambda b_i^q $$ </p>

{% endcapture %}

{% capture context2 %}
#### 젠센 부등식
먼저 볼록 함수의 정의부터 살펴보자
<br/>

##### 볼록 함수(convex function)
* 함수 $f:X\longrightarrow R$가 다음을 만족하면 볼록 함수로 부름 <br/>
  ![Alt text](/pictures/mathematics/볼록.png)
  <p> $$ \forall x_1, x_2 \in X, \forall t \in [0, 1]: f(tx_1+(1-t)x_2) \leq tf(x_1)+(1-t)f(x_2) $$ </p>
* 등호를 빼면 strictly convex function 이다.

----------------
<br/>

* 머암튼 $f:(a,b) \longrightarrow R$가 연속인 볼록 함수라면, 젠센 부등식은
  <p> $$ \forall x_i \in (a, b), p_i > 0, \sum_{i=1}^{n} {p_i} = 1 \; 일 \, 때 \; f\left(\sum_{i=1}^{n} {p_i x_i}\right) \leq \sum_{i=1}^{n} {p_i f(x_i)} $$
* 증명은 [수학적 귀납법](http://suhak.tistory.com/221)으로.
<br/>

#### (가중) 산술기화조화 증명
* 산술-기화-조화 평균 부등식도 사실 귀납법으로 증명이 된다. 하지만 가중치까지 넣어서 바로 젠센부등식으로 증명해보면
  * 위로 볼록한 만만한 함수 $f(x)=-\ln(x)$ 로 두고
<p> $$
  \begin{align*}
    \alpha_1 + \alpha_2 + \cdots + \alpha_n = \alpha, & w_i = \frac{\alpha_i}{\alpha} \\
    f(w_1 x_1 + \cdots + w_n x_n) & \leq w_1 f(x_1) + \cdots + w_n f(x_n) \\
    \ln(w_1 x_1 + \cdots + w_n x_n) & \geq w_1 \ln(x_1) + \cdots + w_n \ln(x_n) = \ln(x_1^{w_1} \cdots x_n^{w_n}) \\
    \therefore w_1 x_1 + w_2 x_2 + \cdots + w_n x_n & \geq x_1^{w_1} x_2^{w_2} \cdots x_n^{w_n} \\
    \frac{\alpha_1 x_1 + \alpha_2 x_2 + \cdots + \alpha_n x_n}{\alpha} & \geq \sqrt[\alpha]{x_1^{\alpha_1} x_2^{\alpha_2} \cdots x_n^{\alpha_n}}
  \end{align*}
$$ </p>

* 기하-조화평균은 <br/>
  $f(\frac{w_1}{x_1} + \cdots + \frac{w_n}{x_n}) \leq w_1 f(\frac{1}{x_1}) + \cdots + w_n f(\frac{1}{x_n})$ 으로 똑같이 증명됨 <br/>

꺄륵

<br/>

#### 코시-슈바르츠 부등식 증명
* [별별 증명법](https://m.blog.naver.com/yh6613/220458975310)이 다 있다.
* 귀찮은 기념으로 간단하게만 설명하면
  * $let A=\sqrt{a_1^2+a_2^2+\cdots+a_n^2}, B=\sqrt{b_1^2+b_2^2+\cdots+b_n^2}$
  * 산술 기화평균 부둥식에 따라 <br/>
    $\sqrt{\dfrac{a_i^2}{A^2} \dfrac{b_i^2}{B^2}} \leq \dfrac{1}{2}\left(\dfrac{a_i^2}{A^2}+\dfrac{b_i^2}{B^2}\right)$
  * 이걸 $i=1$ 부터 $n$에 대한 부등식을 모두 더하면 우변은 1이 되고, 결국 $\sum_{i=1}^{n} {\sqrt{a_i^2 b_i^2}} \leq AB$로 증명된다. <br/>

<br/>
* [재배열 부등식](http://mathseodang.com/220455558272) 도 볼만함

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_최대와최소" %}

### 삼각함수의 정의
* 호도(radian)법: $l=r\theta, \; S=\frac{1}{2}r^2\theta=\frac{1}{2}rl, \; 1\,rad = \frac{180\degree}{\pi}$
* 이 때 $P(x,y)$와 $\theta=\angle xOP$에 대하여, $\sin\theta=\frac{y}{r}, \; \cos\theta=\frac{x}{r}, \; \tan\theta=\frac{y}{x}$이라 정의함

{% capture context1 %}
#### 부채꼴의 넓이
* $l=r\theta$ 인건 $\theta$의 radian 정의임 $\left(\frac{l}{2\pi r}=\frac{\theta}{2\pi}\right)$
* 이 때 $\frac{S}{\pi r^2} = \frac{\theta}{2\pi}$에서 $S=\frac{1}{2}r^2\theta$

<br/>
#### 웃겨서 넣어봤다
![Alt text](/pictures/mathematics/8177-2-7693.gif)  {: width="40%" height="40%"} <br/>
얼싸안코

{% endcapture %}

{% capture context2 %}
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_삼각함수" %}

-------------------------------------

### 으악!
**아래 내용은 더럽게 기억이 나지 않습니다** <br/>
**자라나라 머리머리**

-------------------------------------

### 삼각함수 잡다한 공식(1)
* $\tan\theta = \frac{sin\theta}{\cos\theta}$
* $\tan^2\theta + 1 = \frac{1}{\cos^2 \theta}$
* $\sin(\pi-\theta)=\sin\theta, \cos(\pi-\theta)=-\cos\theta, \tan(\pi-\theta)=-\tan\theta$
* $\sin(\frac{\pi}{2}-\theta)=\cos\theta, \cos(\frac{\pi}{2}-\theta)=\sin\theta, \tan(\frac{\pi}{2}-\theta)=\frac{1}{\tan\theta}$
<br/>

![Alt text](/pictures/mathematics/사인법칙.jpg)
* 사인법칙 $\dfrac{a}{\sin A}=\dfrac{b}{\sin B}=\dfrac{c}{\sin C}=2R$
* 제1 코사인법칙 $a=b\cos C + c\cos B$
* 제2 코사인법칙 $a^2=b^2+c^2-2bc\cos A$
* $\vartriangle ABC$의 넓이 $S=\frac{1}{2}bc \sin A = \sqrt{s(s-a)(s-b)(s-c)} (2s=a+b+c)$

{% capture context1 %}
증명법은 아래에
{% endcapture %}

{% capture context2 %}
#### 사인법칙
##### 원주각
![Alt text](/pictures/mathematics/원주각.png)
* 원 위의 세 점을 잡아서 만드는 각. 저기서 $\angle APB$
* 같은 원 위의 원주각은 모두 동일하다. [링크](https://mathbang.net/186) 참조
* 이건 중학교 수학이다. 물론 기억안남 <br/>
  엌ㅋㅋㅋ

<br/>
![Alt text](/pictures/mathematics/사인법칙.png)
* 아무튼 점 $B$와 $O$를 잇는 선분과 원이 만나는 점 $A'$를 두면 증명이 된다.
* 자세한건 [링크](https://www.mathfactory.net/10678) 참조

<br/>
#### 코사인 법칙
![Alt text](/pictures/mathematics/제1코사인법칙.png)
* 제1 코사인법칙은 매우 직관적이다
  * $a = b\cos C + c\cos B$

<br/>
* 제1 코사인법칙으로부터
  <p> $$
    \begin{align*}
      a^2 = ab \cos C + ca \cos B, b^2 = bc \cos A + ab \cos C, c^2 = ca \cos B + bc \cos A \\
      a^2-b^2-c^2 &= -2bc \cos A \\
      a^2&=b^2+c^2 -2bc \cos A
    \end{align*}
  $$ </p> <br/>

  수식놀음이다.
  
<br/>
#### 헤론의 공식
이걸 증명해야하나 싶긴한데
* $S=\frac{1}{2}bc \sin A$
* $\sin^2 A = 1-\cos^2 A = (1+\cos A)(1-\cos A)이고 \cos A=\frac{b^2+c^2-a^2}{2bc}$이다.
* 쑤셔넣고 정리하면 $\sin A=\frac{2}{bc}\sqrt{s(s-a)(s-b)(s-c)} (2s=a+b+c)$라서 증명된다.

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_삼각함수공식" %}

순열과 조합은 확통 가서 다시 정리함

{% comment %}

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
