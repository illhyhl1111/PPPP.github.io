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
[머릿글](https://illhyhl1111.github.io/posts/first-post/)에서 설명했듯이,  
이 글은 읽는이가 해당 내용을 한번쯤은 공부해봤다는 가정 하에, 회고를 위하여 작성한 요약글입니다.  
모르는 부분은 '이런 개념이 있구나' 정도로만 이해하시고, 링크된 글을 읽으시거나 구글링하여 직접 찾아보십시오.  
기본적으로 목차는 **책 기준**으로 분류됩니다. 책 밖에껀 싸그리 기타 항목에 넣을거임ㅎㅎ

아직 작성이 많이많이많이많이매우많이 덜 되었습니다.  
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
### 조건
* 조건에 포함된 변수 $x$는 $U \neq \varnothing$ 을 정의역으로 함.
* 전체집합 $U$에서의 조건 $p(x)$를 간단히 조건 $p$라고 표기함.
* $U$의 원소 $a$를 대입한 $p(a)$가 참인 명제라면, 명제 $p(a)$가 성립한다, $a$는 조건 $p(x)$를 만족한다 라고 함.

<br/>

### 부정
* 명제 $p$ 혹은 조건 $p(x)$에 대해 $p(x)$가 아니다 를 $p(x)$의 부정이라 하고, $\sim p(x)$$로 표기함.

<p> $$ \sim (p \vee q) \Leftrightarrow (\sim p \wedge \sim q), \sim (p \wedge q) \Leftrightarrow (\sim p \vee \sim q) $$ </p>
<p> $$ \sim (\forall x, p(x)) \Leftrightarrow (\exists x, \sim p(x)), \sim (\exists x, p(x)) \Leftrightarrow (\forall x, \sim p(x))$$ </p>

<br/>

### 진리집합
* $p(x)$를 만족하는 $x$ 전체의 집합 $P$를 조건 $p(x)$의 진리집합이라고 한다.
* $P = \left\\{ x \mid x \in U, p(x) \right\\}$. 표기시 전체집합 $U$를 씹으려는 경향이 강하므로 $P=\left\\{ x \mid p(x) \right\\}$로도 표기.

<br/>

### 조건과 집합
* 집합 $P$, $Q$를 조건 $p$, $q$의 진리집합이라고 둘 때,

<p> $$ P \subset Q \Leftrightarrow (p \Rightarrow q), P \nsubseteq Q \Leftrightarrow (p \nLeftarrow q), \\
p \vee q \Leftrightarrow P \cup Q, p \wedge q \Leftrightarrow P \cup Q, \sim p \Leftrightarrow P^c $$ </p>

### 필요 · 충분 조건
* $p \Rightarrow q$일 때, $p$는 $q$이기 위한 충분조건이고 $q$는 $p$이기 위한 필요조건이 된다.
* $p \Leftrightarrow q$ 면 서로 필요충분조건(동치).
* 집합과의 관계는 $P \subset Q \Rightarrow (p \Rightarrow q) $

<br/>

### 귀류법
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
### 일반적 연산
* 집합 $M$의 두 원소 $a$, $b$의 순서쌍 $(a, b)$에 대응하는 $M$의 원소 $c$가 하나 정해질 때,
이 대응을 집합 $M$의 이항연산 또는 연산이라고 함.
* 기호 $\circ$ 등을 써서 $a \circ b = c$ 등으로 표기.
* 연산 $\circ$이 정의되어 있는 집합 $M$의 부분집합 $N$에 대하여, <br/>
  $a \in N, b \in N \Rightarrow a \circ b \in N$ 이면 $N$은 $\circ$에 관하여 닫혀 있다라고 함.

<br/>

### 교환, 결합법칙
* 교환법칙이 성립 $ \Leftrightarrow a \circ b = b \circ a $
* 결합법칙이 성립 $ \Leftrightarrow (a \circ b) \circ c = a \circ (b \circ c) $

<br/>

### 항등원, 역원
* $\forall a \in N, \exists e \in N, a \circ e = e \circ a = a$ 일 때 $e$를 $\circ$에 대한 항등원이라고 함
* $\forall a \in N, \exists x \in N, a \circ x = x \circ a = e$ 일 때 $x$를 $\circ$에 대한 역원이라고 함
{% endcapture %}

{% capture context2 %}
* 이후에 다루겠지만, 어떤 집합 $M$에 포함된 원소들이 어떤 연산 $\circ$에 대하여 결합법칙이 성립하고 항등원, 역원이 존재하면,
$M$은 $\circ$에 대하여 군(Group)을 이룬다고 한다. <br/>
* 교환법칙까지 성립하는 군을 아벨 군(abelian group), 혹은 가환군(commutative group)이라 한다.     

{% comment %}
https://m.blog.naver.com/PostView.nhn?blogId=obrigadu&logNo=50098477517&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F
{% endcomment %}

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_실수체계" %}

### 정수 문제
* 최대공약수(GCD)와 최소공배수(LCM),
* 유클리드 호제법 $A=BQ+R \Rightarrow \gcd(A, B) = \gcd(B, R)$

{% capture context1 %}
### GCD, LCM
* 두 개 이상의 정수의 공통인 약수를 공약수라 하고, 그 중 가장 큰 수를 최대공약수라 함
* 두 개 이상의 정수의 공통인 배수를 공배수라 하고, 그 중 가장 큰 수를 최소공배수라 함

* $\gcd(A, B) = G, \mathrm{lcm}(A, B) = L$이라 두면, <br/>
  $A = Ga, B = Gb$ (단, $\gcd(a, b) = 1$) <br/>
  $L = Gab, LG = AB$ 를 만족함.

<br/>

### 다항식의 GCD, LCM
* 다항식 $A$, $B$, $Q$ 사이에 $A=B \cdot Q$이면 $B$를 $A$의 약수라고 표현한다.
* 2개 다항식 사이 공통인 약수를 공약수, 가장 차수가 높은 것을 최대공약수라고 함.
* 배수도 똑같
* 정수에서와 똑같은 성질을 가짐

<br/>

### 유클리드 호제법 (Euclidean algorithm)
* 맨날까먹음
* $A > B$인 임의의 자연수 $A$, $B$가 있을 때, $A = B \cdot Q + R$로 몫과 나머지를 분리하면 </br>
  <p> $$\gcd(A, B) = \gcd(B, R)$$ </p>
  임이 성립한다는 것

* 이를 확장한 Extended Euclidian Algorithm은 다음과 같다 <br/>
  <p align="center"> $as + bt=\gcd(a,b)$ 인 정수쌍 $s$, $t$가 존재함 </p>
  모듈러 연산의 역원을 구하는데 우려먹힌다.

<br/>

### 기수법
* 양의 정수 $N_p = a_n p^n + a_{n-1} p^{n-1} + \cdots + a_1 p + a_0$
* 양의 소수 $N_p = \frac{a_1}{p} + \frac{a_2}{p^2} + \cdots + \frac{a_n}{p^n}$
{% endcapture %}

{% capture context2 %}
### Euclidean algorithm으로 gcd 찾기
<p> $$r_0 \leftarrow a, r_1 \leftarrow b \\
r_{i+1}=r_{i−1}−q_i r_i, \quad q_i=\frac{r_{i−1}}{r_i} $$ </p>

만약 $r_{i+1}=0$ 이라면 $r_i$ 가 바로 $\gcd(a,b)$ 이다.

<br/>

### Euclidean algorithm 증명
* $A=Ga, B=Gb$ ($a$, $b$ 는 서로소) 를 $A=BQ+R$에 대입해보면
<p> $$Ga=Gb \cdot Q + R, \quad R=G(a-Qb) $$ </p>
* 이제 $b$와 $a-Qb$가 서로소임을 보이면 되는데, $b=mk$, $a-bQ=mk'$으로 두자($k$, $k'$는 서로소)
* $a=bQ+mk'=m(kQ+k')$이므로 $m$은 $a$, $b$의 공약수인데, 서로소이므로 1임
* 따라서 $m=1$이 되며 $b$와 $a-Qb$는 서로소가 되서 $\gcd(B, R)=G$가 되어버림

<br/>

### Extended Euclidean algorithm 증명
* $r_0 \leftarrow a, r_1 \leftarrow b$
* 초기값들을 넣으면 $as_i+bt_i=r_i \quad for \; i=0,1$
* 이제 $i>1$일 때 참이라고 가정하고 수학적 귀납법을 쓰면

<p> $$r_{i+1}=r_{i−1}−r_i q_i=(as_{i−1}+bt_{i−1})−(as_i+bt_i)q_i=a(s_{i−1}−s_i q_i)+b(t_{i−1}−t_i q_i)=as_{i+1}+bt_{i+1} $$ </p>

* 따라서 $r_{i+1}=0$ 일 때 $as_i+bt_i=r_i$ 는 $as+bt=\gcd(a,b)$ 가 된다.

* [Extended Euclidean algorithm 증명](https://codeonwort.tistory.com/295) 참조

{% endcapture %}
{% include blocks.html context1=context1 context2=context2 topic="고등수학_Euclidean_alg" %}

### 다항식의 사칙연산, 인수분해, 항등식과 미정계수법
$(a-b)(a^2+ab+b^2)=a^3-b^3$같은 공식 수십개 - 응 안적어 <br/>
조립제법으로 다항식 인수분해

{% capture context1 %}
### 조립제법
$x$의 다항식 $F(x)$를 $x-a$로 나누었을 때 몫과 나머지로 분리하는 방법.<br/>
![Alt text](/pictures/mathematics/690b6a0d.png)
{% endcapture %}

{% capture context2 %}
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_조립제법" %}

### 나머지정리
$x$의 다항식 $f(x)$를 $x-a$로 나누었을 때 나머지는 $f(a)$이다.

{% capture context1 %}
* $f(a)=0$인 것과 $f(x)$가 $x-a$로 나누어떨어진다는 동치이다.
* 보통 $f(a)=0$인 $a$를 찾아서 $f(x)$를 인수분해하려고 쓴다.
* $f(x)=ax^n+ \cdots + b$꼴일 때에는 $x= \pm \frac{b의 약수}{a의 약수}$ 를 대입해본다.
{% endcapture %}

{% capture context2 %}
$f(x) = (x-a)Q(x) + R$는 항등식이므로, $R = f(a)$
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_나머지_정리" %}

### 이차방정식
<p> $$
  \begin{align*}
    ax^2 + bx + c = 0 \Rightarrow & x = \left(-b \pm \frac{\sqrt{b^2-4ac}}{2a}\right) \\
    ax^2 + 2bx + c = 0 \Rightarrow & x = \left(-b \pm \frac{\sqrt{b^2-ac}}{a}\right) \\
    D(\mathrm{Determinant}) = & b^2 -4ac
  \end{align*}
$$ </p>

### 점과 좌표
* 선분의 내분점과 외분점 $\dfrac{mx_2 \pm nx_1}{m+n}$
* Pappus의 정리, 삼각형의 무게중심 등등 잡다한 것들

{% capture context1 %}
### 선분의 내분점과 외분점
* $\overline{AB}$를 $m:n$으로 내분하는 점 $P$의 좌표는 $\dfrac{mx_2+nx_1}{m+n}$
* $\overline{AB}$를 $m:n$으로 외분하는 점 $P$의 좌표는 $\dfrac{mx_2-nx_1}{m-n}$

<br/>

### 삼각형의 무게중심, Pappus의 정리
* $A(x_1, y_1), B(x_2, y_2), C(x_3, y_3)$인 $\triangle ABC$의 무게중심은
<p> $$\left(\frac{x_1+x_2+x_3}{3}, \frac{y_1+y_2+y_3}{3}\right)$$ </p>
<br/>

![Alt text](/pictures/mathematics/27755D4256A82ED122.png)
* $\triangle ABC$ 의 변 $\overline{BC}$의 중점을 $M$이라 둘 때,
$\overline{AB}^2 + \overline{BC}^2 = 2(\overline{AM}^2 + \overline{BM}^2)$
{% endcapture %}

{% capture context2 %}
* 삼각형의 무게중심 $G$는 점 $A(x_1, y_1)$와 $\overline{BC}$의 중점 $M\left(\frac{x_2+x_3}{2}, \frac{y_2+y_3}{2}\right)$를 $2:1$로 내분하는 점. <br/>
  나머지 변에 대해서도 마찬가지.

* 파푸스 정리는 그냥 위에 넣은 그림대로 좌표넣고 계산때려보면 $2(a^2+b^2+c^2)$로 같다.
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_점과_좌표" %}

### 직선의 방정식
* 표준형 $y=ax+b$, 일반형 $ax+by+c=0$, 기울기+점, 두 점, $x$ $y$절편이 주어졌을 때 식 등등
* 점과 직선 사이의 거리 $d=\frac{\left\|ax_1+by_1+c\right\|}{\sqrt{a^2+b^2}}$

{% capture context1 %}
### 방정식
* 표준형: $y=ax+b$
* 일반형: $ax+by+c=0$
* 기울기+점: $y-y_1=m(x-x_1)$
* 두 점: $y-y_1=\frac{y_2-y_1}{x_2-x_1}(x-x_1)$
* $x$ $y$절편: $\frac{x}{a}+\frac{y}{b}=1$ <br/>
* 두 직선 $ax+by+c=0$, $a'x+b'y+c'=0$의 교점을 지나는 직선들의 방정식 <br/>
  $m(ax+by+c) + (a'x+b'y+c') = 0$

<br/>

### 수직인 직선
* $y=ax+b$, $y=a'x+b'$이 수직이라면, $aa'=-1$

<br/>

### 점과 직선 사이의 거리
* 점$(x_1, y_1)$과 직선 $ax+by+c=0$ 사이의 거리 $d=\frac{\left\|ax_1+by_1+c\right\|}{\sqrt(a^2+b^2)}$
{% endcapture %}

{% capture context2 %}
### 서로 수직인 두 직선
* $y=ax+b, y=a'x+b'$이 수직이라면, <br/>
  $\tan(\theta_1)=a, \tan(\theta_2)=\tan(\theta_1+\frac{\pi}{2})=-\frac{1}{\tan(\theta_1)}=a'$ <br/>
  $ \therefore a'=-\frac{1}{a}, aa'=1 $

<br/>

### 점과 직선 사이의 거리
* 점 $P$와 직선 $l$ 사이의 거리는, $P$에서 $l$로 내린 수선의 발 $Q(x', y')$과 $P$ 사이의 거리와 같음. <br/>
  <p> $$d^2 = (x'-x_1)^2+(y'-y_1)^2$$ </p>
* $P$를 지나 $l$에 수직인 직선의 방정식은 $y-y_1=\frac{b}{a}(x-x_1), b(x-x_1)-a(y-y_1)=0$ <br/>
  위 식과 $ax+by+c=0$에 $x=x', y=y'$을 대입하고 소거하여 $x'-x_1, y'-y_1$을 구하면 $d^2$을 구할 수 있다.
* 하면된다
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_직선" %}
 
### 원의 방정식
* 표준형 $(x-a)^2+(y-b)^2=r^2$, 일반형 $x^2+y^2+Ax+By+C=0$
* 접선의 방정식 $(x_1-a)(x-a)+(y_1-b)(y-b)=r^2, y-b=m(x-a)\pm r \sqrt{m^2+1}$
* 원과 직선의 교차, 두 원의 교차판별 등등

{% capture context1 %}
### 방정식
* 표준형: $(x-a)^2+(y-b)^2=r^2$
* 일반형: $x^2+y^2+Ax+By+C \rightarrow$
  * 중심$\left(-\frac{A}{2}, -\frac{B}{2}\right)$, 반지름 $\frac{\sqrt{A^2+B^2-4C}}{2}$
  * $A^2+B^2-4C<0$ 이면 허원 이라고도 한단다.
* 세 점을 지나는 원: 일반형에 세 좌표 쑤셔넣고 연립

<br/>

### 원과 직선의 관계
* 직선은 $y=mx+n$이요 원은 $f(x, y)=0$이기 때문에, <br/>
  $y$를 소거하여 $f(x, mx+n)$으로 해버리면 이차방정식이 되어버림. <br/>
  이때 판별식 $D$에 따라서 두 실근, 중근, 두 허근으로 나뉜다. <br/>

* 표준형의 원 위의 점$(x_1, y_1)$에서의 접선의 방정식은
  <p> $$(x_1-a)(x-a)+(y_1-b)(y-b)=r^2$$ </p>
* 기울기가 $m$인 접선의 방정식은
  <p> $$y-b=m(x-a)\pm r \sqrt{m^2+1}$$ </p>

<br/>

### 두 원의 관계
* 서로 만나는 두 원 $x^2+y^2+Ax+By+C=0$, $x^2+y^2+A'x+B'y+C'=0$ 의 교점을 지나는 원의 방정식은 <br/>
  $(x^2+y^2+Ax+By+C)m + (x^2+y^2+A'x+B'y+C') = 0$ 이며  <br/>
* $m=-1$ 이라서 이차항을 조져버리면 두 원의 공통현의 방정식이 되버린다.
{% endcapture %}

{% capture context2 %}
### 접선의 방정식
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
### 평행이동
* $x$축으로 $a$, $y$축으로 $b$만큼 평행이동시킬 때, $T: (x, y) \rightarrow (x+a, y+b)$로 표기하고
* 점 $P(x, y) \rightarrow Q(x+a, y+b)$
* 도형의 방정식 $f(x-a, y-b)=0 \rightarrow f(x-a, y-b)=0$

<br/>

### 대칭이동
* $x$축 - $T: (x, y) \rightarrow (x, -y)$
* $y$축 - $T: (x, y) \rightarrow (-x, y)$
* 원점 - $T: (x, y) \rightarrow (-x, -y)$
* $y=x$ - $T: (x, y) \rightarrow (y, x)$

{% endcapture %}

{% capture context2 %}
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_평행이동" %}

### 함수
* 함수의 정의, 정의역, 공역, 치역
* 일대일 함수, 일대일 대응, 항등함수, 상수함수, 합성함수 등등 잡다한 정의들

{% capture context1 %}
### 함수의 정의
* 두 집합 $X, Y \neq \varnothing$ 이 있을 때,
$X$의 각 원소에서 $Y$의 원소로의 대응을 $X$에서 $Y$로 가는 함수라고 정의하고 $f: X \longrightarrow Y$로 표기함
* 이때 함수 $f$에 대하여 $x \in X$에 $y \in Y$가 대응되는 것을 $f: x \longrightarrow y$, $y=f(x)$ 등으로 나타냄.
* $x$를 독립변수, $y$를 종속변수라고도 한단다.
* 아무튼 하나의 x에 대해서 반드시 하나의 y가 대응되어야 한다는게 중요함

<br/>

### 정의역, 공역, 치역
![Alt text](/pictures/mathematics/250F12365368EBE529.jpg)

<br/>

### 함수의 종류
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

### 합성함수
* 두 함수 $f: X \longrightarrow Y$, $g: Y \longrightarrow Z$일 때, $g(f(x))$는 정의역이 $X$이고 공역이 $Z$가 된다.
* 함성함수 $g \circ f$는 $g \circ f: x \longrightarrow g(f(x)), \; (g \circ f)(x) = g(f(x))$

{% endcapture %}

{% capture context2 %}
### 합성함수와 Group의 성질
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
### 유리수
* $k$에 따른 $y=\frac{k}{x}$ <br/>
![Alt text](/pictures/mathematics/캡처2.JPG)

* $n, m$이 주어진 $y=\frac{k}{x-m}+n$ <br/>
![Alt text](/pictures/mathematics/캡처3.JPG)

* $k, k'$에 따른 $y=k'x+\frac{k}{x}$ <br/>
![Alt text](/pictures/mathematics/캡처1.JPG)

킹갓구글에서 그래프까지 그려주는줄은 몰랐읍니다 충성충성

<br/>

### 무리함수
* $y^2=ax, y=\pm \sqrt{\pm ax}$ <br/>
![Alt text](/pictures/mathematics/캡처4.JPG) <br/>
  정의역과 치역을 좀 생각해야된다.

<br/>

### 역함수
* 역함수의 정의를 위해선, $f:X \longrightarrow Y$에서 $Y$의 임의의 한 원소에 $X$의 원소가 하나씩만 대응되어야 하기 때문에 일대일 대응이어야 함. <br/>
* $y=f(x) \Leftrightarrow x=f^{-1}(y)$
* 함수 $f$가 일대일 대응이면 역함수 $f^{-1}$은 존재한다 (존재성)

<br/>

### 역함수의 성질
* $(f^{-1})^{-1} = f$
* $f^{-1}(f(x))=x \quad (f^{-1} \circ f = I_x)$
* $f(f^{-1}(y))=y \quad (f \circ f^{-1} = I_y)$
* $f:X \longrightarrow Y, g:Y \longrightarrow X$에서 $g \circ f = I_x, f \circ g = I_y \Leftrightarrow g=f^{-1}$ (유일성)
* 일대일 대응 $f:X \longrightarrow Y, g:Y \longrightarrow Z$에 대하여  $(g \circ f)^{-1} = f^{-1} \circ g^{-1}$ <br/>

* 역함수의 기하학적 성질로, $y=f(x)$ 그래프와 $y=f^{-1}(x)$는 $y=x$에 대하여 대칭이다. <br/>
![Alt text](/pictures/mathematics/역함수.JPG)

{% endcapture %}

{% capture context2 %}
### 역함수 증명
* 존재성, 유일성 - TODO <br/>

* $(g \circ f)^{-1} = f^{-1} \circ g^{-1}$ 증명
  <p> $$(f^{-1} \circ g^{-1}) \circ (g \circ f) = f^{-1} \circ (g^{-1} \circ g) \circ f = f^{-1} \circ I \circ f = f^{-1} \circ f = I \\
        (g \circ f) \circ (f^{-1} \circ g^{-1}) = g \circ (f \circ f^{-1}) \circ g^{-1} = g \circ I \circ g^{-1} = g \circ g^{-1} = I \\
        \therefore (g \circ f)^{-1} = f^{-1} \circ g^{-1}$$ </p>
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_함수2" %}

### 최대와 최소
* 산술평균 $\geq$ 기하평균 $\geq$ 조화평균 ==> $\frac{a+b}{2} \geq \sqrt{ab} \geq \frac{2}{\frac{1}{a}+\frac{1}{b}}$, 등호는 $a=b$
* 코시-슈바르츠 부등식 $(a^2+b^2)(x^2+y^2) \geq (ax+by)^2$, 등호는 $\frac{a}{x}=\frac{b}{y}$

{% capture context1 %}
### 판별식을 이용한 최대, 최소
* $y=ax^2+bx+c$에서 $y$의 범위는 $0=ax^2+bx+(c-y)$에서 $D>=0$를 사용해도 됨

<br/>

### 산술기하조화
* 일반적인 형태로,
<p> $$ \frac{x_1 + x_2 + \cdots + x_n}{n} \geq \sqrt[n]{x_1 x_2 \cdots x_n} \geq \frac{n}{\frac{1}{x_1}+\frac{1}{x_2}+ \cdots + \frac{1}{x_n}} $$ </p>
* $n=2$일 때 증명은 쉽다. 하지만 $n$항으로 일반화하면...

![Alt text](/pictures/mathematics/산술기하조화.jpg){: width="40%" height="40%"}  <br/>
$n=2$일 때 증명은 너무 쉽다고 심지어 그림으로 농락하는것도 있다...

<br/>

### 가중 산술-기하 평균 부등식
* 각 항 앞에 가중치를 더한 부등식이다.
* 가중 산술-기하 평균 부등식은
<p> $$ \frac{\alpha_1 x_1 + \cdots + \alpha_n x_n}{\alpha} \geq \sqrt[\alpha]{x_1^{\alpha_1} \cdots x_n^{\alpha_n}} \\
       (x_i>0, \alpha_i>0) $$ </p>

<br/>

### 코시-슈바르츠 부등식
* 일반식은
  <p> $$ (a_1^2+a_2^2+\cdots+a_n^2)(x_1^2+x_2^2+\cdots+x_n^2) \geq (a_1x_1+a_2x_2+\cdots+a_nx_n)^2 $$ </p>
* 아예 제곱항도 $p$로 일반화시키면 [횔더 부등식](http://mathseodang.com/220450030140)이 된다
  <p> $$ \left(\sum_{i=1}^{n} {a_i^p}\right)^{1/p}\left(\sum_{i=1}^{n} {b_i^q}\right)^{1/q} \geq \sum_{i=1}^{n} {a_i b_i} \\
         p>1, q>1, \frac{1}{p}+\frac{1}{q}=1, \; equality \quad iff \quad a_i^p=\lambda b_i^q $$ </p>

{% endcapture %}

{% capture context2 %}
### 젠센 부등식
먼저 볼록 함수의 정의부터 살펴보자

#### 볼록 함수(convex function)
* 함수 $f:X\longrightarrow R$가 다음을 만족하면 볼록 함수로 부름 <br/>
  ![Alt text](/pictures/mathematics/볼록.png)
  <p> $$ \forall x_1, x_2 \in X, \forall t \in [0, 1]: f(tx_1+(1-t)x_2) \leq tf(x_1)+(1-t)f(x_2) $$ </p>
* 등호를 빼면 strictly convex function 이다.

----------------

* 머암튼 $f:(a,b) \longrightarrow R$가 연속인 볼록 함수라면, 젠센 부등식은
  <p> $$ \forall x_i \in (a, b), p_i > 0, \sum_{i=1}^{n} {p_i} = 1 \; 일 \, 때 \; f\left(\sum_{i=1}^{n} {p_i x_i}\right) \leq \sum_{i=1}^{n} {p_i f(x_i)} $$
* 증명은 [수학적 귀납법](http://suhak.tistory.com/221)으로.

<br/>

### (가중) 산술기화조화 증명
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

### 코시-슈바르츠 부등식 증명
* [별별 증명법](https://m.blog.naver.com/yh6613/220458975310)이 다 있다.
* 귀찮은 기념으로 간단하게만 설명하면
  * $let \; A=\sqrt{a_1^2+a_2^2+\cdots+a_n^2}, \; B=\sqrt{b_1^2+b_2^2+\cdots+b_n^2}$
  * 산술 기화평균 부둥식에 따라 <br/>
    $\sqrt{\dfrac{a_i^2}{A^2} \dfrac{b_i^2}{B^2}} \leq \dfrac{1}{2}\left(\dfrac{a_i^2}{A^2}+\dfrac{b_i^2}{B^2}\right)$
  * 이걸 $i=1$ 부터 $n$에 대한 부등식을 모두 더하면 우변은 1이 되고, 결국 $\sum\limits_{i=1}^{n} {\sqrt{a_i^2 b_i^2}} \leq AB$로 증명된다. <br/>

<br/>
* [재배열 부등식](https://namu.wiki/w/%EC%9E%AC%EB%B0%B0%EC%97%B4%20%EB%B6%80%EB%93%B1%EC%8B%9D) 도 볼만함

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_최대와_최소" %}

### 삼각함수의 정의
* 호도(radian)법: $l=r\theta, \; S=\frac{1}{2}r^2\theta=\frac{1}{2}rl, \; 1\,rad = \frac{180\degree}{\pi}$
* 이 때 $P(x,y)$와 $\theta=\angle xOP$에 대하여, $\sin\theta=\frac{y}{r}, \; \cos\theta=\frac{x}{r}, \; \tan\theta=\frac{y}{x}$이라 정의함

{% capture context1 %}
### 부채꼴의 넓이
* $l=r\theta$ 인건 $\theta$의 radian 정의임 $\left(\frac{l}{2\pi r}=\frac{\theta}{2\pi}\right)$
* 이 때 $\frac{S}{\pi r^2} = \frac{\theta}{2\pi}$에서 $S=\frac{1}{2}r^2\theta$

<br/>

### 웃겨서 넣어봤다
![Alt text](/pictures/mathematics/8177-2-7693.gif){: width="40%" height="40%"} <br/>
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
* $\tan\theta = \dfrac{sin\theta}{\cos\theta}$
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
### 사인법칙
#### 원주각
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

### 코사인 법칙
![Alt text](/pictures/mathematics/제1코사인법칙.png)
* 제1 코사인법칙은 매우 직관적이다
  * $a = b\cos C + c\cos B$

<br/>
* 제1 코사인법칙으로부터
  <p> $$
    \begin{align*}
      a^2 = ab \cos C + ca \cos B, b^2 &= bc \cos A + ab \cos C, c^2 = ca \cos B + bc \cos A \\
      a^2-b^2-c^2 &= -2bc \cos A \\
      a^2&=b^2+c^2 -2bc \cos A
    \end{align*}
  $$ </p> <br/>

  수식놀음이다.

<br/>

### 헤론의 공식
이걸 증명해야하나 싶긴한데
* $S=\frac{1}{2}bc \sin A$
* $\sin^2 A = 1-\cos^2 A = (1+\cos A)(1-\cos A)이고 \cos A=\frac{b^2+c^2-a^2}{2bc}$이다.
* 쑤셔넣고 정리하면 $\sin A=\frac{2}{bc}\sqrt{s(s-a)(s-b)(s-c)} (2s=a+b+c)$라서 증명된다.

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_삼각함수_공식" %}

순열과 조합은 확통 가서 다시 정리함

## 수학 1

### 행렬
* $A=(a_ij)=\begin{pmatrix} a_{11} & a_{12} \\\\ a_{21} & a_{22} \end{pmatrix}$
* $A \times B = \begin{pmatrix} a_{11}b_{11}+a_{12}b_{21} & a_{11}b_{12}+a_{12}b_{22} \\\\ a_{21}b_{11}+a_{22}b_{21} & a_{21}b_{12}+a_{22}b_{22}\end{pmatrix}$
* $A^{-1}=\dfrac{1}{a_{11} a_{22}-a_{12} a_{21}}{\begin{pmatrix} a_{22} & -a_{12} \\\\ -a_{21} & a_{11} \end{pmatrix} }$

{% capture context1 %}
### 행렬의 정의
* 수 또는 문자를 직사각형 형태로 배열하여 괄호로 묶어낸 것.
* 가로 줄을 행이라 하고, 세로 줄을 열이라 할 떄, $m$개 행, $n$개 열로 이루어진 행렬을 $m \times n$ 행렬이라 함
* $n \times n$은 정사각행렬

<br/>

### 행렬의 연산
$A=\begin{pmatrix} a_{11} & a_{12} \\\\ a_{21} & a_{22} \end{pmatrix}, B=\begin{pmatrix} b_{11} & b_{12} \\\\ b_{21} & b_{22} \end{pmatrix}$일 때
* $A=B \Leftrightarrow a_{ij} = b_{ij}$
* $A+B=\begin{pmatrix} a_{11}+b_{11} & a_{12}+b_{12} \\\\ a_{21}+b_{21} & a_{22}+b_{22}\end{pmatrix}$
* $A-B=\begin{pmatrix} a_{11}-b_{11} & a_{12}-b_{12} \\\\ a_{21}-b_{21} & a_{22}-b_{22}\end{pmatrix}$
* $kA=\begin{pmatrix} ka_{11} & ka_{12} \\\\ ka_{21} & ka_{22}\end{pmatrix}$ <br/>

* ![Alt text](/pictures/mathematics/274D6B4152FB2FB105.png) <br/>
* $A \times B = \begin{pmatrix} a_{11}b_{11}+a_{12}b_{21} & a_{11}b_{12}+a_{12}b_{22} \\\\ a_{21}b_{11}+a_{22}b_{21} & a_{21}b_{12}+a_{22}b_{22}\end{pmatrix}$
* 일반적으로, $A \times B = (AB_{ij}) = \left(\sum\limits_{k} {a_{ik}b_{kj}}\right)$ <br/>

* $O$: 모든 성분이 0인 행렬
* $I_n = (I_{n,ij})$, $I_{n,ij}= \begin{cases} 1 & \text{if }i = j \\\\ 0 & \text{else} \end{cases}$ 인 $n$차 정사각행렬

<br/>

### 역행렬
$n$차 정사각행렬 $A$에 대하여, $XA=AX=I_n$ 인 행렬 $X$가 존재할 때, 행렬 $X$를 $A$의 역행렬이라 하고 $A^{-1}$로 나타냄
* $XA=I \Leftrightarrow X=A^{-1}, \; AX=I \Leftrightarrow X=A^{-1}$
* $I^{-1} = I$
* $(A^{-1})^{-1}=A$
* $(AB)^{-1}=B^{-1}A^{-1}$
* $(kA)^{-1}=\frac{1}{k}A^{-1}$
* $(A^n)^{-1}=(A^{-1})^n$ <br/>

* 이차 정사각행렬 $A$에 대해서 $A^{-1}=\dfrac{1}{a_{11} a_{22}-a_{12} a_{21}}{\begin{pmatrix} a_{22} & -a_{12} \\\\ -a_{21} & a_{11} \end{pmatrix} }$
* 일반항은 다음 단계에

<br/>

### 연립일차방정식과 행렬
* $\begin{cases} ax+by=p \\\\ cx+dy=q \end{cases} \Leftrightarrow
   \begin{pmatrix} a & b \\\\ c & d \end{pmatrix} \begin{pmatrix} x \\\\ y\end{pmatrix} = \begin{pmatrix} p \\\\ q \end{pmatrix}  \Leftrightarrow AX=B$
* 이때 $X=A^{-1}B$
* $A$의 역행렬이 존재하지 않는다면, 해는 없거나($a:c=b:d \neq p:q$) 무한함($a:c=b:d=p:q$)

<br/>

### 그래프와 행렬(Adjacency Matrix)
![Alt text](/pictures/mathematics/2453_1.JPG) <br/>
이 때 행렬 $A^n$의 성분 $A^n_{ij}$는 $n$번 이동하여 점 $i$에서 $j$로 이동할 수 있는 경로의 갯수

{% endcapture %}

{% capture context2 %}
### 행렬과 군
* 행렬을 원소로 하는 집합에서 덧셈은 교환, 결합법칙을 만족하고, 항등원 $O$와 역원 $-A$가 존재하므로 가환군이다.
* 정사각행렬을 원소로 하는 집합에서 덧셈은 교환법칙을 만족하고, 항등원 $I$가 존재하지만, 결합법칙은 만족하지 않고 역행렬은 없을수도 있는 [모노이드](https://ko.wikipedia.org/wiki/%EB%AA%A8%EB%85%B8%EC%9D%B4%EB%93%9C)이다.
  * [증명??](https://proofwiki.org/wiki/Square_Matrices_forms_Monoid)

<br/>

### 행렬의 곱셈은 대체 왜 저따구로 정의되었는가
<p> $$A \times B = (AB_{ij}) = \left(\sum\limits_{k} {a_{ik}b_{kj}}\right) $$ </p>
<br/>
$A+B=\begin{pmatrix}a_{11}+b_{11} & a_{12}+b_{12} \\\\ a_{21}+b_{21} & a_{22}+b_{22} \end{pmatrix}$라고 해놨는데 <br/>
$A \times B= \begin{pmatrix} a_{11}b_{11} & a_{12}b_{12} \\\\ a_{21}b_{21} & a_{22}b_{22} \end{pmatrix}$는 왜 아닌가 <br/>
<br/>
행렬을 배우면서 이러한 의문이 생기지 않는다면 공부를 매우 하기 싫었던 사람이었을것이다

------------------------

일단 $A \times B= \begin{pmatrix} a_{11}b_{11} & a_{12}b_{12} \\\\ a_{21}b_{21} & a_{22}b_{22} \end{pmatrix}$라고 생각해보자 <br/>
그럼 행렬의 존재 이유는? <br/>
그렇게 되면 여러 숫자를 하필이면 직사각형 형태로 엮어서 저장하는 쓰잘데기없는 숫자묶음 말고 더 의미가 있는가? <br/>
일단 수학 공부를 좀 하긴 한 사람이면 행렬의 존재 이유 자체가 이 곱셈연산의 방식에 있음을 여럼풋이 느낄 수 있을것이다. <br/>
그렇긴 한데 그래서 왜 저렇게 곱하는거냐고

------------------------

일단 2차원 평면상의 점 $(x, y)$가 있다고 치자. <br/>
그럼 이 점을 어딘가로 선형사상(linear transform) 시켜버리는 함수 $f:(x, y) \longrightarrow (ex+fy,\, gx+hy)$는 종종 중요하게 쓰인다. <br/>
그런 함수가 하나 더 있다고 치자. $g:(x, y) \longrightarrow (ax+by,\, cx+dy)$ <br/>
<br/>
그럼 점 $(x, y)$를 $f$로 한번 transform하고 $g$로 transform한 점 $g(f(x, y))$를 표현해보자.<br/>
<p> $$g(f(x,y)) = g(ex+fy,\, gx+hy) = ((ae+bg)x+(af+bh)y,\, (ce+dg)x+(cf+dh)y)$$ </p>
먼가 더럽다.<br/>
<br/>
또 이번엔 3차원 공간상의 점 $(x, y, z)$에 대한 선형사상을 생각해보자 <br/>
그럼 $f:(x, y, z) \longrightarrow (ax+by+cz,\, dx+ey+fz,\, gx+hy+iz), \quad g:(x,\, y,\, z) \longrightarrow ...$ <br/>
$g(f(x,\, y,\, z)) = ......$ <br/>
아 쓰기싫다. <br/>
<br/>
이렇게 선형사상을 함수로 써버리면 매우 꼴뵈기 싫은 부분이 몇개 생기는데,
* 첫번째로는 $f:(x,\, y) \longrightarrow (ex+fy,\, gx+hy), g:(x,\, y) \longrightarrow (ax+by,\, cx+dy)$ 등<br/>
  선형사상의 성질을 결정하는 것은 $a,\, b,\, c,\, d$와 같은 상수항인데 계속 $x,\, y$항을 써줘야 된다는것
* 두번째로는 2차원 평면이면 4개의 항을, 3차원 공간이면 9개의 항을, $n$차원 초평면이면 $n^2$개의 항을<br/>
  무려 한 line에다 다 때려박아야 된다는것

이런 안타까운 상황에서 옛날옛적 수학자들은 저러한 표현을 쓰다가 손이 좀 아팠을 것이다.

------------------------

손이 아파서 화가 난 수학자들은 아래 수식을 뻘하게 쳐다본다 <br/>
<p> $$f:(x,\, y,\, z) \longrightarrow (ax+by+cz,\, dx+ey+fz,\, gx+hy+iz)$$ </p>
여기서 $ax+by+cz,\, dx+ey+fz,\, gx+hy+iz$는 $f(x, y, z)$의 $x,\, y,\, z$축 항을 분리해서 쓴거다. <br/>
'그럼 야 $ax+by+cz$도 $x,\, y,\, z$축 항을 분리해서 $a,\, b,\, c$로 쓰면 되지 않겠느냐?' 하는 합리적 의심이 떠오른다

------------------------

그럼 이제 $f:(x, y) \longrightarrow (ex+fy,\, gx+hy), g:(x, y) \longrightarrow (ax+by,\, cx+dy)$를<br/>
<p> $$X= \begin{pmatrix} x \\ y \end{pmatrix}, F = \begin{pmatrix} e & f \\ g & h \end{pmatrix}, G = \begin{pmatrix}a & b \\ c & d \end{pmatrix}$$ </p>
와 같이 써보자. <br/>
그럼 이제 어떻게 $F$와 $X$를 합쳐서 $(ex+fy,\, gx+hy)$ 꼴이 나오게 할 것이고<br/>
또 어떻게 $G, F, X$를 합쳐서 $g(f(x,y)) = ((ae+bg)x+(af+bh)y,\, (ce+dg)x+(cf+dh)y)$ 꼴이 나오게 할 것인가<br/>
<br/>
여기서 수학자들은 뭔가 발견하는데 <br/>
$X, F, G$와 같은 점과 선형사상을 행렬이라고 정의하고, <br/>
행렬의 곱셈 연산을 $A \times B = (AB_{ij}) = \left(\sum\limits_{k} {a_{ik}b_{kj}}\right)$ 와 같이 정의한다면 <br/>
$f(x)$를 $F \times X$, <br/>
$g(f(x))$를 $G \times F \times X$, <br/>
$g \circ f$를 $G \times F$로 나타낼 수 있다는 것. <br/>
더 나아가 이는 임의의 $n$차원의 점과 사상에 대해서도 성립한다. <br/>
와 씐난다! <br/>
[이것이 바로 선형대수학 제일의 철학, ‘선형사상(=함수)은 행렬과 같다’ 는 말이다.](http://wiki.mathnt.net/index.php?title=%EA%B3%A0%EA%B5%90%EC%83%9D%EB%8F%84_%EC%9D%B4%ED%95%B4%ED%95%A0_%EC%88%98_%EC%9E%88%EB%8A%94_%EA%B5%B0%EB%A1%A0_%EC%9E%85%EB%AC%B8)

------------------------

아무튼, $AB_{ij} = \sum\limits_{k} {a_{ik}b_{kj}}$같은 정의에 과연 어떤 해석이 가능하길래 점과 사상의 곱, 사상과 사상의 곱 모두에 적용이 되는가? <br/>
솔직히 잘 모르겠다. 나중에 알게되면 적어봄 <br/>
<br/>
그 밖에도, 그래프를 행렬로 표현하는 Adjacency matrix에서 곱셈의 의미 등 행렬의 곱셈 정의에는 기타 심오한 의미가 담긴 것으로 보인다.<br/>
아니면 선형사상을 표현하려고 행렬을 정의했는데 side effect로 여러 분야에서 먹힌걸수도 있고<br/>
더 공부해야됨<br/>

<br/>

### 일반적 역행렬
<p> $$ \begin{align} A^{-1} &= \frac{1}{\left|A\right|} adj(A) \\
\text{where }adj(A) &= [\bar{A_ij}]^t, \; \bar{A_ij} = (-1)^{i+j}\left|M_{ij}\right| \end{align}$$ </p>

어... 난감하다 <br/>
하나씩 보자

* $adj(A)$
  * Adjoint Matrix로써 위 정의 $adj(A) = [\bar{A_ij}]^t$ 를 따른다.

* $M_{ij}$
  * Minor matrix
  * 원래 행렬에서 $i$행 $j$열을 제거한 행렬. <br/>
    ![Alt text](/pictures/mathematics/4.jpg)
<br/>

* $\left\|A \right\|$
  * determinant
  * $\left\| A \right\| = \sum\limits_{j=1}^{n} {(-1)^{k+j}a_{kj}\left\| M_{kj} \right\|}$
    * 여기서 $k$는 아무 행이나 상관없다.
<br/>

뭐.. 역행렬의 선형대수학적 의미(역사상) 등 심오한 파트는 일단 [링크](https://m.blog.naver.com/PostView.nhn?blogId=at3650&logNo=221057878162&categoryNo=3)만 남긴다. <br/>
선형대수 할때 자세히 다룰 예정..

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학1_행렬" %}

### 지수, 로그
* $x^n=a$인 수 $x$를 $a$의 $n$제곱근이라 함. 이때 $a^{\frac{1}{n}}=x$
* $a>0$, $a\neq 1$일 때, 임의의 양수 $b=a^x \Leftrightarrow x=\log_{a}{b}$

![Alt text](/pictures/mathematics/로그함수.JPG) <br/>
![Alt text](/pictures/mathematics/로그함수2.JPG)

{% capture context1 %}

### 지수의 확장
1. 정수 범위로 확장
  * $0$이 아닌 실수 $a$에 대하여 $a^0=1$, $a^{-n}=\dfrac{1}{a^n}$

2. 유리수 범위로 확장
  * $a>0$에 대하여 $a^{\frac{m}{n}}=\sqrt[n]{m}$

3. 실수 범위로 확장
  * $a>0, b>0$에 대하여 $a^x a^y=a^{x+y}, \dfrac{a^x}{a^y} = a^{x-y}, (a^x)^y=a^{xy}, (ab)^x=a^x b^x$

<br/>

### 로그의 성질
$a>0$, $a\neq 1$, $x>0$, $y>0$일 때
* $\log_a{1}=0, \log_a{a}=1$
* $\log_a{xy}=\log_a{x}+log_a{y}, \log_a{\dfrac{x}{y}}=\log_a{x}-\log_a{y}$
* $\log_a{x^n}=n\log_a{x}$
* $\log_a{b}=\dfrac{\log_c{b}}{\log_c{a}}, \log_a{b}=\dfrac{1}{\log_b{a}}$

<br/>

### 지수함수와 로그함수
* $y=\log_a{x}$의 역함수는 $y=a^x$이기 때문에 둘은 $y=x$에 대칭임

{% endcapture %}

{% capture context2 %}

### 로그 성질 증명
$\log_a{xy}=\log_a{x}+log_a{y}$
* $\log_a{x}=m,\; \log_a{y}=n$이라 하면, $x=a^m,\; y=a^n,\; xy=a^{m+n}$에서 $\log_a{x}+\log_a{y}=m+n=\log_a{xy}$

<br/>

$\log_a{b}=\dfrac{\log_c{b}}{\log_c{a}}$
* $\log_a{b}=x$라 하면 $b=a^x, \; \log_c{b}=log_c{a^x}=x\log_c{a}, \; \log_a{b}=x=\dfrac{\log_c{b}}{\log_c{a}}$

<br/>

### 실수 범위로 지수의 확장
자연수에서만 정의되던 지수의 성질을 유지하면서 이를 확장해 나가보자.<br/>
기존의 연산 법칙을 유지시키면서 수 체계를 확장시키는 것을 **대수적 형식 불역의 원리**라고 한단다.

기존의 연산 법칙이 뭐냐 그럼<br/>
책에서 나오는 논리를 쌩까고 또 Group Theory를 가져와보자.

-------------------

#### Group isomorphism
Group isomorphism이란, $(G, \circ)$, $(H, *)$의 2개의 군이 있으면 <br/>
$\forall a, b \in G$에 대하여, $\phi(a \circ b) = \phi(a) * \phi(b)$ 를 만족하는 $\phi:G \longrightarrow H$,<br/>
즉 $G$의 원소를 $H$의 원소로 보내버리는 $\phi$를 (group) homomorphism이라 한다.

이때 $\phi$가 일대일 대응이면 $\phi$를 group isomorphism이라고 한다.
[링크](https://proofwiki.org/wiki/Definition:Isomorphism_(Abstract_Algebra)/Group_Isomorphism)

참고로 [Isomorphism](https://ko.wikipedia.org/wiki/%EB%8F%99%ED%98%95_%EC%82%AC%EC%83%81)(동형 사상)이란, <br/>
서로 구조가 같은 두 대상 사이에, 모든 구조를 보존하는 사상이라고 한다. <br/>
그러니까 어떤 구조 $X$를 함수 $f:X \longrightarrow Y$ 에 넣어서 $Y$가 됬어도, $Y$ 안에 $X$의 모든 정보가 담겨있다는 것이며 <br/>
달리 말하자면 $f^{-1}:Y \longrightarrow X$가 존재하며 $f$는 일대일 대응이다.

-------------------

일단 자연수로 시작한 지수의 정의에서, 지수함수 $\exp$는 다음 성질이 있다. (밑을 우선 $e$로 두었지만, 임의의 밑에 대해서 성립함)
<p> $$\forall x,y \in \mathbb{R}: \exp(x+y) = \exp(x) \cdot \exp(y) $$ </p>
이 기존 연산법칙을 유지하면서, 대수적 형식 불역의 원리에 맞춰 수 체계를 실수까지 확장해보자!

$(\mathbb{R}, +)$의 **additive group of real numbers**와, <br/>
$(\mathbb{R}_{>0}, \times)$의 **multiplicative group of positive real numbers**의 두 group을 생각해 보면, <br/>
함수 $\exp$는 누가 봐도 Group homomorphism이다. <br/>
다시 말하자면, 지수함수는 실수의 덧셈군을 양의 실수의 곱셈군으로 매칭시키는 함수가 된다.

이때, $\exp$가 단조증가함수라는 성질에 따라 $\exp$는 일대일 대응함수가 되며[증명](https://proofwiki.org/wiki/Strictly_Monotone_Function_is_Bijective) <br/>
$y=\exp(x)$의 그 역함수는 바로바로 $y=\ln(y)$가 된다. <br/>
그래서 $\exp$는 뭐다? group isomorphism이다.<br/>
(역으로, $\ln$ 함수도 group isomorphism이 된다. 아마?)

------------------------

이딴 얘기를 왜 하는가? Group isomorphism인데 뭐 어쩌라고 <br/>
일단 자연수 범위에서 지수함수 $a^n$이란 어떤 수 $a$를 $n$번 반복해서 곱하는거였다. <br/>
근데 이 정의만으론 $a^{\sqrt{2}}$ 같은걸 해석할 엄두가 안나는 것임. <br/>
결국 실수 범위에서도 납득이 가능한 정의를 찾고 싶은거다. <br/>

그래서 어떻게 이걸 해석했느냐? 하면 <br/>
자연수 범위에서 얻어낸 지수함수의 성질 $f(x+y) = f(x) \cdot f(y)$을 오히려 지수함수의 정의로 바꿔버린 것<br/>
그러니까 지수함수란 $f(x+y) = f(x) \cdot f(y)$을 만족하는 함수가 되도록 정의해버림.<br/>
그리고 위에서 정의한 Group isomorphism에 따라,<br/>
**지수함수는 (실수 덧셈식)을 (양의 실수 곱셈식)으로 매핑시키는 함수가 된다.**<br/>
예를 들면, $\exp$는 $(1+3=4)$을 $(2.718*20.086=54.598)$로 매핑시키는 함수로 정의되는 것

그런데 실수 덧셈식을 양의 실수 곱셈식으로 매핑하는 함수라니, 뭔가 너무 제한이 없다.<br/>
일단 한가지 조건 $f(x+y) = f(x) \cdot f(y)$이 있긴 한데, 이것만으로 함수를 특정짓기엔 부족하다.

그래서 여러 지수함수 중, $f(x)=2^x$를 $f(1)=2$을 만족하는 지수함수, $f(x)=3^x$을 $f(1)=3$을 만족하는 지수함수,<br/>
그리고 $f(x)=\exp(x)=e^x$를 $f(1)=e$를 만족하는 지수함수로 부른다.<br/>

이러한 조건을 만족하는 $f(x)$의 값은 유일하다!
- 증명 아이디어:
  * 일단 임의의 자연수 $n$에 대하여 $f\left(\frac{1}{n}\right)$이 유일함을 보일 수 있다 (아래의 $\exp(\frac{1}{3}) = \sqrt[3]{e}$ 부분과 같이)
  * 그럼 임의의 실수 $x$에 대해 위 조건을 만족하는 $f(x)=\alpha, \; \beta=\alpha+\epsilon(\neq 0)$ 2개의 값이 존재한다고 가정하자
  * 그럼 임의의 자연수 n에 대하여, <br/>
    $f\left(x-\frac{1}{n}\right)=\alpha \div f\left(\frac{1}{n}\right) < f(x) = \beta = \alpha+\epsilon < f\left(x+\frac{1}{n}\right) = \alpha * f\left(\frac{1}{n}\right)$
  * 근데 $\epsilon > 0$이라고 가정하면, <br/>
    $\alpha+\epsilon < \alpha * f\left(\frac{1}{n}\right), \; 1+\frac{\epsilon}{\alpha} < f\left(\frac{1}{n}\right)$ <br/>
    여기서 식은 임의의 자연수 $n$에 대해서 성립해야 하므로, $n$를 미친놈마냥 크게 두면 그딴 $\epsilon$은 존재하지 않음
  * $\epsilon < 0$일때도 마찬가지로 하면 된다. 아무튼 모순임.

----------------------

그러면 우선 $\exp(2)=\exp(1+1)=\exp(1) * \exp(1)=e * e$, $\exp(3)=\exp(2+1)=\exp(2) * \exp(1)=(e * e) * e $ 가 되고 <br/>
$\exp$는 additive group of **real** numbers의 집합을 정의역으로 하기 때문에, 당연히 $2+(-1)$ 같은 꼴도 허용이 되며,<br/>
$\exp(2+(-1))=\exp(1)= e$는 $\exp(2) * \exp(-1) = e*e * \exp(-1)$ 와 같으므로<br/>
$\exp(-1)=\dfrac{1}{e}$가 되고, $\exp(0)=\exp(1) \cdot \exp(-1)=1$이 된다.<br/>

$\frac{1}{3}+(\frac{1}{3}+\frac{1}{3})$도 $\exp$의 정의역으로 허용이 되기 때문에<br/>
$\exp(\frac{1}{3}+(\frac{1}{3}+\frac{1}{3})) = \exp(1)=e$ 는 $\exp(\frac{1}{3}) * (\exp(\frac{1}{3}) * \exp(\frac{1}{3}))$와 같으므로<br/>
$\exp(\frac{1}{3}) = \sqrt[3]{e}$가 된다.

$\exp(\sqrt{2})$ 역시 어떤 양의 실수 곱셈식으로 매핑될 것이며, 그 결과는 당연히 양의 실수이다.

-----------------

아무튼 설명이 길었는데, 요약하자면
1. 정의역 $X=\mathbb{R}$, 치역 $Y=\mathbb{R}_{>0}$을 가지는 지수함수 $f(x)$는,
2. $f(x+y)=f(x) \cdot f(y)$을 만족하도록 정의된, (실수들의 덧셈) $\longrightarrow$ (양의 실수들의 곱셈) 으로 매핑시키는 함수이고,
3. 그 중 $f(x)=a^x$는 $f(1)=a$을 만족하는 함수로 정의된다.

혼자서 공부한거라 이상한 부분이 있을수 있음

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학1_지수_로그" %}

### 수열
* 등차수열 $a_n=a+(n-1)d, S_n=\dfrac{n\{2a+(n-1)d\}}{2}$
* 등비수열 $a_n=ar^{n-1}, S_n=\dfrac{a(1-r^n)}{1-r}=\dfrac{a(r^n-1)}{r-1} (a\neq 1)$
* $\sum\limits_{k=1}^{n} {k^2} = \dfrac{n(n+1)(2n+1)}{6}, \quad \sum\limits_{k=1}^{n} {k^3} = \left\\{\dfrac{n(n+1)}{2}\right\\}^2$
* $\sum\limits_{k=1}^{n} {\dfrac{1}{k(k+1)}} = \sum\limits_{k=1}^{n} {\dfrac{1}{k} - \dfrac{1}{k+1}} = 1-\dfrac{1}{n+1}$
* $\sum\limits_{k=1}^{n} {\dfrac{1}{\sqrt{k} + \sqrt{k-1}}} = \sum\limits_{k=1}^{n} {\sqrt{k} - \sqrt{k-1}} = \sqrt{n}$

{% capture context1 %}
증명은 다음단계에
{% endcapture %}

{% capture context2 %}
### 등차수열의 합
* $S_n = a + (a+d) + (a+2d) + \cdots + \\{a+(n-1)d\\}$
* $S_n = \\{a+(n-1)d\\} + \\{a+(n-2)d\\} + \\{a+(n-3)d\\} + \cdots + a$
* $2S_n = \\{2a+(n-1)d\\} \times n, S_n = \frac{n\\{2a+(n-1)d\\}}{2}$

<br/>

### 등비수열의 합
* $S_n = a+ar+ar^2+\cdots\+ar^{n-1}$
* $rS_n= ar+ar^2+ar^3+\cdots\+ar^{n}$
* $(1-r)S_n=a-ar^n = a(1-r^n), \; S_n = \dfrac{a(1-r^n)}{1-r}=\dfrac{a(r^n-1)}{r-1} (r\neq 1)$

<br/>

### 자연수의 거듭제곱 합
* 일단 $\sum\limits_{k=1}^{n} {k} = \frac{n(n+1)}{2}$이다.
* 귀납적으로(더 정확히는 transfinite induction) $1$부터 $m-1$까지의 거듭제곱의 합 $\sum\limits_{k=1}^{n} {k^{m-1}} = S_{m-1}(n)$을 모두 알고 있다고 가정하자

<br/>

* $a_x = (x+1)^{m+1} - x^{m+1} = \sum\limits_{k=0}^{m} {_{m+1} C_k x^k}$ 으로 두면
<p>$$ \begin{align}
\sum\limits_{x=1}^{n} {a_x} &= (n+1)^m -1 = \sum\limits_{x=1}^{n} {\sum\limits_{k=0}^{m} {_{m+1} C_k x^k}} \\
&= \sum\limits_{k=0}^{m} {_{m+1} C_k \left(\sum\limits_{x=1}^{n} {x^k} \right) } \\
&= \sum\limits_{k=0}^{m} {_{m+1} C_k S_k(n)} \\
\therefore (m+1) S_m(n) &= (n+1)^m -1 - \sum\limits_{k=0}^{m-1} {_{m+1} C_k S_k(n)}
\end{align} $$</p>

<br/>

### 분수꼴 수열의 합
수열이 $\dfrac{1}{a_n a_{n+1}}$ (등차수열 $a_n$) 형태면 <br/>
$\dfrac{1}{a_n a_{n+1}} = \dfrac{1}{a_{n+1}-a_{n}}\left(\dfrac{1}{a_n} - \dfrac{1}{a_{n+1}} \right)$로 바꾼다.

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학1_수열" %}

### 수학적 귀납법
자연수 $n$에 대한 명제 $p(n)$이 모든 자연수 $n$에 대하여 성립한다는 것을 증명하는 방법. 다음 2가지를 보이면 된다
  1. $n=1$일 때, $p(n)$이 성립
  2. $n=k$일 때, $p(n)$이 성립한다고 가정하면 $n=k+1$일 때에도 명제 $p(n)$이 성립

귀납법을 통해 수열의 점화식을 $a_{n+1} - a_n = d, a_1 = a$와 같이 나타낸다.

{% capture context1 %}

### 초한귀납법(transfinite induction) (강한 수학적 귀납법)
* 귀납법 $p(k) \Rightarrow p(k+1)$을 확장하여, $p(1) \wedge p(2) \wedge \cdots \wedge p(k) \Rightarrow p(k+1)$임을 보이는 정리.
* 아예 자연수 $\mathbb{N} = (1, 2, \cdots )$가 아닌, 순서 관계가 정의된 임의의 집합(서수) $A$로 확장할 수도 있다.
* [한줄로 요약](https://namu.wiki/w/%EC%88%98%ED%95%99%EC%A0%81%20%EA%B7%80%EB%82%A9%EB%B2%95)하면 아래와 같다
  * $x \in A$에 대하여, $\forall y \in A, \left(y<x \Rightarrow p(y) \right) \Rightarrow p(x)$

<br/>

### 수열의 점화식과 일반항
1. $a_{n+1} = a_n + f(n)$
  * $a_n = a_1 + \sum\limits_{k=1}^{n-1} {f(k)}$

2. $a_{n+1} = f(n)a_n$
  * $a_n = a_1 \prod\limits_{k=1}^{n-1} {f(k)}$

3. $a_{n+1} = pa_n + q \; (p\neq 0, p\neq 1, q\neq 0)$
  * $a_{n+1}-\alpha = p(a_n - \alpha)$ 꼴로 변형$(\alpha=\frac{q}{p+1})$하면
  * $a_n=(a_1-\alpha)p^{n-1}+\alpha$

{% endcapture %}

{% capture context2 %}
### 뻘소리1 - 귀납법의 증명
수학적 귀납법을 어떻게 증명하느냐? 가 문득 궁금해졌다 <br/>
괜히 그랬다. 아 내 시간

--------------------

우선 [자연수의 정렬성](http://blog.daum.net/_blog/BlogTypeView.do?blogid=0RpSK&articleno=13&categoryId=3&regdt=20141126162353)이라는게 있는데, <br/>
간단히 말해서 자연수 $\mathbb{N}$의 임의의 부분집합 S에는 최소항이 존재한다는 사실.

페아노 공리계 안에서, 이 자연수의 정렬성은 초한귀납법과 [무한 강하법](https://ko.wikipedia.org/wiki/%EB%AC%B4%ED%95%9C%EA%B0%95%ED%95%98%EB%B2%95)과 모두 서로 동치이다.<br/>
앞에서 다룬 바로는, 초한귀납법은 임의의 서수 $A$에 대해서 성립하는, 귀납법의 상위 개념이다.<br/>
그러면
* 초한귀납법 ($\Leftrightarrow$ 자연수의 정렬성)
* $\mathbb{N} \backslash {0} \subseteq \mathbb{N} + 1$(모든 $0$이 아닌 자연수는 어떤 자연수 $+1$이다)

이 2개의 논리곱과 수학적 귀납법은 [동치가 된다](https://ko.wikipedia.org/wiki/%EC%88%98%ED%95%99%EC%A0%81_%EA%B7%80%EB%82%A9%EB%B2%95).<br/>

[증명](http://j1w2k3.tistory.com/1116)

-------------------

그럼 이제 서로 동치인건 알겠으니, <br/>
자연수의 정렬성과 (모든 $0$이 아닌 자연수는 어떤 자연수 $+1$이다) 라는 사실이 먼저 증명되는가, <br/>
수학적 귀납법이 먼저 증명되는가 라는 문제가 있는데 <br/>
자연수 체계를 묘사하는 5개의 공리을 모아놓은 [페아노 공리계](https://ko.wikipedia.org/wiki/%ED%8E%98%EC%95%84%EB%85%B8_%EA%B3%B5%EB%A6%AC%EA%B3%84) 에서는
아무래도 자연수의 정렬성을 먼저 공리로 두고 귀납법을 증명하는거 같긴 한데 <br/>
솔직히 잘 모르겠다 뭐래는건지

참고로 그 악명높은 1+1=2 의 증명도 페아노 공리계를 좀 더 파고들면 가능한 것 같다.
[링크](http://blog.naver.com/PostView.nhn?blogId=a4gkyum&logNo=220978355057&parentCategoryNo=60&categoryNo=&viewDate=&isShowPopularPosts=true&from=search)

아 안해

<br/>

----------------------------

### 뻘소리2 - 귀납법의 범위 확장
자연수에서만 정의한 수학적 귀납법의 범위를 어디까지 확장할 수 있는가 <br/>
두둥

일단 정수까진 가능할 것 같다. $p(0)$가 성립함을 보이고 $p(-k) \Rightarrow p(-k-1)$이 성립함을 보이면 될 것 같다..

그렇다면 $(\mathbb{Z}, \mathbb{Z})$과 같은 두 정수 쌍은? <br/>
$p(n, m) \Rightarrow p(n, m\pm 1) \wedge p(n\pm 1, m)$을 보이면 될 것 같다 <br/>
임의의 유리수 $\frac{p}{q}$ 는 결국 두 정수 쌍으로 나타낼 수 있다. <br/>
결국 유리수에 대해서도 성립하는 것 같다..

자연수, 정수, 유리수는 일단 모두 $\aleph_0$ 에 속한다. 그러니까 [원소 갯수가 수학적으로 같다](https://terms.naver.com/entry.nhn?docId=3568639&cid=58944&categoryId=58970). <br/>
근데 실수부턴 $2^{\aleph_0}$에 속하기 때문에 [안된다](https://terms.naver.com/entry.nhn?docId=3568763&cid=58944&categoryId=58970). <br/>

정수나 유리수에 대해서 적용이 됨을 엄밀하게 증명 가능한지는 모르겠다. <br/>
아몰랑

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학1_귀납법" %}

### 수열의 극한
무한수열 ${a_n}$에서, $n \to \infty$로 보낼 때
  * 수렴: $\lim\limits_{n \to \infty} {a_n} = \alpha$
  * 발산: $\lim\limits_{n \to \infty} {a_n} = \pm \infty$
    * 진동: 발산하되 양이나 음의 무한대로 발산하지 않음

* 무한수열 ${a_n}$의 $n$항까지의 부분합 $S_n=\sum\limits_{k=1}^{n} {a_k}$가 $n \to \infty:\; S_n \to S$일 때 무한급수가 수렴한다고 함.
* 무한급수 $S=\sum\limits_{n=1}^{\infty} {a_n}$가 수렴 $\Rightarrow \lim\limits_{n \to \infty} {a_n}=0$

{% capture context1 %}
### 극한의 정의(급식)
* 무한수열 ${a_n}$에서 $n$이 한없이 커질 때 $a_n$이 일정한 값 $\alpha$에 한없이 가까워지면, <br/>
  무한수열 ${a_n}$는 $\alpha$에 수렴한다고 정의하고 $\alpha$를 극한값이라 한다.
  * $\lim\limits_{n \to \infty} {a_n}=\alpha$, 또는 $n \to \infty$ 일 때 $a_n \to \alpha$ 로 표현한다
* $\lim\limits_{n \to \infty} {a_n}=\pm \infty$일 때 양의(음의) 무한대로 발산한다고 정의하고,
* ${a_n}$이 수렴하거나 양이나 음의 무한대로 발산하지 않으면 수열이 진동한다고 정의한다. (발산의 일종)

극한의 정의(학식)은 나중에 학식파트에서 자세히 다루도록 하자.

<br/>

### 수열의 극한 기본성질
$\lim\limits_{n \to \infty} {a_n} = \alpha, \; \lim\limits_{n \to \infty} {b_n} = \beta$ 일 때,
* $\lim\limits_{n \to \infty} {a_n\pm b_n} = \alpha \pm \beta$
* $\lim\limits_{n \to \infty} {ka_n} = k\alpha$
* $\lim\limits_{n \to \infty} {a_n b_n} = \alpha \beta$
* $(b_n \neq 0, \beta \neq 0) \Rightarrow \lim {\frac{a_n}{b_n}} = \frac{\alpha}{\beta}$

무한급수 $\sum\limits_{n=1}^{\infty} {a_n}=S, \; \sum\limits_{n=1}^{\infty} {b_n}=T$ 일 때,
* $\sum\limits_{n=1}^{\infty} {a_n\pm b_n}=S\pm T$
* $\sum\limits_{n=1}^{\infty} {ca_n}=cS$

<br/>

### 수열의 극한의 대소관계
* $\left(\lim\limits_{n \to \infty} {a_n} = \alpha, \lim\limits_{n \to \infty} {b_n} = \beta \right) \;
  \wedge \; \left( \forall n \in \mathbb{N}, a_n \leq b_n \right) \Rightarrow \alpha \leq \beta$
* $\left(\lim\limits_{n \to \infty} {a_n} = \lim\limits_{n \to \infty} {b_n} = \alpha \right) \;
  \wedge \; \left( \forall n \in \mathbb{N}, a_n \leq c_n \leq b_n \right) \Rightarrow \lim\limits_{n \to \infty} {c_n} = \alpha$

두번째는 샌드위치 정리라고도 불린다.

<br/>

### 수열의 극한값 구하기
* 분수꼴의 무한수열 $\dfrac{a_n}{b_n}$의 극한은 $a_n$과 $b_n$의 최고차항의 계수로 구한다.
  * (분모 차수) $<$ (분자 차수)이면 $\pm \infty$
  * (분모 차수) $>$ (분자 차수)이면 $0$
  * 차수가 같으면 $\dfrac{a_n의 \; 최고차항 계수}{b_n의 \; 최고차항 계수}$

* 수열 버전의 로피탈 정리인 Stolz-Cesaro Theorem이란게 있는데
<p> $$ \lim\limits_{n \to \infty} {\dfrac{a_{n+1}-a_n}{b_{n+1}-b_{n}}} = L \Rightarrow \lim\limits_{n \to \infty} {\frac{a_n}{b_n}} = L $$ </p>
  증명은.. 관심없어서 생략

* 무한등비수열 $a_n = ar^{n-1}$에서, $r>1$일 때 발산, $r=1$일 때 수렴, $\left\| r \right\|< 1$일 때 $0$(수렴), $r \leq -1$일 때 진동한다.

{% endcapture %}

{% capture context2 %}
수1 파트에서 여태껏 뻘소리 오지게 했는데 <br/>
극한은 대학교 입학하면 미적분학에서 바로 다루니까 여기선 이지하게 가자

### 무한등비수열의 극한 증명
1. $r>1$일 때
  * $r=1+h(h>0), r^n=(1+h)^n \geq 1+nh$. 테일러 급수 쓰면 되지만 귀납법써도 증명 됨.
  * $\lim\limits_{n \to \infty} {r^n} = \lim\limits_{n \to \infty} {1+nh} = \infty$
2. $r=1$일 때
  * 뭐
3. $\left\| r \right\| <1$일 때
  * $r=0$이면 $0$, $r\neq 0$이면 $\dfrac{1}{\left\| r\right\|}>1, \; \lim\limits_{n \to \infty} {\dfrac{1}{\left\| r\right\|}} = \infty$
  * $\therefore \lim\limits_{n \to \infty} {\left\|r^n \right\|}=0, \; \lim\limits_{n \to \infty} {r^n}=0$
4. $r \leq -1$일 때
  * $r=-1$이면 ${r^n}$은 진동하고, $r<-1$이면 $\lim\limits_{n \to \infty} {\left\|r^n \right\|}=\infty$ 이고 부호가 교대로 바뀌므로 진동함.

<br/>

### 샌드위치 정리 증명
증명을 찾아봤더니 극한의 학식정의론 증명이 안된다 <br/>
미적분학 가서 해야지 ㅅㄱ

<br/>

### 무한급수와 수열의 극한 사이의 관계 증명
<p> $$ \left(\lim\limits_{n \to \infty} {a_n} = \lim\limits_{n \to \infty} {b_n} = \alpha \right) \; \wedge \; \left(\forall n \in \mathbb{N}, \; a_n \leq c_n \leq b_n \right) \Rightarrow \lim\limits_{n \to \infty} {c_n} = \alpha $$ </p>
* $ a_n = S_n - S_n-1 (n \geq 2), \lim\limits_{n \to \infty} {a_n} = \lim\limits_{n \to \infty} {S_n - S_{n-1}} = S-S = 0 $
* 대우로, $\lim\limits_{n \to \infty} {a_n} \neq 0$ 이면 무한급수 $\sum\limits_{n=1}^{\infty} {a_n}$은 발산함.

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학1_극한" %}

## 수학 2

-------------------------------------

### 으아아아악!
**아래 내용은 진짜진짜로 매우 기억이 나지 않습니다** <br/>
**흑흑흑흑흑흑흑흑흑흑**

-------------------------------------

### 삼각함수 잡다한 공식(2)
* $1+\tan^2\theta = \sec^2\theta$, $1+\cot^2\theta = \csc^2 \theta$
* $\sin(\alpha\pm\beta) = \sin\alpha \cos\beta \pm \cos\alpha \sin\beta$,
  $\cos(\alpha\pm\beta) = \cos\alpha\cos\beta \mp \sin\alpha\sin\beta$,
  $\tan(\alpha\pm\beta) = \dfrac{\tan\alpha\pm\tan\beta}{1\mp\tan\alpha\tan\beta}$
* $a\sin\theta+b\cos\theta = \sqrt{a^2+b^2}\sin(\theta+\alpha) = \sqrt{a^2+b^2}\cos(\theta-\beta)$  
  (단, $\cos\alpha=\dfrac{a}{\sqrt{a^2+b^2}}$, $\cos\beta=\dfrac{b}{\sqrt{a^2+b^2}}$)
* $\sin 2\alpha = 2\sin\alpha\cos\beta$, $\cos 2\alpha=\cos^2\alpha-\sin^2\alpha$,
  $\tan 2\alpha = \dfrac{2\tan\alpha}{1-\tan^2\alpha}$
* $\sin^2\dfrac{\alpha}{2}=\dfrac{1-\cos\alpha}{2}$, $\cos^2\dfrac{\alpha}{2}=\dfrac{1+\cos\alpha}{2}$, 
  $\tan^2\dfrac{\alpha}{2}=\dfrac{1-\cos\alpha}{1+\cos\alpha}$
* $\sin\alpha\cos\beta=\dfrac{1}{2}\left\\{\sin(\alpha+\beta)+\sin(\alpha-\beta)\right\\}$,
  $\cos\alpha\sin\beta=\dfrac{1}{2}\left\\{\sin(\alpha+\beta)-\sin(\alpha-\beta)\right\\}$  
  $\cos\alpha\cos\beta=\dfrac{1}{2}\left\\{\cos(\alpha+\beta)+\cos(\alpha-\beta)\right\\}$,
  $\sin\alpha\sin\beta=-\dfrac{1}{2}\left\\{\cos(\alpha+\beta)-\cos(\alpha-\beta)\right\\}$
* $\sin A+\sin B=2\sin\dfrac{A+B}{2}\cos\dfrac{A-B}{2}$,
  $\sin A-\sin B=2\cos\dfrac{A+B}{2}\sin\dfrac{A-B}{2}$  
  $\cos A+\cos B=2\cos\dfrac{A+B}{2}\cos\dfrac{A-B}{2}$,
  $\cos A-\cos B=-2\sin\dfrac{A+B}{2}\sin\dfrac{A-B}{2}$
  
{% capture context1 %}
### 종류
1. 삼각함수의 덧셈정리
2. 삼각함수의 합성 (from 덧셈정리)
3. 배각 공식 (from 덧셈정리)
4. 반각 공식 (from 배각공식)
5. 곱 $\to$ 합 (from 덧셈정리)
6. 합 $\to$ 곱 (from 곱 $\to$ 합)

증명은 다음 단계에
{% endcapture %}

{% capture context2 %}
### 덧셈정리 증명
![Alt text](/pictures/mathematics/덧셈공식.PNG)
* 두 각도 $\alpha$와 $\beta$를 단위원의 두 점 $P(cos\alpha, \sin\alpha), Q(\cos\beta, \sin\beta)$로 나타낸다.
* 코사인 법칙에 의해 $\bar{PQ}^2=1^2+1^2-2\cdot 1 \cdot 1 \cdot \cos(\alpha - \beta) = 2-2\cos(\alpha-\beta)$
* 거리 공식에 의해 $\bar{PQ}^2=(\cos\beta-\cos\alpha)^2+(\sin\beta-\sin\alpha)^2=2-2(\cos\alpha\cos\beta+\sin\alpha\sin\beta)$
* 따라서, $\cos(\alpha-\beta)=\cos\alpha\cos\beta+\sin\alpha\sin\beta$
* $\beta$ 대신 $-\beta$를 넣으면 $\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta$
* $\sin\theta=\cos\left(\frac{\pi}{2}-\theta\right)$를 $\sin(\alpha+\beta)$에 대입하면
  $\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta$

<br/>

### 삼각함수 합성 증명
![Alt text](/pictures/mathematics/삼각합성1.PNG) ![Alt text](/pictures/mathematics/삼각합성2.PNG)
* $\sin\alpha = \dfrac{b}{\sqrt{a^2+b^2}},\; \cos\alpha=\dfrac{a}{\sqrt{a^2+b^2}}$
<p> $$\begin{align}
   a\sin\theta+b\cos\theta &= \sqrt{a^2+b^2}\left(\dfrac{b}{\sqrt{a^2+b^2}}\sin\theta+\dfrac{b}{\sqrt{a^2+b^2}}\cos\theta \right) \\
                           &= \sqrt{a^2+b^2}(\cos\alpha\sin\theta+\sin\alpha\cos\theta) \\
                           &= \sqrt{a^2+b^2}\sin(\theta+\alpha)
\end{align}$$</p> 
* $\beta=\dfrac{\pi}{2}-\alpha, \; \sin\beta = \dfrac{a}{\sqrt{a^2+b^2}},\; \cos\beta=\dfrac{b}{\sqrt{a^2+b^2}}$ 
<p> $$\begin{align}
   a\sin\theta+b\cos\theta &= \sqrt{a^2+b^2}\left(\dfrac{b}{\sqrt{a^2+b^2}}\sin\theta+\dfrac{b}{\sqrt{a^2+b^2}}\cos\theta \right) \\
                           &= \sqrt{a^2+b^2}(\sin\beta\sin\theta+\cos\beta\cos\theta) \\
                           &= \sqrt{a^2+b^2}\sin(\theta-\alpha)
\end{align}$$</p> 

<br/>

### 배각공식 증명
덧셈공식의 특별한 케이스니 생략

<br/>

### 반각공식 증명
* $\cos 2\alpha=1-2\sin^2\alpha, \; \sin^2\alpha=\dfrac{1-\cos 2\alpha}{2}, 
   \; \sin^2\dfrac{\alpha}{2} = \dfrac{1-\cos\alpha}{2}$
* $\cos 2\alpha=2\cos^2\alpha-1, \; \cos^2\alpha=\dfrac{1+\cos 2\alpha}{2}, 
   \; \cos^2\dfrac{\alpha}{2} = \dfrac{1+\cos\alpha}{2}$

<br/>

### 합 $\leftrightarrow$ 차
* $\sin(\alpha+\beta) = \sin\alpha\cos\beta+\cos\alpha\sin\beta$
* $\sin(\alpha-\beta) = \sin\alpha\cos\beta-\cos\alpha\sin\beta$
* $\therefore \sin\alpha\cos\beta = \frac{1}{2}\left\\{\sin(\alpha+\beta)+\sin(\alpha-\beta)\right\\}$

* $2\sin\alpha\cos\beta = \sin(\alpha+\beta)+\sin(\alpha-\beta)$
* $\text{let } \alpha+\beta=A, \alpha-\beta=B$
* $\sin A+\sin B=2\sin\dfrac{A+B}{2}\cos\dfrac{A-B}{2}$

{% endcapture %}
{% include blocks.html context1=context1 context2=context2 topic="수학2_삼각함수" %}

### 함수의 극한
* 함수 $f(x)$에서, $x \to a$로 보낼 때, $\lim\limits_{x \to a} {f(x)}=\alpha$ 또는 $x\to a \longrightarrow f(x)\to\alpha$  
* $\lim\limits_{x\to 0} {\dfrac{\sin x}{x}}=1,\; \lim\limits_{x\to 0} {(1+x)}^{\frac{1}{x}}=e,\; \lim\limits_{x\to \infty} {\left(1+\frac{1}{x}\right)}^x=e$  
* $\ln{x} := \log_{e}{x},\; \lim\limits_{x\to 0} {\frac{\log_{a}(1+x)}{x}}=\frac{1}{\ln{a}},\; \lim\limits_{x\to 0} {\frac{a^x-1}{x}}=\ln{a}$
  
* 함수 $f(x)$에서 $\lim\limits_{x\to a} {f(x)} = f(a)$일 때 $f(x)$ 는 $x=a$에서 연속이라고 한다.  
* 함수 $f(x)$가 닫힌 구간 $[a, b]$에서 연속이면 $f(x)$는 최대, 최소값을 가지며(최대, 최소의 정리),  
* $f(a)\neq f(b)$일 때 $f(a),\; f(b)$ 사이의 임의의 실수 $k$에 대하여 $f(c)=k$인 $c$가 $(a, b)$에 존재한다. (중심값 정리)

{% capture context1 %}
### 함수의 극한 정의(급식)
* 함수 $f(x)$에서 $x\neq a$가 한없이 $a$에 가까워질 때,  
  $f(x)$의 값이 일정한 값 $\alpha$에 한없이 가까워지면 $f(x)$는 $\alpha$에 수렴한다고 한다.  
* $\lim\limits_{x \to a} {f(x)}=\alpha$ 또는 $(x\to a) \longrightarrow (f(x)\to\alpha)$  
* $g(x)=\dfrac{x^2-1}{x-1}$에서 $g(1)$은 정의되지 않지만, $\lim\limits_{x \to 1}{g(x)}$는 2로 정의된다.

<br/>

* 함수 $f(x)$에서 $x<a$가 한없이 $a$에 가까워질 때 $f(x)$의 값이 일정한 값 $\alpha$에 한없이 가까워지면  
  $f(x)$의 좌극한은 $\lim\limits_{x \to a-0}{f(x)}=\alpha$로 정의되고,  
* $x>a$가 한없이 $a$에 가까워질 때 $f(x)$의 값이 $\beta$에 한없이 가까워지면  
  $f(x)$의 우극한은 $\lim\limits_{x \to a+0}{f(x)}=\beta$로 정의된다.
* 이때 $\lim\limits_{x \to a-0}{f(x)}=\lim\limits_{x \to a+0}{f(x)}=\alpha \Leftrightarrow \lim\limits_{x \to a}{f(x)}=\alpha$ 로 극한값이 정의된다.

<br/>

### 함수의 극한 성질
$\lim\limits_{x \to a}{f(x)}=\alpha,\; \lim\limits_{x \to a}{g(x)}=\beta$ 일 때
* $\lim\limits_{x \to a}{cf(x)}=c\alpha$
* $\lim\limits_{x \to a}{f(x)\pm g(x)}=\alpha\pm \beta$
* $\lim\limits_{x \to a}{f(x)g(x)}=\alpha \beta$
* $\lim\limits_{x \to a}{\dfrac{f(x)}{g(x)}}=\dfrac{\alpha}{\beta}$


$a$에 가까운 모든 $x$에 대하여
* $f(x) \leq g(x) \Rightarrow \alpha\leq\beta$
* $\left(f(x) \leq h(x) \leq g(x) \; \wedge \; \alpha=\beta \right) \Rightarrow \lim\limits_{x\to\alpha} {h(x)} = \alpha$

<br/>

### 삼각함수의 극한
* $\lim\limits_{x\to 0} \dfrac{\sin(x)}{x}=1$  
* $\lim\limits_{x\to 0} \dfrac{\tan(x)}{x}=1$ 
* $\lim\limits_{x\to 0} \dfrac{\sin(bx)}{ax}=\dfrac{b}{a}$

<br/>

### 무리수 e
* $\ln{x} := \log_{e}{x}$  
* $\lim\limits_{x\to 0} {(1+x)}^{\frac{1}{x}}=e \quad (e=2.71828182845\cdots)$  
* $x\to \frac{1}{x} \to \lim\limits_{x\to \infty} {\left(1+\frac{1}{x}\right)}^x=e$  

<br/>

### 함수의 연속 정의(급식)
함수 $f(x)$가 아래를 모두 만족할 때 $x=a$에서 연속이라고 한다
1. $x=a$ 에서 정의되어 있고
2. $\lim\limits_{x\to a} {f(x)}$가 존재하며
3. $\lim\limits_{x\to a} {f(x)} = f(a)$일 때

<br/>

이 때 $f(x)$가 구간 $(a, b)$의 모든 실수에 대하여 연속일 때, $f(x)$는 $(a, b)$에서 연속함수라고 한다.  
* 닫힌 구간 $[a, b]$에 대해서는 추가로 $\lim\limits_{x\to a+0} {f(x)}=f(a),\; \lim\limits_{x\to b-0} {f(x)}=f(b)$를 만족해야 함

<br/>

$f(x),\; g(x)$가 $x=a$에서 연속이면, 아래는 모두 연속
* $cf(x),\; f(x)\pm g(x),\; f(x)g(x),\; \frac{f(x)}{g(x)}$

{% endcapture %}

{% capture context2 %}

### 삼각함수의 극한 증명
![Alt text](/pictures/mathematics/삼각함수_극한.JPG)  
$0<x<\frac{\pi}{2}$일 때, $\triangle OAB <$ 부채꼴 $OAB < \triangle OAT$  
<p>$$ 
\therefore \frac{1}{2}\sin x < \frac{1}{2}x < \frac{1}{2}\tan x, \\  
1 < \dfrac{x}{\sin x} < \cos{x}, \; \cos{x} < \dfrac{\sin x}{x} < 1  \\
\lim\limits_{x\to +0} {\cos{x}} = 1, \; \lim\limits_{x\to +0} {\frac{\sin x}{x}} = 1 
$$</p>

<br/>

### 최대, 최소, 중간값의 정리
증명은 기억상 미적분학에서 다룬다. 아니더라도 그때 가서 다시 함.

다변수 함수에서 최대, 최소 정리를 일반화시키면: 
<p align="center">
$f:\; \mathbb{R}^n \to \mathbb{R}$가 $A \subset \mathbb{R}^n$에서 연속이고, $A$가 compact하면 $f$는 $A$에서 최대값과 최소값을 가진다.  
</p>
가 된다. [compact 정의](https://ko.wikipedia.org/wiki/%EC%BD%A4%ED%8C%A9%ED%8A%B8_%EA%B3%B5%EA%B0%84)
<br/>

### 자연상수 e
고등학교에서는 교육과정 순서때문에 $e$를 $\lim\limits_{x\to 0} {1+x}^{\frac{1}{x}}$로 정의하지만,  
아무래도 갑툭튀 하는 감이 없지않아 있다.   

엄밀한 증명 순서는 자연로그 $\ln{x}=\int_{1}^{x} {\frac{1}{t}dt}$를 먼저 정의한 이후 $\ln{x}=1$을 만족하는 $x$값을 $e$라고 정의하는게 가장 명확한 정의라고 한다.
[꺼라위키 나무](https://namu.wiki/w/%EC%9E%90%EC%97%B0%EC%83%81%EC%88%98)  
하지만 역사적으로는 $\lim\limits_{x\to 0} {(1+x)}^{\frac{1}{x}}=e$ 가 먼저 나온게 맞다.

자연로그의 정의로부터 $e=\lim\limits_{x\to 0} {(1+x)}^{\frac{1}{x}}$를 유도하는 순서로는
1. $\ln{x}$로부터 $e$, 그리고 $e^x$를 정의, $\frac{de^x}{dx}=e^x$ 임을 유도
2. 테일러 급수로부터 $e^x= \sum\limits_{n=0}^{\infty} {\dfrac{x^n}{n!}},\; e=\sum\limits_{n=0}^{\infty} {\dfrac{1}{n!}}$
3. 이항정리로부터 $e=\sum\limits_{n=0}^{\infty} {\dfrac{1}{n!}}=\lim\limits_{x\to 0} {(1+x)}^{\frac{1}{x}}$ 임을 유도 

하면 된다.

--------------------

$e$는 매우 많은 성질을 가지고 있다. 몇가지만 나열해보자면
1. [초월수](https://ko.wikipedia.org/wiki/%EC%B4%88%EC%9B%94%EC%88%98)이다. 모든 실수 초월수는 무리수라서 역시 무리수이다. [증명](https://ko.wikipedia.org/wiki/E_(%EC%83%81%EC%88%98)#%EB%AC%B4%EB%A6%AC%EC%88%98)
2. $x=0$에서 지수함수 $f(x)=a^x$의 기울기가 0이 되는 $a$이며, 동시에 $ce^x$는 $\frac{df(x)}{dx}=f(x)$ 인 유일한 함수이다.
3. 테일러 급수에 의해 $e=\sum\limits_{n=0}^{\infty} {\dfrac{1}{n!}}$
4. 복소수 범위로 확장된 지수함수 $a^{i\theta}$에서, $a^{i\pi}=-1$ 로 매칭시키는 상수이다. 나중에 오일러 공식 할때 다룰 예정
5. 확률이 $1/n%$인 뽑기를 $n$번 뽑았을 때, 한번도 안 뽑힐 확률은 $n \to \infty$일 때 $1/e$로 수렴한다.  
   동시에 이율을 $1/n$, 횟수를 $n$으로 두는 복리계산의 합은 $n \to \infty$일 때 $e$로 수렴한다.

-----------------

**개인적으로 생각하는** 가장 직관적인 정의는  
* 함수 $f(x)=a^x$의 $x$에서 기울기값은 원래 함수값 $a^x$에 특정한 상수 $C$가 곱해진 값으로 나타나는 성질이 있는데  
* $a=1$일 때 $C$는 $0$이고 $a\to\infty$일 때 $C$는 $\infty$로 발산한다.  
* 근데 $a$가 증가함에 따라 $C$가 연속적으로 증가하니까, 자연스레 $C=1$이 되는 순간이 있을 것이고  
  그 때의 무리수 $a=2.71828182845\cdots$ 를 $e$로 정의한다.
  
이후 기타 $e$의 성질들은 차근차근 유도 가능함

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학2_극한" %}

### 미분
* $x=a$에서 연속인 함수 $f(x)$의 미분계수
  $f'(a) = \lim\limits_{\Delta x\to 0} {\dfrac{\Delta y}{\Delta x}} = \lim\limits_{\Delta x\to 0} {\dfrac{f(a+\Delta x)-f(a)}{\Delta x}}$  
* 도함수 $f'(x)=\dfrac{d}{dx}f(x) = \lim\limits_{\Delta x\to 0} {\dfrac{f(x+\Delta x)-f(x)}{h}} 
= \lim\limits_{h\to 0} {\dfrac{f(x+h)-f(x)}{h}} = \lim\limits_{\Delta t\to x} {\dfrac{f(t)-f(x)}{t-x}}$  

{% capture context1 %}
### 평균변화율
* $x$의 값이 $a$에서 $b$로 변할 때, 함숫값 $y$의 증분$(\Delta y) \; f(a) - f(b)$를 $x$의 증분$(\Delta x) \; b-a$으로 나눈 값  
* 즉 $\frac{\Delta y}{\Delta x} = \frac{f(b)-f(a)}{b-a} = \frac{f(a+\Delta x)-f(a)}{\Delta x}$ 
* 기하학적으로는 함수 $y=f(x)$ 그래프 위의 두 점 $P(a, f(a)),\; Q(a+\Delta x, f(a+\Delta x))$에 대하여 직선 $PQ$의 기울기를 뜻함 

<br/>

### 미분계수
* 함수 $f(x)$의 $a\to a+\Delta x$의 평균변화율의 $\Delta x\to 0$ 일 때의 극한값
* $f'(a) = \lim\limits_{\Delta x\to 0} {\frac{f(a+\Delta x)-f(a)}{\Delta x}}$이 존재 할 때(우극한 = 좌극한)    
  $f(x)$는 $x=a$에서 미분가능하다고 하며, 이 값을 $y=f(x)$의 미분계수라고 한다.  
* $f(x)$가 어떤 구간에 속하는 $x$에서 모두 미분 가능할 때, $f(x)$는 그 구간에서 미분가능하다고 한다.

<br/>

* 미분가능성한 함수는 연속인 함수의 충분조건이다.  
  * $f(x)$가 $x=a$에서 미분가능 $\Rightarrow f(x)$는 $x=a$에서 연속

![Alt text](/pictures/mathematics/미분가능성.JPG)  
역의 반례

<br/>

* 기하학적으로는 곡선 $y=f(x)$ 위의 점 $(a, f(a))$에서의 접선의 기울기를 뜻함
 
<br/>
 
### 도함수
* 정의역 $X$에서 미분가능한 함수 $y=f(x)$에 대하여 $\forall x\in X$를 $f'(x)$로 대응시키는 함수.  
* $f':x \longrightarrow f'(x) = \lim\limits_{\Delta x\to 0} {\frac{f(x+\Delta x)-f(x)}{\Delta x}}$  
* 이 함수를 구하는 것을 미분법이라고 한다.

<br/>

미분법의 매우 기본적인 공식으로는
1. $f(x)=x^n \Rightarrow f'(x)=nx^{n-1}$
2. $f(x)=c \Rightarrow f'(x)=0$
3. ${cf(x)}'=cf'(x)$
4. ${f(x)\pm g(x)}'=f'(x)\pm g'(x)$
5. ${f(x)g(x)}'=f'(x)g(x) + f(x)g'(x)$

{% endcapture %}

{% capture context2 %}
### 미분가능 $\Rightarrow$ 연속 증명
* 미분가능 $\Rightarrow f'(a)=\lim\limits_{x\to a} {\frac{f(x)-f(a)}{x-a}}$가 존재, $f'(a)$ 존재  
* $\lim\limits_{x\to a} {f(x)-f(a)} = \lim\limits_{x\to a} {\frac{f(x)-f(a)}{x-a}\cdot (x-a)}$   
  $=\lim\limits_{x\to a} {\frac{f(x)-f(a)}{x-a}}\cdot \lim\limits_{x\to a} {(x-a)}=f'(a)\cdot 0 = 0$  
* $\therefore \lim\limits_{x\to a} {f(x)}=f(a), \quad y=f(x)$는 $x=a$에서 연속이다.

<br/>

### 미분 표기법들
1. 라이프니츠(Leibniz) 표기법
    * $\dfrac{dy}{dx}=\dfrac{df(x)}{dx}=\dfrac{d}{dx}f(x)$
    * $\left. \dfrac{df}{dx} \right\|_{x=a} = \dfrac{df}{dx}(a) = \dfrac{d}{dx}f(a)$
    * $\dfrac{d^n y}{dx^n}= \dfrac{d^n f(x)}{dx^n}= \dfrac{d^n }{dx^n}f(x)$
    
2. 라그랑주(Lagrange) 표기법
    * $f^{(1)} = f', \; f^{(2)} = f'', \; f^{(3)}=f''', \quad f^{(n)} = f\, \overset{n}{\overbrace{''\cdots'}}$
    
3. 뉴턴(Newton) 표기법
    * $\overset{1}{\dot{y}}=\dot{y}, \; \overset{2}{\dot{y}}=\ddot{y}, \; \overset{3}{\dot{y}}=\dddot{y}, \quad \overset{n}{\dot{y}}$
    
4. 오일러(Euler) 표기법
    * $Df, \; D^2f, \; D^3f, \quad D^nf$

<br/>

### 미분'계수'?
[꺼라위키 출처](https://namu.wiki/w/%EB%AF%B8%EB%B6%84#s-3), [영어위키](https://en.wikipedia.org/wiki/Differential_of_a_function)
  
미분은 2가지 다른 단어가 미분이라는 한 단어로 번역된 것이라고 하는데, 
* 도함수를 얻는 과정인 differentiate의 명사형 differentiation(미분)과
* differential(미분)

이 있다.  
  
differential은 $f(\mathbb{x})$의 $\mathbb{x}=\mathbb{a}$ 에서의 선형$(L(a\mathbb{x}+\mathbb{y})=aL(\mathbb{x})+L(\mathbb{y}))$ 근사 함수 $L(\mathbb{x})=\mathbb{Ax}$를 구하는 것이고,
이 때 $\mathbb{x}=\mathbb{a}$에서 differential(미분)의 계수는 각 방향으로의 기울기값이 되며, 그렇기 때문에 기울기 == 미분'계수'가 된다  
* $dy=\frac{\partial y}{\partial x_1}dx_1+\frac{\partial y}{\partial x_1}dx_1+ \cdots + \frac{\partial y}{\partial x_n}dx_n$ 에서 $dx_i$의 계수: $x_i$방향으로의 기울기

<br/>

즉 미분은 도함수(derivative)를 구하는 것(differentiation)이거나    
혹은 선형근사함수를 구하는 것(differential)인데  
기울기를 구하는 것은 선형근사함수를 구한 결과(미분)의 계수이기 때문에 미분계수.

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학2_미분" %}

### 미분공식들
* $\left\\{\frac{f(x)}{g(x)} \right\\}' = \frac{f'(x)g(x)-f(x)g'(x)}{\\{g(x)\\}^2}$
* $r\in \mathbb{R}, y=x^r$의 도함수 $y'=rx^{r-1}$
* $y=f(u), u=g(x)$의 도함수 $y'=f'(g(x))g(x),\; \frac{dy}{dx}=\frac{dy}{du}\cdot \frac{du}{dx}$
* $x=f(t),\; y=g(t)$일 때 $\frac{dy}{dx}=\dfrac{\frac{dy}{dt}}{\frac{dx}{dt}}=\frac{g'(t)}{f'(t)}$
* 음함수 $f(x,\,y)=0$ 는 각 항을 $x$에 대하여 미분하여 $\frac{dy}{dx}$를 구한다
  * $f(x,\,y)=x^2+y^2-4=0 \Rightarrow f'(x,\,y)=2x+2y\frac{dy}{dx}=0, \; \frac{dy}{dx}=-\frac{x}{y}$
* $y=f^{-1}(x)$의 도함수 $\frac{dy}{dx}=\dfrac{1}{\frac{dx}{dy}}$ 
* $(\sin x)'=\cos x,\; (\cos x)'=-\sin x,\; (\tan x)'=\sec^2 x,\; (\sec x)'=\sec x\tan x,$   
  $(\cot x)'=-\csc^2 x,\; \csc x =-\csc x\cot x$
* $(\log_a x)'=\frac{1}{x\ln{a}},\; (a^x)'=a^x \ln{a}$

{% capture context1 %}
증명은 다음단계에
{% endcapture %}

{% capture context2 %}
* $r\in \mathbb{R}, y=x^r$의 도함수 $y'=rx^{r-1}$
  * $\dfrac{d}{dx}x^r = \dfrac{d}{dx}e^{r\ln x} = e^{r\ln x} \dfrac{r}{x} =rx^{r-1}$


* $\left\\{\dfrac{f(x)}{g(x)} \right\\}' = \dfrac{f'(x)g(x)-f(x)g'(x)}{\\{g(x)\\}^2}$
  * $y=\dfrac{1}{g(x)}, \Delta y=\dfrac{1}{g(x+\Delta x)}-\dfrac{1}{g(x)}= \dfrac{g(x)-g(x+\Delta x)}{g(x+\Delta x)g(x)}$
  * $\left\\{\dfrac{1}{g(x)}\right\\}'=\lim\limits_{\Delta x\to 0} {\dfrac{\Delta y}{\Delta x}}
    =-\lim\limits_{\Delta x\to 0} {\dfrac{g(x+\Delta x)-g(x)}{\Delta x}}\cdot \lim\limits_{\Delta x\to 0} {\dfrac{1}{g(x+\Delta x)g(x)}}=-\dfrac{g'(x)}{g^2(x)}$
  * $\left\\{\dfrac{f(x)}{g(x)}\right\\}'=\dfrac{f'(x)}{g(x)}+\dfrac{f(x)}{g'(x)}=\dfrac{f'(x)g(x)-f(x)g'(x)}{\\{g(x)\\}^2}$


* $y=f(u),\; u=g(x)$의 도함수 $\frac{dy}{dx}=\frac{dy}{du}\cdot \frac{du}{dx}$
  * $\Delta x\to 0$이면 $\Delta u\to 0$ 
  * $\dfrac{dy}{dx}=\lim\limits_{\Delta x\to 0} {\dfrac{\Delta y}{\Delta u}\cdot\dfrac{\Delta u}{\Delta x}} 
    =\lim\limits_{\Delta u\to 0} {\dfrac{\Delta y}{\Delta u}\cdot \lim\limits_{\Delta x\to 0} \dfrac{\Delta u}{\Delta x}} = \dfrac{dy}{du}\cdot \dfrac{du}{dx}$


* $y=f^{-1}(x)$의 도함수 $\frac{dy}{dx}=\dfrac{1}{\frac{dx}{dy}}$
  * $x=f(y),\; \frac{dx}{dx}=1=\frac{df(y)}{dx}=\frac{df(y)}{dy}\cdot\frac{dy}{dx}$
  * $\frac{dy}{dx}=\dfrac{1}{\frac{df(y)}{dy}}=\dfrac{1}{\frac{dx}{dy}}$


* $(\sin x)'=\cos x$
  * $(\sin x)'=\lim\limits_{h\to 0} {\frac{\sin(x+h)-\sin x}{h}}=\lim\limits_{h\to 0} {\frac{2\cos(x+h/2)\sin(h/2)}{h}}$  
    $=\lim\limits_{h\to 0} cos(x+h/2)\cdot {\frac{\sin(h/2)}{h/2}}=\cos x \cdot 1=\cos x$

    
* $(\log_a x)'=\dfrac{1}{x\ln{a}}$
  * $(\log_a x)'=\left\\{\dfrac{\log_e{x}}{\log_e{a}}\right\\}'=\dfrac{\ln'x}{\ln a}$
  * $\ln'x = \lim\limits_{h\to 0}{\frac{\ln(x+h)-\ln x}{h}}=\lim\limits_{h\to 0} {\frac{1}{x}\left\\{\frac{x}{h}\ln\left(1+\frac{h}{x}\right)\right\\}}$  
    $= \frac{1}{x}\lim\limits_{h\to 0}{\ln\left(1+\frac{h}{x}\right)^{\frac{x}{h}}}=\frac{1}{x}\ln e=\frac{1}{x}$

    
* $(a^x)'=a^x \ln{a}$
  * $(a^x)'=\lim\limits_{h\to 0} {\frac{a^{x+h}-a^x}{h}}=a^x\lim\limits_{h\to 0}{\frac{a^h-1}{h}}$
  * $a^h=t+1,\; h=\log_a(t+1),\; \lim\limits_{h\to 0}{\frac{a^h-1}{h}}=\lim\limits_{t\to 0}{\frac{t}{\log_a(t+1)}}=\lim\limits_{t\to 0}{\frac{1}{\log_a(t+1)^{1/t}}}=\ln{a}$

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학2_미분공식" %}


### 도함수의 활용
* 함수의 접선의 방정식 $y-f(a)=f'(a)(x-a)$, 접선에 수직인 방정식 $y-f(a)=-\frac{1}{f'(a)}(x-a)$
* 평균값의 정리: $[a, b]$에서 연속이고 $(a, b)$에서 미분가능한 $f(x)$에서 $\frac{f(b)-f(a)}{b-a}=f'(c)$인 $c$가 $[a, b]$ 안에 존재
* 증가(감소): $f'(a)>0$이면 $f(x)$는 $x=a$에서 증가상태에 있고, 구간 내 모든 $x$에 대하여 $f'(x)>0$이면 $f(x)$는 증가함수이다.
* $f'(a)=0$일 때, $f(x)$는 $f''(a)<0$이면 $x=a$에서 극댓값, $f''(a)>0$이면 $x=a$에서 극솟값을 가진다.
* 어떤 구간에서 $f''(x)>0$이면 $f(x)$는 아래로 볼록하고, $f''(x)<0$이면 위로 볼록하며, 곡선이 오목에서 볼록으로 바뀌는 지점을 변곡점이라 한다.  

{% capture context1 %}
### 평균값의 정리
#### 롤의 정리
![Alt text](/pictures/mathematics/롤의정리.JPG)  
함수 $f(x)$가 닫힌 구간 $[a, b]$에서 연속이고, $(a, b)$에서 미분가능하고, $f(a)=f(b)$이면  
<p> $$\exists c\in (a, b):\; f'(c)=0$$ </p>


-----------------------
#### 롤의 정리로부터 평균값의 정리 유도
![Alt text](/pictures/mathematics/평균값정리.JPG)
* $\bar{PQ}$의 방정식: $y-f(a)=\frac{f(b)-f(a)}{b-a}(x-a)$
* $g(x)= f(x)-\left\\{f(a)+\frac{f(b)-f(a)}{b-a}(x-a) \right\\}$로 두면, $g(x)$는 연속, 미분가능하며 $g(a)=g(b)=0$이다.
* 롤의 정리에 의해
 <p> $$
 \exists c\in (a, b):\; g'(c)=0 \\ f'(c)=\left. \frac{d}{dx}\left( g(x)+\frac{f(b)-f(a)}{b-a}(x-a)\right)\right\|_{x=c} =\frac{f(b)-f(a)}{b-a}
 $$ </p>

{% endcapture %}

{% capture context2 %}
### 롤의 정리 증명
$[a, b]$에서 연속이고 $(a, b)$에서 미분가능한 $f:[a, b] \longrightarrow \mathbb{R}$에 대하여, 
* 함수 $f$가 상수함수라면, $\forall c\in(a, b):\; f'(c)=0$
* 상수함수가 아니라면, $\exists x\in(a, b):\; f(x)\neq f(a)=f(b)$
  * WLOG, $\exists x\in(a, b):\; f(x)>f(a)=f(b)$
* 최대, 최소의 정리에 의하여 $f$는 $x=c\in(a, b)$에서 최댓값을 가진다.
  * $\exists c\in(a,b):\; f(x)-f(c) \leq 0$
* $\lim\limits_{x\to c+}{\frac{f(x)-f(c)}{x-c}} \leq 0,\; \lim\limits_{x\to c-}{\frac{f(x)-f(c)}{x-c}} \geq 0$
* $f$는 $x=c\in(a, b)$에 대하여 미분가능하므로, $\lim\limits_{x\to c+}{\frac{f(x)-f(c)}{x-c}}=\lim\limits_{x\to c-}{\frac{f(x)-f(c)}{x-c}}=f'(c)=0$

<br/>

### Fermat's Theorem for Extrema
$f:(a, b)\longrightarrow \mathbb{R}$에서, $f$가 $x_0\in (a, b)$에서 미분가능하다면,  
$x_0$는 극점 $\Rightarrow f'(x_0)=0$
* 어떠한 미분가능한 함수 $f$의 모든 극점(local extremum)은 stationary point이다 라는 정리.  
* 여기서 stationary point이란 $f$의 도함수가 0인 지점을 뜻한다.
  * 다변수 함수에 대해서, stationary point는 모든 편미분 계수가 0인 지점
* 대우: $f$가 $x_0\in (a, b)$에서 미분가능하다면, $f'(x_0)\neq 0 \Rightarrow x_0$는 극점이다.
 
<br/> 

증명을 해보자. [원래 방향으로도 증명이 가능하지만](https://en.wikipedia.org/wiki/Fermat%27s_theorem_(stationary_points)) 대우를 증명해보자.  
* WLOG, 미분가능한 점 $x_0\in(a, b)$에 대하여 $f'(x_0)=K>0$이라고 가정하자
* 미분의 정의상 $\lim\limits_{\varepsilon\to 0} {\frac{f(x_0+\varepsilon)-f(x_0)}{\varepsilon}}=K$
* $\varepsilon$에 대하여 극한을 취하지 않고, 충분히 작은 $\varepsilon_0$에 대하여 $(x_0-\varepsilon_0, x_0+\varepsilon_0)$ 구간에 속하는 $\varepsilon$에 대해서 생각해 보면,
  $\varepsilon_0$가 충분히 작다면 구간 안의 모든 $\varepsilon$는 평균변화율이 $K/2$보다 클 것이다.
  * $\varepsilon\in (x_0-\varepsilon_0, x_0+\varepsilon_0):\; \frac{f(x_0+\varepsilon)-f(x_0)}{\varepsilon}>\dfrac{K}{2}$
* $\varepsilon>0$일 때, $f(x_0+\varepsilon)>f(x_0)+(K/2)\varepsilon>f(x_0)$
* $\varepsilon<0$일 때, $f(x_0+\varepsilon)<f(x_0)+(K/2)\varepsilon<f(x_0)$
* 따라서, $f(x_0)$는 구간 $(x_0-\varepsilon_0, x_0+\varepsilon_0)$에 대하여 왼쪽에서는 $f(x-\varepsilon)$이 더 작고, 오른쪽에서는 $f(x+\varepsilon)$이 더 크기 때문에 극값이 아니다.

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="수학2_도함수활용" %}

## 적분과 통계

### 부정적분
F'(x)=f(x)일 때 F(x)를 f(x)의 부정적분이라고 함. \int f(x)dx=F(x)+C, \int\left(\dfrac{d}{dx}f(x)dx\right)=f(x)+C  
치환적분: \int f(g(x))g'(x)dx=\int \left(f(t)\dfrac{dt}{dx}\right)=\int f(t)dt  
부분적분: \int f'(x)g(x)dx=f(x)g(x)-\int f(x)g'(x)dx,\; \int u'vdx=uv-\int uv'dx

{% capture context1 %}
### 정의
F'(x)=f(x)에서 F(x)로부터 f(x)를 구하는 연산을 미분(differentiation)이라고 하고 f(x)를 도함수(derivative)라고 한다면  
f(x)로부터 F(x)을 구하는 연산을 부정적분이라고 하며  
F(x)는 역도함수(antiderivative), 원함수, 원시함수(primitive function)이라고 부른다.

<br/>

### 부정적분의 계산
1. \int kdx=kx+C
2. \int x^n dx=\frac{1}{n+1}x^{n+1}+C (r\in\mathbb{R},\; n\neq 1)
    * \int x^{-1} dx=\ln \|x\|+C 
3. \int kf(x)dx=k\int f(x)dx
4. \int \left(f(x)\pm g(x)\right)dx = \int f(x)dx \pm \int g(x)dx
5. \int \sin x dx=-\cos x+C,\; \int \cos xdx=\sin x+C
    * \int \sec^2 xdx=\tan x+C,\; \int \csc^2 xdx=-\cot x+C
    * \int \sec x\tan xdx=\sec x+C,\; \int \csc x\cot xdx=-\csc x+C
6. \int a^x dx=\dfrac{a^x}{\ln a}+C
{% endcapture %}

{% capture context2 %}
### 잡소리
부정적분은 미분의 역연산으로 정의된다.  
적분은 원래 함수의 넓이를 구하려고 생긴 것인데, 그건 정적분이고  
함수의 넓이를 구하는 정적분과 함수의 기울기를 구하는 미분과의 관계를 나타낸 것이 미적분학의 제 1 기본정리이며  
정적분이 부정적분의 차로 계산됨을 나타낸 것이 미적분학의 제 2 기본정리이다.

<br/>

### 부정적분의 계산 증명
\int \left(f(x)\pm g(x)\right)dx = \int f(x)dx \pm \int g(x)dx
* \frac{d}{dx}\left(\int f(x)dx\pm \int g(x)dx\right)=\frac{d}{dx}\left(\int f(x)dx\right)\pm\frac{d}{dx}\left(\int g(x)dx\right)=f(x)\pm g(x)
* \therefore \int f(x)dx \pm \int g(x)dx +C = \int \left(f(x)\pm g(x)\right)dx
* 위 식은 임의의 f(x), g(x)에 대하여 성립하므로, f(x)=g(x)=0으로 두면 C=0


나머지 식들도 위와 비슷하게 한다.

<br/>

### 치환적분 증명, infinitesimal differential
y=\int f(t)dt라고 두자  
chain rule에 의하여, \frac{dy}{dx}=\frac{dy}{dt}\cdot \frac{dt}{dx}=f(t)\frac{dt}{dx}=f(g(x))g'(x)  
\therefore, y=\int f(t)dt =\int \left(f(t)\frac{dt}{dx}\right)= \int f(g(x))g'(x)dx
  
위 예시던, 미분의 chain rule에서던, 기타등등  
dx, dy와 같은 미분소(differential)가 곱해지고 cancel out되고 등등 실제 변수마냥 취급되는 것을 확인할 수 있다.  
미분소가 항상 분자/분모 형태로 묶여 나오던 미분파트와는 다르게, 적분에서는 미분소가 \int dx로 묶여 나오면서 dx라는 term이 따로 노는 형태가 처음 등장하는데,    
이때 \left(\dfrac{dy}{dx}\right)dx가 어떻게 dy가 되는지, 그러니까 dx를 왜 실제 변수처럼 취급하여 cancel out할 수 있는지,  
더 근본적으로는, 그래서 dx가 정확히 무엇인지 궁금했었다.   
물론 위 식 \int f(t)dt =\int \left(f(t)\frac{dt}{dx}\right)에서 간접적으로 보여지긴 한다만, 그래도 직관적이진 않았다.

여기에 대한 해답은 [위키 링크](https://en.wikipedia.org/wiki/Differential_(infinitesimal))로 일단 대체한다.  
솔직히 아직 완전히 이해가 된건 아니고, 위 링크도 뭔가 속시원한 답을 주진 않는 것 같다. 

미분의 여러 notations 들 중, 왜 하필이면 라이프니츠의 표기법이 승리했는지를 알 수 있다.  
미분이라는 것을 ', dot, D와 같이 하나의 기본 연산자가 아니라, dy와 dx 두 미분소의 결합으로 두었기 때문에  
\left(\dfrac{dy}{dx}\right)dx 이라는 직관적 표현이 다른 표기법으로는 죽었다 깨어나도 불가능하기 때문.  

<br/>

### 부분적분 증명
곱의 미분법에 의하여, \left\\{f(x)g(x)\right\\}'=f'(x)g(x)+f(x)g'(x)  
이걸 부정적분하면, f(x)g(x)+C =\int f'(x)g(x)dx + \int f(x)g'(x)dx  
임의의 f(x), g(x)에 대하여 성립해야 하므로, f(x)=g(x)=0으로 두면 C=0  
\therefore \int f'(x)g(x)dx=f(x)g(x)-\int f(x)g'(x)dx, \; \int u'vdx=uv-\int uv'dx

부분적분에서는 함수를 적분될 놈(u)이랑 미분될 놈(v)으로 구분하는게 제일 중요한데,  
미분 우선순위는 \ln x, x^n, \sin x, e^x 순서대로 좋다(미분해서 빨리 조질 수 있는 형태).

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_부정적분" %}

### 정적분
구분구적법의 극한 \lim\limits_{n\to\infty}{\sum_{k=1}^{n} {f(x_k)\Delta x}}=\int_a^b {f(x)dx}  
\int_a^b {f(x)dx}=\left[F(x)\right]_a^b=F(b)-F(a)  

{% capture context1 %}
### 구분구적법과 정적분
![Alt text](/pictures/mathematics/정적분.jpg)  
넓이를 구하는데 사용되는 적분이라는 개념의 시초  
[a, b]에서 연속인 어떤 함수 f(x)를 n등분하여 각 분점의 x좌표를 x_0(=a), x_1, \cdots x_n(=b)로 두었을 때,  
\Delta x=\frac{b-a}{n}으로 두면, [a, b] 구간에서 f(x) 그래프의 넓이를 다음과 같이 근사할 수 있다.
<p> $$ S_n \simeq \sum\limits_{k=1}^n {f(x_k)\Delta x} $$</p>

이때 n\to\infty로 보내버리면 S_n은 실제 넓이의 참값에 수렴하게 되는데, 이를
<p> $$ S=\lim\limits_{n\to\infty} S_n = \lim\limits_{n\to\infty} {\sum\limits_{k=1}^n {f(x_k)\Delta x}} =\int_a^b f(x)dx $$</p>
로 표현한다.

<br/>

### 정적분의 계산
* \int_a^a f(x)dx=0
* \int_a^b f(x)dx=-\int_b^a f(x)dx
* \int_a^b kf(x)dx=k\int_a^b f(x)dx
* \int_a^b \left\\{f(x)\pm g(x)\right\\}dx=\int_a^b f(x)dx \pm \int_a^b g(x)dx
* \int_a^b f(x)dx=\int_a^c f(x)dx+\int_c^b f(x)dx

<br/>

* g(a)=\alpha, g(b)=\beta \Rightarrow \int_a^b f(g(x))g'(x)dx=\int_{\alpha}^{\beta} f(t)dt
* \int_a^b f'(x)g(x)dx=\left[f(x)g(x)\right]_a^b-\int_a^b f(x)g'(x)dx
* f(-x)=f(x) \Rightarrow \int_a^a f(x)dx=2\int_0^a f(x)dx
* f(-x)=-f(x) \Rightarrow \int_a^a f(x)dx=0
* \dfrac{d}{dx} \int_{h(x)}^{g(x) f(t)dt=f(g(x))g'(x)-f(h(x))h'(x)

{% endcapture %}

{% capture context2 %}
### 미적분학의 기본정리
위에서 잠깐 언급했지만, 미적분학의 기본정리는 
* 함수의 기울기를 구하는 미분
* 함수의 넓이를 구하는 적분

이 관련없어 보이는 두 개념을 서로 연관시키는 2가지의 정리이다.

<br/>

#### 제1 기본정리
함수 \f가 닫힌구간 [a,b]에서 연속이면, 함수 F(x)=\int _{a}^{x}f(t)\,dt 는 닫힌구간 [a,b]에서 연속이며 열린구간 (a,b)에서 미분이 가능하고,
함수 F의 도함수는 f이다.

x,x+h\in [a,b] 일 때,
\begin{aligned}
F'(x)&=\lim _{{h\to 0}}{\frac  {F(x+h)-F(x)}{h}}\\
     &=\lim _{{h\to 0}}{\frac  {1}{h}}\left[\int _{{a}}^{{x+h}}f(t)\,dt-\int _{{a}}^{{x}}f(t)\,dt\right]\\
     &=\lim _{{h\to 0}}{\frac  {1}{h}}\int _{{x}}^{{x+h}}f(t)\,dt
\end{aligned}  
이때, [적분의 평균값 정리](https://ko.wikipedia.org/wiki/%ED%8F%89%EA%B7%A0%EA%B0%92_%EC%A0%95%EB%A6%AC#%EC%A0%81%EB%B6%84_%ED%8F%89%EA%B7%A0%EA%B0%92_%EC%A0%95%EB%A6%AC)에 의해   
c\in [x,x+h]:\; {\frac  {1}{h}}\int _{{x}}^{{x+h}}f(t)\,dt=f(c)  
함수 f는 주어진 구간에서 연속이므로, [샌드위치 정리](https://en.wikipedia.org/wiki/Squeeze_theorem)에 의해 h가 작아짐에 따라 x+h는 x에 다가가고, 그러므로 c도 x에 다가간다.  
\lim _{h\to 0}f(c)=f(x)  
$\begin{aligned}
F'(x)&=\lim _{{h\to 0}}{\frac  {1}{h}}\int _{{x}}^{{x+h}}f(t)\,dt\\
     &=\lim _{{h\to 0}}f(c)\\
     &=f(x)
\end{aligned}$

-------------------

#### 제2 기본정리
함수 f가 닫힌구간 [a,b]에서 연속이며, 함수 F가 f의 임의의 부정적분이면, \int _{a}^{b}f(t)dt=F(b)-F(a)

함수 G를 G(x)=\int _{a}^{x}f(t)\,dt 으로 정의하면, 제1 기본정리에 의해 G(x)의 도함수는 f(x)가 되기 때문에 G(x)=\int f(x)dx +C' 이다. 
또 함수 F는 f의 임의의 부정적분이랬으니 F(x)=\int f(x)dx+C''이며,  
정리하면 F(x)=G(x)+C 가 된다.  
F와, (제1 기본정리에 의해) G는 [a,b]에서 연속이므로,
$\begin{aligned}
F(b)-F(a)&=\left[G(b)+C\right]-\left[G(a)+C\right]\\
         &=G(b)-G(a)\\
         &=\int _{{a}}^{{b}}f(t)\,dt-\int _{{a}}^{{a}}f(t)\,dt\\
         &=\int _{{a}}^{{b}}f(t)\,dt-0\\
         &=\int _{{a}}^{{b}}f(t)\,dt
\end{aligned}$

<br/> 
 
좀 더 엄밀한 증명은 [영어위키](https://en.wikipedia.org/wiki/Fundamental_theorem_of_calculus)를 참조하면 되는데 그렇게까지 살아야될거같진 않다. 

<br/>

### 리만 적분
위에서, 구분구적법 $ S_n \simeq \sum\limits_{k=1}^n {f(x_k)\Delta x} $에서 n\to\infty로 보내버리면 S_n은 실제 넓이의 참값에 수렴한다고 했다.  
진짜?  
않이... 왜?

좀 더 엄밀하게 다뤄보자. 하악  
![Alt text](/pictures/mathematics/하악.JPG)

일단 [리만 적분](http://mathnmath.tistory.com/95)이라는걸 정의해보자. 
![Alt text](/pictures/mathematics/구분구적법.jpg)
급식때에는 각 구간을 양심적으로 n등분하고, 함수값은 각 구간의 왼쪽(혹은 오른쪽) 구간을 선택했다.  
이걸 일반화한게 리만 적분인데, 일반화한 부분은
1. 구간을 균등하게 자르지 않고 내맘대로 자른다.
    * partition \Gamma = \\{x_0=a, x_1, x_2, \cdots, x_{n-1}, x_n=b \\}
    * 임의의 x_i는 [a, b] 구간 안에만 있음 된다. 심지어 x_i < x_{i+1}일 필요도 없이 내맘대로인데 편의상 x_i < x_{i+1}로 둔다.
    * \Gamma의 norm을 \max_i \|x_i-x_{i-1}\|, 그러니까 모든 subinterval의 가장 큰 길이를 norm으로 정의한다.
2. 각 구간에서, 함수값을 어느 것으로 선택할지 내맘대로 고른다.
    * \min(x_{i-1}, x_i) \leq \xi_i \leq \max(x_{i-1}, x_i)
    * \xi 를 태그(tag)라고 부른다.

<br/>

이렇게, 구간 [a, b]에서 함수의 넓이를 나타낸 급수는 다음과 같다  
<p> $$ \sum_{i=1}^n {f(\xi)|x_i-x_{i-1}|} $$ </p>
얘를 리만합(Riemann sum) 이라고 한다.  
![Alt text](/pictures/mathematics/리만적분.jpg)

<br/>

이때 파티션의 최대 길이인 \Gamma의 norm을 0으로 보낼 때, 즉 모든 subinterval의 길이를 0으로 보낼 때,  
\lim\limits_{\|\Gamma\|\to 0} {\sum_{i=1}^n {f(\xi)\|x_i-x_{i-1}\|}}가 어떠한 값으로 만약 수렴한다면? 이를 \int_a^b f(x)dx라고 정의한다.  
<p> $$ \int_a^b f(x)dx = \lim\limits_{\|\Gamma\|\to 0} {\sum_{i=1}^n {f(\xi)|x_i-x_{i-1}|}} $$ </p>
더 정확히는, 임의의 \Gamma, \xi 및 \epsilon에 대하여, \|\Gamma\| < \delta(\epsilon) 일 때 \|리만합-I\|<\epsilon인 \delta(\epsilon)이 존재한다면 리만 적분값 I가 정의된다.  

다르부 적분이라는 개념도 있는데, 어떠한 분할 \Gamma 에 대하여,
* 가장 넓이를 크게 태그를 고르는 상합 U(f, \Gamma)=\sum\limits_{i=1}^n \sup f([x_{i-1}, x_i])(x_i-x_{i-1})
* 가장 넓이를 작게 태그를 고르는 하합 L(f, \Gamma)=\sum\limits_{i=1}^n \inf f([x_{i-1}, x_i])(x_i-x_{i-1})

이 2가지를 정의하고, 상합에 대하여 \Gamma\to 0으로 보냈을 때 가장 큰 적분값인 상적분이 정의되며, 하합에 대해선 하적분이 정의된다.  
상적분과 하적분 값이 I로 같으면 적분값이 정의된다.

파티션 나누는거에 따라서 값이 달라지면 오또케요 라고 생각할 수 있는데  
\|\Gamma\|\to 0으로만 보낸다면 파티션이랑은 관련없이 같은 값으로 수렴한다는게 증명된단다. 암튼 그렇다고 함.  
고로 우리는 머리굴릴 필요 없이 가장 편한 균등분할로 나누면 된다.  


<br/>

결국, n\to\infty로 보내버리면 구분구적법의 넓이가 실제 넓이의 참값에 수렴한다는 사실은 리만 적분이 가능한 함수에 한정되는 것이다.  
그럼 어떤 함수가 리만 적분 가능한가?  

정답은, 적분 영역 내에서 불연속인 점을 모은 집합이 measure zero 집합인 경우라고 하는데,  
좀 더 풀어 쓰면, 불연속인 점들을 모아서 집합을 만들면, 그게 유한 집합이거나 [가산 무한 집합](https://ko.wikipedia.org/wiki/%EA%B0%80%EC%82%B0_%EC%A7%91%ED%95%A9)인 경우에 해당된다.

가산 무한 집합은, 그 집합을 자연수 집합으로 보내는 단사 함수가 존재하는 집합,  
즉 자연수보다 크기가 작거나 같은(\aleph_0) 집합이다.  
실수의 크기는 \aleph_1=2^{\aleph_0}이므로, 불연속점의 크기가 \aleph_0 만큼 되어 봤자 씹을 수 있다는 뜻 ㅎ 
 
<br/>
 


{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_정적분" %}



## 기하와 벡터
TBD

# 미적분학
TBD

# TO BE DONE!
