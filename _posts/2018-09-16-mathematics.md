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
2년간 매일같이 쳐다보던 고등학교 수학도 안쓰다보면 결국 까먹는다. 하느님  
본인이 12년도 고등학교 입학이라 그 당시 교육과정을 따른다. 책이 그거밖에 없음  

내용 구분은 보통 개념 단위로 정리할 예정이지만, 예외로 고등학교 수학과정은 단원 단위로 정리한다.  
내맘임  

- 쓰다 보니 삼천포로 오지게 빠져대서 고등학교 수학이라 하기엔 좀 민망한 수준이 되어버린것이다.  
  물론 이걸 보는 사람이 있겠냐만은,,, 만약 본인이 고등학생이고 과고 정도 수준 미만이라면 그냥 빨간버튼 내용은 이해가 안되는게 있는게 정상이니 모르겠다면 그러려니 하자.


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
* 명제 $p$ 혹은 조건 $p(x)$에 대해 $p(x)$가 아니다 를 $p(x)$의 부정이라 하고, $\sim p(x)$로 표기함.

<p> $$ \sim (p \vee q) \Leftrightarrow (\sim p \wedge \sim q)
\quad \sim (p \wedge q) \Leftrightarrow (\sim p \vee \sim q) $$ </p>
<p> $$ \sim (\forall x, p(x)) \Leftrightarrow (\exists x, \sim p(x)),
\quad \sim (\exists x, p(x)) \Leftrightarrow (\forall x, \sim p(x))$$ </p>

<br/>

### 진리집합
* $p(x)$를 만족하는 $x$ 전체의 집합 $P$를 조건 $p(x)$의 진리집합이라고 한다.
* $P = \left\\{ x \mid x \in U, p(x) \right\\}$. 표기시 전체집합 $U$를 씹으려는 경향이 강하므로 $P=\left\\{ x \mid p(x) \right\\}$로도 표기.

<br/>

### 조건과 집합
* 집합 $P$, $Q$를 조건 $p$, $q$의 진리집합이라고 둘 때,

<p> $$ P \subset Q \Leftrightarrow (p \Rightarrow q)
\quad P \nsubseteq Q \Leftrightarrow (p \nLeftarrow q), \\
p \vee q \Leftrightarrow P \cup Q
\quad p \wedge q \Leftrightarrow P \cap Q
\quad \sim p \Leftrightarrow P^c $$ </p>

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
* $ \sim (p \vee q) \Rightarrow (P \cup Q)^c \Rightarrow (P^c \cap Q^c) \Rightarrow (\sim p \wedge \sim q) $
* $ \sim$ (모든 $x$에 대하여 $p(x)$이다) $\Rightarrow \sim (p(x_1) \; and \; p(x_2) \; and \; \cdots \; and \; p(x_n))$ <br/>
  $ \Rightarrow (\sim p(x_1)) \; or \; (\sim \; p(x_2)) \; or \; \cdots \; or \; (\sim p(x_n)) \Rightarrow$ 어떤 $x$에 대하여 $\sim p(x) $ <br/>
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
* $A > B$인 임의의 자연수 $A$, $B$가 있을 때, $A = B \cdot Q + R$로 몫과 나머지를 분리하면 <br/>
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
r_{i+1}=r_{i−1}−q_i r_i, \quad q_i=\lfloor\frac{r_{i−1}}{r_i}\rfloor $$ </p>

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
$\overline{AB}^2 + \overline{AC}^2 = 2(\overline{AM}^2 + \overline{BM}^2)$
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
* 점$(x_1, y_1)$과 직선 $ax+by+c=0$ 사이의 거리 $d=\frac{\left\|ax_1+by_1+c\right\|}{\sqrt{a^2+b^2}}$
{% endcapture %}

{% capture context2 %}
### 서로 수직인 두 직선
* $y=ax+b, y=a'x+b'$이 수직이라면, <br/>
  $\tan(\theta_1)=a, \tan(\theta_2)=\tan(\theta_1+\frac{\pi}{2})=-\frac{1}{\tan(\theta_1)}=a'$ <br/>
  $ \therefore a'=-\frac{1}{a}, aa'=-1 $

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
    $n=y_1-mx_1, x_1^2+y_1^2=r^2$
  * 열심히 대입하면 $y_1^2 m^2 + 2x_1 y_1 m + x_1^2=(y_1 m + x_1)^2 = 0, m=-\frac{x_1}{y_1}$ <br/>
  * 그래서 접선의 방정식은 $y-y_1=-\frac{x_1}{y_1}(x-x_1), x_1x + y_1 y=r^2$가 된당  <br/>

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
* 도형의 방정식 $f(x, y)=0 \rightarrow f(x-a, y-b)=0$

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
* $y=ax^2+bx+c$에서 $y$의 범위는 $0=ax^2+bx+(c-y)$에서 $D \geq 0$를 사용해도 됨

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
       (x_i>0, \alpha_i>0, \alpha = \alpha_1 + \cdots + \alpha_n) $$ </p>

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
* 방향을 따져서 아래로 볼록이라고 하고 위로 오목이라고도 한다.

----------------

* 머암튼 $f:(a,b) \longrightarrow R$가 연속인 (아래로) 볼록 함수라면, 젠센 부등식은
  <p> $$ \forall x_i \in (a, b), p_i > 0, \sum_{i=1}^{n} {p_i} = 1 \; 일 \, 때 \; f\left(\sum_{i=1}^{n} {p_i x_i}\right) \leq \sum_{i=1}^{n} {p_i f(x_i)} $$
* 대충 말로 풀면 '평균의 함숫값보다 함숫값의 평균이 더 크다'
* 볼록 방향 바뀌면 부등호 방향도 바뀜
* 증명은 [수학적 귀납법](http://suhak.tistory.com/221)으로.

<br/>

### (가중) 산술기화조화 증명
* 산술-기화-조화 평균 부등식도 사실 귀납법으로 증명이 된다. 하지만 가중치까지 넣어서 바로 젠센부등식으로 증명해보면
  * 아래로 볼록한 만만한 함수 $f(x)=-\ln(x)$ 로 두고
<p> $$
  \begin{align*}
    \alpha_1 + \alpha_2 + \cdots + \alpha_n = \alpha,\; & w_i = \frac{\alpha_i}{\alpha} \\
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
  * 산술 기화평균 부등식에 따라 <br/>
    $\sqrt{\dfrac{a_i^2}{A^2} \dfrac{b_i^2}{B^2}} \leq \dfrac{1}{2}\left(\dfrac{a_i^2}{A^2}+\dfrac{b_i^2}{B^2}\right)$
  * 이걸 $i=1$ 부터 $n$에 대한 부등식을 모두 더하면 우변은 1이 되고, 결국 $\sum\limits_{i=1}^{n} {\sqrt{a_i^2 b_i^2}} \leq AB$로 증명된다. <br/>

<br/>
* [재배열 부등식](https://namu.wiki/w/%EC%9E%AC%EB%B0%B0%EC%97%B4%20%EB%B6%80%EB%93%B1%EC%8B%9D) 도 볼만함

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_최대와_최소" %}

### 삼각함수의 정의
* 호도(radian)법: $l=r\theta, \; S=\frac{1}{2}r^2\theta=\frac{1}{2}rl, \; 1\,rad = \frac{180\circ}{\pi}$
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
* $1 + \tan^2\theta = \frac{1}{\cos^2 \theta}$
* $\sin(\pi-\theta)=\sin\theta, \cos(\pi-\theta)=-\cos\theta, \tan(\pi-\theta)=-\tan\theta$
* $\sin(\frac{\pi}{2}-\theta)=\cos\theta, \cos(\frac{\pi}{2}-\theta)=\sin\theta, \tan(\frac{\pi}{2}-\theta)=\frac{1}{\tan\theta}$

<br/>
![Alt text](/pictures/mathematics/사인법칙.jpg)
* 사인법칙 $\dfrac{a}{\sin A}=\dfrac{b}{\sin B}=\dfrac{c}{\sin C}=2R$
* 제1 코사인법칙 $a=b\cos C + c\cos B$
* 제2 코사인법칙 $a^2=b^2+c^2-2bc\cos A$
* $\vartriangle ABC$의 넓이 $S=\frac{1}{2}bc \sin A = \sqrt{s(s-a)(s-b)(s-c)} \quad (2s=a+b+c)$

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
  
* 벡터로 쉽게 증명가능하다. $\mathbf{c}=\mathbf{a}-\mathbf{b}$로 두면  
  * $c^2=\mathbf{c} \cdot \mathbf{c}=(\mathbf{a}-\mathbf{b})\cdot(\mathbf{a}-\mathbf{b})=a^2+b^2-2ab\cos\theta$

<br/>

### 헤론의 공식
이걸 증명해야하나 싶긴한데
* $S=\frac{1}{2}bc \sin A$
* $\sin^2 A = 1-\cos^2 A = (1+\cos A)(1-\cos A)이고 \cos A=\frac{b^2+c^2-a^2}{2bc}$이다.
* 쑤셔넣고 정리하면 $\sin A=\frac{2}{bc}\sqrt{s(s-a)(s-b)(s-c)} \; (2s=a+b+c)$라서 증명된다.

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="고등수학_삼각함수_공식" %}

순열과 조합은 확통 가서 다시 정리함

## 수학 1

### 행렬
* $A=(a_{ij})=\begin{pmatrix} a_{11} & a_{12} \\\\ a_{21} & a_{22} \end{pmatrix}$
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
\text{where }adj(A) &= [\bar{A_{ij}}]^t, \; \bar{A_{ij}} = (-1)^{i+j}\left|M_{ij}\right| \end{align}$$ </p>

어... 난감하다 <br/>
하나씩 보자

* $adj(A)$
  * Adjoint Matrix로써 위 정의 $adj(A) = [\bar{A_{ij}}]^t$ 를 따른다.

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
  * $a>0$에 대하여 $a^{\frac{m}{n}}=\sqrt[n]{a^m}$

3. 실수 범위로 확장
  * $a>0, b>0$에 대하여 $a^x a^y=a^{x+y}, \dfrac{a^x}{a^y} = a^{x-y}, (a^x)^y=a^{xy}, (ab)^x=a^x b^x$

<br/>

### 로그의 성질
$a>0$, $a\neq 1$, $x>0$, $y>0$일 때
* $\log_a{1}=0, \log_a{a}=1$
* $\log_a{xy}=\log_a{x}+\log_a{y}, \; \log_a{\dfrac{x}{y}}=\log_a{x}-\log_a{y}$
* $\log_a{x^n}=n\log_a{x}$
* $\log_a{b}=\dfrac{\log_c{b}}{\log_c{a}}, \; \log_a{b}=\dfrac{1}{\log_b{a}}$

<br/>

### 지수함수와 로그함수
* $y=\log_a{x}$의 역함수는 $y=a^x$이기 때문에 둘은 $y=x$에 대칭임

{% endcapture %}

{% capture context2 %}

### 로그 성질 증명
$\log_a{xy}=\log_a{x}+\log_a{y}$
* $\log_a{x}=m,\; \log_a{y}=n$이라 하면, $x=a^m,\; y=a^n,\; xy=a^{m+n}$에서 $\log_a{x}+\log_a{y}=m+n=\log_a{xy}$

<br/>

$\log_a{b}=\dfrac{\log_c{b}}{\log_c{a}}$
* $\log_a{b}=x$라 하면 $b=a^x, \; \log_c{b}=\log_c{a^x}=x\log_c{a}, \; \log_a{b}=x=\dfrac{\log_c{b}}{\log_c{a}}$

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
그러니까 어떤 구조 $X$를 함수 $f:X \longrightarrow Y$ 에 넣어서 $Y$가 됐어도, $Y$ 안에 $X$의 모든 정보가 담겨있다는 것이며 <br/>
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
    $f\left(x-\frac{1}{n}\right)=\alpha \div f\left(\frac{1}{n}\right) < f(x) = \beta = \alpha+\epsilon < f\left(x+\frac{1}{n}\right) = \alpha \times f\left(\frac{1}{n}\right)$
  * 근데 $\epsilon > 0$이라고 가정하면, <br/>
    $\alpha+\epsilon < \alpha * f\left(\frac{1}{n}\right), \; 1+\frac{\epsilon}{\alpha} < f\left(\frac{1}{n}\right)$ <br/>
    여기서 식은 임의의 자연수 $n$에 대해서 성립해야 하므로, $n$를 미친놈마냥 크게 두면 그딴 $\epsilon$은 존재하지 않음
  * $\epsilon < 0$일때도 마찬가지로 하면 된다. 아무튼 모순임.
- 보충:
  * 우선 $f(1) = c > 0$라고 하자.
  $y = x$ 대입하면 $f(x+x)=f(x) \cdot f(x) = f(x) * f(x)$.
  수학적 귀납법으로 자연수 $n$에 대해 $f(nx) = f(x) * f(x) * \cdots * f(x)$.
  $x = \frac{1}{n}$ 넣으면 $f(1)=f(\frac{1}{n})^n$이고 따라서 $f\left(\frac{1}{n}\right) = \sqrt[n]{c}$.
  * $c > 1$일 때 $f(\frac{1}{n}) \geq 1$이고 따라서 $f\left(x+\frac{1}{n}\right) = f(x) \cdot f\left(\frac{1}{n}\right) > f(x)$.
  그래서 $f\left(x-\frac{1}{n}\right) < f(x) < f\left(x+\frac{1}{n}\right)$.
  * $c < 1$일 때는 부등호 반대로 하면 되고, $c=1$이면 $f \equiv 1$임을 적당히 잘 보일 수 있음

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
* 등차수열 $a_n=a+(n-1)d, \; S_n=\dfrac{n(2a+(n-1)d)}{2}$
* 등비수열 $a_n=ar^{n-1}, \; S_n=\dfrac{a(1-r^n)}{1-r}=\dfrac{a(r^n-1)}{r-1} \; (r \neq 1)$
* $\sum\limits_{k=1}^{n} {k^2} = \dfrac{n(n+1)(2n+1)}{6}, \quad \sum\limits_{k=1}^{n} {k^3} = \left(\dfrac{n(n+1)}{2}\right)^2$
* $\sum\limits_{k=1}^{n} {\dfrac{1}{k(k+1)}} = \sum\limits_{k=1}^{n} {\dfrac{1}{k} - \dfrac{1}{k+1}} = 1-\dfrac{1}{n+1}$
* $\sum\limits_{k=1}^{n} {\dfrac{1}{\sqrt{k} + \sqrt{k-1}}} = \sum\limits_{k=1}^{n} {\sqrt{k} - \sqrt{k-1}} = \sqrt{n}$

{% capture context1 %}
증명은 다음단계에
{% endcapture %}

{% capture context2 %}
### 등차수열의 합
* $S_n = a + (a+d) + (a+2d) + \cdots + (a+(n-1)d)$
* $S_n = (a+(n-1)) + (a+(n-2)d) + (a+(n-3)d) + \cdots + a$
* $2S_n = (2a+(n-1)d) \times n, \; S_n = \frac{n(2a+(n-1)d)}{2}$

<br/>

### 등비수열의 합
* $S_n = a+ar+ar^2+\cdots\+ar^{n-1}$
* $rS_n= ar+ar^2+ar^3+\cdots\+ar^{n}$
* $(1-r)S_n=a-ar^n = a(1-r^n), \; S_n = \dfrac{a(1-r^n)}{1-r}=\dfrac{a(r^n-1)}{r-1} \; (r\neq 1)$

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
  * $a_{n+1}-\alpha = p(a_n - \alpha)$ 꼴로 변형 $(\alpha=\frac{q}{1-p})$하면
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
자연수 체계를 묘사하는 5개의 공리를 모아놓은 [페아노 공리계](https://ko.wikipedia.org/wiki/%ED%8E%98%EC%95%84%EB%85%B8_%EA%B3%B5%EB%A6%AC%EA%B3%84) 에서는
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
* $ a_n = S_n - S_{n-1} (n \geq 2), \lim\limits_{n \to \infty} {a_n} = \lim\limits_{n \to \infty} {S_n - S_{n-1}} = S-S = 0 $
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
                           &= \sqrt{a^2+b^2}\cos(\theta-\beta)
\end{align}$$</p>
* 아님 그냥 간단하게 $\sin(\theta+\alpha) = \sin\left(\theta+\frac{\pi}{2}-\beta\right) = cos(\theta - \beta)$

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
고등학교에서는 교육과정 순서때문에 $e$를 $\lim\limits_{x\to 0} (1+x)^{\frac{1}{x}}$로 정의하지만,  
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
2. $x=0$에서 지수함수 $f(x)=a^x$의 기울기가 1이 되는 $a$이며, 동시에 $ce^x$는 $\frac{df(x)}{dx}=f(x)$ 인 유일한 함수이다.
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
* 도함수 $f'(x)=\dfrac{d}{dx}f(x) = \lim\limits_{\Delta x\to 0} {\dfrac{f(x+\Delta x)-f(x)}{\Delta x}} 
= \lim\limits_{h\to 0} {\dfrac{f(x+h)-f(x)}{h}} = \lim\limits_{t\to x} {\dfrac{f(t)-f(x)}{t-x}}$  

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
* $f(x)$가 어떤 구간에 속하는 $x$에서 모두 미분가능할 때, $f(x)$는 그 구간에서 미분가능하다고 한다.

<br/>

* 미분가능한 함수는 연속인 함수의 충분조건이다.  
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
4. $\{f(x)\pm g(x)\}'=f'(x)\pm g'(x)$
5. $\{f(x)g(x)\}'=f'(x)g(x) + f(x)g'(x)$

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
    * $f^{(1)} = f', \; f^{(2)} = f'', \; f^{(3)}=f''', \quad f^{(n)} = f\, \overset{n}{\overbrace{' '\cdots'}}$
    
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
* $dy=\frac{\partial y}{\partial x_1}dx_1 + \frac{\partial y}{\partial x_2}dx_2+ \cdots + \frac{\partial y}{\partial x_n}dx_n$ 에서 $dx_i$의 계수: $x_i$방향으로의 기울기

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
* $F'(x)=f(x)$일 때 $F(x)$를 $f(x)$의 부정적분이라고 함. $\displaystyle\int f(x)dx=F(x)+C,\; \displaystyle\int\left(\dfrac{d}{dx}f(x)dx\right)=f(x)+C$  
* 치환적분: $\displaystyle\int f(g(x))g'(x)dx=\displaystyle\int \left(f(t)\dfrac{dt}{dx}\right)=\displaystyle\int f(t)dt$  
* 부분적분: $\displaystyle\int f'(x)g(x)dx=f(x)g(x)-\displaystyle\int f(x)g'(x)dx,\; \displaystyle\int u'vdx=uv-\displaystyle\int uv'dx$

{% capture context1 %}
### 정의
* $F'(x)=f(x)$에서 $F(x)$로부터 $f(x)$를 구하는 연산을 미분(differentiation)이라고 하고 $f(x)$를 도함수(derivative)라고 한다면    
* 반대로 $f(x)$로부터 $F(x)$을 구하는 연산을 부정적분이라고 하며  
* $F(x)$는 역도함수(antiderivative), 원함수, 원시함수(primitive function)이라고 부른다.

<br/>

### 부정적분의 계산
1. $\displaystyle\int kdx=kx+C$
2. $\displaystyle\int x^n dx=\dfrac{1}{n+1}x^{n+1}+C (r\in\mathbb{R},\; n\neq 1)$
    * $\displaystyle\int x^{-1} dx=\ln \|x\|+C$ 
3. $\displaystyle\int kf(x)dx=k\displaystyle\int f(x)dx$
4. $\displaystyle\int \left(f(x)\pm g(x)\right)dx = \displaystyle\int f(x)dx \pm \displaystyle\int g(x)dx$
5. $\displaystyle\int \sin x dx=-\cos x+C,\; \displaystyle\int \cos xdx=\sin x+C$  
   $\displaystyle\int \sec^2 xdx=\tan x+C,\; \displaystyle\int \csc^2 xdx=-\cot x+C$  
   $\displaystyle\int \sec x\tan xdx=\sec x+C,\; \displaystyle\int \csc x\cot xdx=-\csc x+C$
6. $\displaystyle\int a^x dx=\dfrac{a^x}{\ln a}+C$
{% endcapture %}

{% capture context2 %}
### 잡소리
부정적분은 미분의 역연산으로 정의된다.  
적분은 원래 함수의 넓이를 구하려고 생긴 것인데, 그건 정적분이고  
함수의 넓이를 구하는 정적분과 함수의 기울기를 구하는 미분과의 관계를 나타낸 것이 미적분학의 제 1 기본정리이며  
정적분이 부정적분의 차로 계산됨을 나타낸 것이 미적분학의 제 2 기본정리이다.

<br/>

### 부정적분의 계산 증명
$\displaystyle\int \left(f(x)\pm g(x)\right)dx = \displaystyle\int f(x)dx \pm \displaystyle\int g(x)dx$
* $\dfrac{d}{dx}\left(\displaystyle\int f(x)dx\pm \displaystyle\int g(x)dx\right)=\dfrac{d}{dx}\left(\displaystyle\int f(x)dx\right)\pm\dfrac{d}{dx}\left(\displaystyle\int g(x)dx\right)=f(x)\pm g(x)$
* $\therefore \displaystyle\int f(x)dx \pm \displaystyle\int g(x)dx +C = \displaystyle\int \left(f(x)\pm g(x)\right)dx$
* 위 식은 임의의 $f(x),\; g(x)$에 대하여 성립하므로, $f(x)=g(x)=0$으로 두면 $C=0$


나머지 식들도 위와 비슷하게 한다.

<br/>

### 치환적분 증명, infinitesimal differential
$y=\displaystyle\int f(t)dt$라고 두자  
chain rule에 의하여, $\dfrac{dy}{dx}=\dfrac{dy}{dt}\cdot \dfrac{dt}{dx}=f(t)\dfrac{dt}{dx}=f(g(x))g'(x)$  
$\therefore, y=\displaystyle\int f(t)dt =\displaystyle\int \left(f(t)\dfrac{dt}{dx}\right)= \displaystyle\int f(g(x))g'(x)dx$
  
위 예시던, 미분의 chain rule에서던, 기타등등  
$dx,\, dy$와 같은 미분소(differential)가 곱해지고 cancel out되고 등등 실제 변수마냥 취급되는 것을 확인할 수 있다.  
미분소가 항상 분자/분모 형태로 묶여 나오던 미분파트와는 다르게, 적분에서는 미분소가 $\int dx$로 묶여 나오면서 $dx$라는 term이 따로 노는 형태가 처음 등장하는데,    
이때 $\left(\dfrac{dy}{dx}\right)dx$가 어떻게 $dy$가 되는지, 그러니까 $dx$를 왜 실제 변수처럼 취급하여 cancel out할 수 있는지,  
더 근본적으로는, 그래서 $dx$가 정확히 무엇인지 궁금했었다.   
* 물론 위 식 $\displaystyle\int f(t)dt =\displaystyle\int \left(f(t)\dfrac{dt}{dx}\right)$에서 간접적으로 보여지긴 한다만, 그래도 직관적이진 않았다.

<br/>

여기에 대한 해답은 [위키 링크](https://en.wikipedia.org/wiki/Differential_(infinitesimal))로 일단 대체한다.  
솔직히 아직 완전히 이해가 된건 아니고, 위 링크도 뭔가 속시원한 답을 주진 않는 것 같다. 

미분의 여러 notations 들 중, 왜 하필이면 라이프니츠의 표기법이 승리했는지를 알 수 있다.  
미분이라는 것을 $',\, \cdot,\, D$와 같이 하나의 기본 연산자가 아니라, $dy$와 $dx$ 두 미분소의 결합으로 두었기 때문에  
$\left(\dfrac{dy}{dx}\right)dx=dy$ 이라는 직관적 표현이 다른 표기법으로는 죽었다 깨어나도 불가능하기 때문.  

<br/>

### 부분적분 증명
$\displaystyle\int f'(x)g(x)dx=f(x)g(x)-\displaystyle\int f(x)g'(x)d$
* 곱의 미분법에 의하여, $\left\\{f(x)g(x)\right\\}'=f'(x)g(x)+f(x)g'(x)$  
* 이걸 부정적분하면, $f(x)g(x)+C =\displaystyle\int f'(x)g(x)dx + \displaystyle\int f(x)g'(x)dx$  
* 임의의 $f(x), g(x)$에 대하여 성립해야 하므로, $f(x)=g(x)=0$으로 두면 $C=0$  
* $\therefore \displaystyle\int f'(x)g(x)dx=f(x)g(x)-\displaystyle\int f(x)g'(x)dx, \; \displaystyle\int u'vdx=uv-\displaystyle\int uv'dx$


부분적분에서는 함수를 적분될 놈($u$)이랑 미분될 놈($v$)으로 구분하는게 제일 중요한데,  
미분 우선순위는 $\ln x \to\; x^n \to\; \sin x \to\; e^x$ 순서대로 좋다(미분해서 빨리 조질 수 있는 형태).

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_부정적분" %}

### 정적분
* 구분구적법의 극한 $\lim\limits_{n\to\infty}{\sum\limits_{k=1}^{n} {f(x_k)\Delta x}}=\int_a^b {f(x)dx}$  
* $\displaystyle\int_a^b {f(x)dx}=\left[F(x)\right]_a^b=F(b)-F(a)$  

{% capture context1 %}
### 구분구적법과 정적분
![Alt text](/pictures/mathematics/정적분.jpg)  
넓이를 구하는데 사용되는 적분이라는 개념의 시초  
$[a, b]$에서 연속인 어떤 함수 $f(x)$를 $n$등분하여 각 분점의 $x$좌표를 $x_0(=a), x_1, \cdots x_n(=b)$로 두었을 때,  
$\Delta x=\dfrac{b-a}{n}$으로 두면, $[a, b]$ 구간에서 $f(x)$ 그래프의 넓이를 다음과 같이 근사할 수 있다.
<p> $$ S_n \simeq \sum\limits_{k=1}^n {f(x_k)\Delta x} $$</p>

이때 $n\to\infty$로 보내버리면 $S_n$은 실제 넓이의 참값에 수렴하게 되는데, 이를
<p> $$ S=\lim\limits_{n\to\infty} S_n = \lim\limits_{n\to\infty} {\sum\limits_{k=1}^n {f(x_k)\Delta x}} =\int_a^b f(x)dx $$</p>
로 표현한다.

<br/>

### 정적분의 계산
* $\displaystyle\int_a^a f(x)dx=0$
* $\displaystyle\int_a^b f(x)dx=-\displaystyle\int_b^a f(x)dx$
* $\displaystyle\int_a^b kf(x)dx=k\displaystyle\int_a^b f(x)dx$
* $\displaystyle\int_a^b \left\\{f(x)\pm g(x)\right\\}dx=\displaystyle\int_a^b f(x)dx \pm \displaystyle\int_a^b g(x)dx$
* $\displaystyle\int_a^b f(x)dx=\displaystyle\int_a^c f(x)dx+\displaystyle\int_c^b f(x)dx$

<br/>

* $g(a)=\alpha, g(b)=\beta \Rightarrow \displaystyle\int_a^b f(g(x))g'(x)dx=\displaystyle\int_{\alpha}^{\beta} f(t)dt$
* $\displaystyle\int_a^b f'(x)g(x)dx=\left[f(x)g(x)\right]_a^b-\displaystyle\int_a^b f(x)g'(x)dx$
* $f(-x)=f(x) \Rightarrow \displaystyle\int_a^a f(x)dx=2\displaystyle\int_0^a f(x)dx$
* $f(-x)=-f(x) \Rightarrow \displaystyle\int_a^a f(x)dx=0$
* $\dfrac{d}{dx} \displaystyle\int_{h(x)}^{g(x)} f(t)dt=f(g(x))g'(x)-f(h(x))h'(x)$

{% endcapture %}

{% capture context2 %}
### 미적분학의 기본정리
위에서 잠깐 언급했지만, 미적분학의 기본정리는 
* 함수의 기울기를 구하는 미분
* 함수의 넓이를 구하는 적분

이 관련없어 보이는 두 개념을 서로 연관시키는 2가지의 정리이다.

<br/>

#### 제1 기본정리
함수 $f$가 닫힌구간 $[a,b]$에서 연속이면,  
함수 $F(x)=\displaystyle\int_{a}^{x}f(t)\,dt$ 는 닫힌구간 $[a,b]$에서 연속이며 열린구간 $(a,b)$에서 미분이 가능하고,  
함수 $F$의 도함수는 $f$이다.

pf)  
$x,x+h\in [a,b]$ 일 때,  
<p> $$\begin{align*}
F'(x)&=\lim_{h\to 0} {\frac{F(x+h)-F(x)}{h}} \\
     &=\lim_{h\to 0} {\frac{1}{h}\left[\int_{a}^{x+h} f(t)\,dt - \int_{a}^{x} f(t)\,dt\right]} \\
     &=\lim_{h\to 0} {\frac{1}{h}\int_{x}^{x+h} f(t)\,dt}
\end{align*}$$ </p> 
 
이때, [적분의 평균값 정리](https://ko.wikipedia.org/wiki/%ED%8F%89%EA%B7%A0%EA%B0%92_%EC%A0%95%EB%A6%AC#%EC%A0%81%EB%B6%84_%ED%8F%89%EA%B7%A0%EA%B0%92_%EC%A0%95%EB%A6%AC)에 의해   
$c\in [x,x+h]:\; \dfrac{1}{h} \displaystyle\int_{x}^{x+h}f(t)\,dt=f(c)$  
함수 $f$는 주어진 구간에서 연속이므로, [샌드위치 정리](https://en.wikipedia.org/wiki/Squeeze_theorem)에 의해 $h$가 작아짐에 따라 $x+h$는 $x$에 다가가고, 그러므로 $c$도 $x$에 다가간다.  
$\therefore \lim\limits_{h\to 0}f(c)=f(x)$
  
<p> $$\begin{align*}
F'(x)&=\lim_{h\to 0}{\frac{1}{h}} \int_{x}^{x+h}f(t)\,dt\\
     &=\lim_{h\to 0}f(c)\\
     &=f(x)
\end{align*}$$ </p>

-------------------

<br/>

#### 제2 기본정리
함수 $f$가 닫힌구간 $[a,b]$에서 연속이며, 함수 $F$가 $f$의 임의의 부정적분이면, $\displaystyle\int_{a}^{b}f(t)dt=F(b)-F(a)$

pf)  
함수 $G$를 $G(x)=\displaystyle\int_{a}^{x}f(t)\,dt$ 으로 정의하면, 제1 기본정리에 의해 $G(x)$의 도함수는 $f(x)$가 되기 때문에 $G(x)=\displaystyle\int f(x)dx +C'$ 이다.  
또 함수 $F$는 $f$의 임의의 부정적분이랬으니 $F(x)=\displaystyle\int f(x)dx+C''$이며,  
정리하면 $F(x)=G(x)+C$ 가 된다.
  
$F$와, (제1 기본정리에 의해) $G$는 $[a,b]$에서 연속이므로,
<p> $$\begin{align*}
F(b)-F(a)&=\left[G(b)+C\right]-\left[G(a)+C\right] \\
         &=G(b)-G(a) \\
         &=\int_{a}^{b} f(t)\,dt-\int_{a}^{a}f(t)\,dt \\
         &=\int_{a}^{b} f(t)\,dt-0 \\
         &=\int_{a}^{b} f(t)\,dt
\end{align*}$$ </p>

<br/> 
 
좀 더 엄밀한 증명은 [영어위키](https://en.wikipedia.org/wiki/Fundamental_theorem_of_calculus)를 참조하면 되는데 그렇게까지 살아야될거같진 않다. 

<br/>

### 리만 적분
위에서, 구분구적법 $ S_n \simeq \sum\limits_{k=1}^n {f(x_k)\Delta x} $에서 $n\to\infty$로 보내버리면 $S_n$은 실제 넓이의 참값에 수렴한다고 했다.  
진짜?  
않이... 왜?

좀 더 엄밀하게 다뤄보자.  
하악  


일단 [리만 적분](http://mathnmath.tistory.com/95)이라는걸 정의해보자.  
![Alt text](/pictures/mathematics/구분구적법.jpg)  
급식때에는 각 구간을 양심적으로 $n$등분하고, 함수값은 각 구간의 왼쪽(혹은 오른쪽) 구간을 선택했다.  
이걸 일반화한게 리만 적분인데, 일반화한 부분은
1. 구간을 균등하게 자르지 않고 내맘대로 자른다.
    * partition $\Gamma = \\{x_0=a, x_1, x_2, \cdots, x_{n-1}, x_n=b \\}$
    * 임의의 $x_i$는 $[a, b]$ 구간 안에만 있음 된다. 심지어 $x_i < x_{i+1}$일 필요도 없이 내맘대로인데 편의상 $x_i < x_{i+1}$로 둔다.
    * $\Gamma$의 norm을 $\displaystyle\max_i \|x_i-x_{i-1}\|$, 그러니까 모든 subinterval의 가장 큰 길이를 norm으로 정의한다.
2. 각 구간에서, 함수값을 어느 것으로 선택할지 내맘대로 고른다.
    * $\min(x_{i-1}, x_i) \leq \xi_i \leq \max(x_{i-1}, x_i)$
    * $\xi$ 를 태그(tag)라고 부른다.

<br/>

![Alt text](/pictures/mathematics/리만적분.jpg)  
이렇게, 구간 $[a, b]$에서 함수의 넓이를 나타낸 급수는 다음과 같다  
<p> $$ \sum_{i=1}^n {f(\xi)|x_i-x_{i-1}|} $$ </p>

얘를 리만합(Riemann sum) 이라고 한다.  

<br/>

이때 파티션의 최대 길이인 $\Gamma$의 norm을 0으로 보낼 때, 즉 모든 subinterval의 길이를 0으로 보낼 때,  
$\lim\limits_{\|\Gamma\|\to 0} {\sum\limits_{i=1}^n {f(\xi)\|x_i-x_{i-1}\|}}$가 어떠한 값으로 만약 수렴한다면? 이를 $\displaystyle\int_a^b f(x)dx$라고 정의한다.
  
<p> $$ \int_a^b f(x)dx = \lim\limits_{\|\Gamma\|\to 0} {\sum_{i=1}^n {f(\xi)|x_i-x_{i-1}|}} $$ </p>

더 정확히는, 임의의 $\Gamma$, $\xi$ 및 $\epsilon$에 대하여,  
$\|\Gamma\| < \delta(\epsilon)$ 일 때 $\|$리만합$-I\|<\epsilon$인 $\delta(\epsilon)$이 존재한다면 리만 적분값 $I$가 정의된다.  

<br/>

다르부 적분이라는 개념도 있는데, 어떠한 분할 $\Gamma$ 에 대하여,
* 가장 넓이를 크게 태그를 고르는 상합 $U(f, \Gamma)=\sum\limits_{i=1}^n \sup f([x_{i-1}, x_i])(x_i-x_{i-1})$
* 가장 넓이를 작게 태그를 고르는 하합 $L(f, \Gamma)=\sum\limits_{i=1}^n \inf f([x_{i-1}, x_i])(x_i-x_{i-1})$

이 2가지를 정의하고, 상합에 대하여 $\Gamma\to 0$으로 보냈을 때 가장 큰 적분값인 상적분이 정의되며, 하합에 대해선 하적분이 정의된다.  
상적분과 하적분 값이 $I$로 같으면 적분값이 정의된다.

파티션 나누는거에 따라서 값이 달라지면 오또케요 라고 생각할 수 있는데  
$\|\Gamma\|\to 0$으로만 보낸다면 파티션이랑은 관련없이 같은 값으로 수렴한다는게 증명된단다. 암튼 그렇다고 함.  
고로 우리는 머리굴릴 필요 없이 가장 편한 균등분할로 나누면 된다.  


<br/>

결국, $n\to\infty$로 보내버리면 구분구적법의 넓이가 실제 넓이의 참값에 수렴한다는 사실은 리만 적분이 가능한 함수에 한정되는 것이다.  
그럼 어떤 함수가 리만 적분 가능한가?  

정답은, 적분 영역 내에서 불연속인 점을 모은 집합이 measure zero 집합인 경우라고 하는데,  
좀 더 풀어 쓰면, 불연속인 점들을 모아서 집합을 만든 것이 유한 집합이거나 [가산 무한 집합](https://ko.wikipedia.org/wiki/%EA%B0%80%EC%82%B0_%EC%A7%91%ED%95%A9)인 경우에 해당된다.

가산 무한 집합은, 그 집합을 자연수 집합으로 보내는 단사 함수가 존재하는 집합,  
즉 자연수보다 크기가 작거나 같은($\aleph_0$) 집합이다.  
실수의 크기는 $\aleph_1=2^{\aleph_0}$이므로, 불연속점의 크기가 $\aleph_0$ 만큼 되어 봤자 씹을 수 있다는 뜻 
 
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_정적분" %}

### 순열조합
<table style="font-family:나눔고딕; font-size: 15px;">
<thead><tr><th colspan="5" align="center">서로 다른 $n$개의 원소에서 $r$개를 고르는 방법의 숫자.  </th></tr></thead>
<tbody>
<tr>
  <td> </td> <td>표기</td> <td>계산</td> <td>순서고려</td> <td>중복허용</td>
</tr>
<tr>
  <td>순열</td> <td>$_n\mathrm{P}_r$</td> <td>$\dfrac{n!}{(n-r)!}$</td> <td>O</td> <td>X</td>
</tr>
<tr>
  <td>중복순열</td> <td>$_n\Pi_r$</td> <td>$n^r$</td> <td>O</td> <td>O</td>
</tr>
<tr>
  <td>조합</td> <td>$_n\mathrm{C}_r$</td> <td>$\dfrac{n!}{r!(n-r)!}$</td> <td>X</td> <td>X</td>
</tr>
<tr>
  <td>중복조합</td> <td>$_n\mathrm{H}_r$</td> <td>$_{n+r-1}\mathrm{C}_r$</td> <td>X</td> <td>O</td>
</tr>
</tbody>
</table>

* 선별된 r개 중 구별되지 않는 원소가 $s, t, u, \cdots$ 만큼 있으면 $(s!t!u!\cdots)$만큼 나눈다.  
* `이항정리`: $ (a+b)^n=\,_n\mathrm{C}_0 a^n b^0+\,_n\mathrm{C}_1 a^{n-1}b^1+\cdots+\,_n\mathrm{C}_n a^0 b^n = \sum\limits _{k=0}^{n} {_n\mathrm{C}_k a^k b^{n-k}} $

{% capture context1 %}
### 순열
* 서로 다른 $n$개의 원소에서 $r$개를 택하여 순서 있게 배열하는 가능한 가짓수.  
* $_n\mathrm{P}_r=n(n-1)(n-2)\cdots (n-r+1)=\dfrac{n!}{(n-r)!}$
* 중복을 허용할 경우, $_n\Pi_r=n^r$


* 원소에 같은 것이 있는 경우, 같은 것이 각각 $p, q, r, \cdots, s(p+q+r+\cdots+s=n)$개가 있을 경우,
  * 원소 전체를 뽑는 경우엔 $\dfrac{n!}{p!\times q!\times r!\times \cdots \times s!}$
  * ![Alt text](/pictures/mathematics/최단경로.JPG) 
  * $A\to B$로 가는 최단경로의 갯수에 매칭된다.
  * 모두 뽑는게 아닌 경우엔 뽑힌 $r$개의 원소 중 같은 원소가 몇개가 되는지를 모두 따져서 일일이 더하는 개싸움이 된다.

<br/>

### 원순열
* 서로 다른 $n$개의 원소를 원형으로 배열하는 것을 원순열이라 함
* $(n-1)!$가지 배열이 존재함.
  * 회전 대칭인 경우가 $n$가지 존재하기 때문
* ![Alt text](/pictures/mathematics/원순열.png)
* 저런 탁자같은데 배열하는 갯수는 $n!$에다가 대칭인 갯수를 나눈다.


* 원순열을 뒤집는 것 까지 허용되는 경우를 염주순열이라고 함
* 이미 회전에 대해선 대칭인 경우를 모두 제거하였으므로, 좌우 반전 하나만 고려하여 2로 나눈다. $\frac{1}{2}(n-1)!$
  * 같은 원소를 포함 할 경우, 좌우가 처음부터 대칭이라서 2로 나눌 수가 없는 케이스가 또 생긴다..

<br/>

### 조합
* 서로 다른 $n$개의 원소에서 $r$개를 순서를 고려하지 않고 뽑는 가능한 가짓수,  
* $ _n\mathrm{C}_r = \dfrac{_n\mathrm{P}_r}{r!} = \dfrac{n!}{r!(n-r)!} =\, _n\mathrm{C} _{n-r} $  
* $ _{n-1}\mathrm{C} _{r-1} +\, _{n-1}\mathrm{C}_r =\, _n\mathrm{C}_r $


* 서로 다른 $n$개의 원소에서 $a, b, c$개 만큼 각각 뽑아서 분리하는 가짓수는  
  $_n\mathrm{C}_a \times _n\mathrm{C}_b \times _n\mathrm{C}_c$  
* 이때 $a=b$ 이면 각 그룹간의 구별이 불가능하므로 $2!$로 나누어 준다. $a=b=c$ 이면 $3!$으로 나눔.

<br/>

### 중복조합
![Alt text](/pictures/mathematics/중복조합.jpg)  
* 중복을 허용하는 경우, 원소를 $r$개 막대기를 $(n-1)$개로 두고 $(n+r-1)$개 슬롯에 막대기를 꽂으면 각 막대기 사이의 원소 갯수가 특정 원소의 선택횟수가 된다.  
* 즉 $ _n\mathrm{H}_r =\, _{n+r-1}\mathrm{C} _{n-1} =\, _{n+r-1}\mathrm{C}_r$

<br/>

### 이항정리
* $(a+b)^n$ 에서 $a^k b^{n-k}$의 계수는 $n$개의 곱셈항 중 $a$를 $r$번 선택하는 갯수 $_n\mathrm{C}_k$와 같다.  
* $(x+1)^n = \sum\limits_{k=0}^{n} {_n\mathrm{C}_k x^k}$ 로부터
<p> $$ \begin{align*}
       x=1 &\Rightarrow \sum\limits_{k=0}^{n} {_n\mathrm{C}_k} =\, _n\mathrm{C}_0+_n\mathrm{C}_1+_n\mathrm{C}_2 \cdots + _n\mathrm{C}_n= 2^n \\
       x=-1 &\Rightarrow \sum\limits_{k=0}^{n} {_n\mathrm{C}_k (-1)^k} =\, _n\mathrm{C}_0-_n\mathrm{C}_1+_n\mathrm{C}_2 \cdots + (-1)^n \, _n\mathrm{C}_n = 0 \\
       \left. \dfrac{d}{dx}(x+1)^n \right|_{x=1} &= \sum\limits_{k=0}^{n} {_n\mathrm{C}_k k\cdot1^{k-1}} =\, _n\mathrm{C}_1+2_n\mathrm{C}_2 \cdots + n_n\mathrm{C}_n=n\cdot 2^{n-1} \\
       \left. \dfrac{d}{dx}(x+1)^n \right|_{x=-1} &= \sum\limits_{k=0}^{n} {_n\mathrm{C}_k k(-1)^{k-1}} =\, _n\mathrm{C}_1-2_n\mathrm{C}_2 \cdots + (-1)^n\cdot n_n\mathrm{C}_n=0 \\
\end{align*} $$ </p>

{% endcapture %}

{% capture context2 %}
### 이항계수
이항계수 $\displaystyle{n\choose k}$를 $(x+y)^n$을 전개하였을 때 음이 아닌 정수 $k\leq n$에 대한 $x^k y^{n-k}$ 항의 계수로 정의하면   
$(x+y)^n=\sum\limits_{k=0}^{n} \displaystyle{n\choose k}x^k y^{n-k}$가 된다.  
* 이때 $\displaystyle{n\choose k}$는 $_n\mathrm{C}_k$와 동일함을 수학적 귀납법으로 증명 가능하다. [증명](https://ko.wikipedia.org/wiki/%EC%9D%B4%ED%95%AD_%EC%A0%95%EB%A6%AC)


$k\in \mathbb{N}$ 을 확장시켜, 복소수 값을 가지는 $\alpha\in \mathbb{C}$로 확장시킬 수 있다.  
<p> $$ (x+y)^\alpha=\sum\limits_{k=0}^{\infty} {\alpha\choose k}x^{\alpha-k} y^{k} = x^{\alpha} + \alpha x^{\alpha-1} + \dfrac{\alpha(\alpha-1)}{2}x^{\alpha-2}y^2 + cdots$$ </p>  

$\|x\|>\|y\|$일 때, $\displaystyle{\alpha\choose k} = \dfrac{\alpha(\alpha-1)(\alpha-2)\cdots(\alpha-k+1)}{k!}$가 성립한다고 하는데 아니면 왜 아닌지는 잘 몰겠다.  
몰라 

<br/>

### 다항정리
<p> $$(x_{1}+x_{2}+\cdots +x_{m})^{n}=\sum _{k_{1},k_{2},\dots ,k_{m}\in \mathbb {N} }^{k_{1}+k_{2}+\cdots k_{m}=n}{\dfrac {n!}{k_{1}!k_{2}!\cdots k_{m}!}}x_{1}^{k_{1}}x_{2}^{k_{2}}\cdots x_{m}^{k_{m}}=\sum _{K\in \mathbb {N} ^{m}}^{|K|=n}{\binom {n}{K}}x^{K}$$ </p>  
이 때 이항 계수에 대응되는 다항 계수 $ \displaystyle{n \choose K} = {n \choose k_1,k_2,\cdots,k_m} = \dfrac{n!}{k_{1}!k_{2}!\cdots k_{m}!} $이며,  
이는 $\displaystyle{n\choose k_1} \displaystyle{n-k_1\choose k_2} \displaystyle{n-k_1-k_2\choose k_3}\cdots \displaystyle{n-k_1-k_2\cdots-k_{m-1}\choose k_m}$ 과 같기 때문에, 정리하면 

<p> $${\binom {n}{K}} = {\binom {n}{k_1,k_2,\cdots,k_m}}=\prod_{i=1}^{m}{\binom {k_{i}+k_{i+1}+\cdots +k_{m}}{k_{i}}}=\prod_{i=1}^{m}{\binom {k_{1}+k_{2}+\cdots +k_{i}}{k_{i}}}$$ </p>
가 된다.

<br/>

### gamma function
$n\in\mathbb{N}:\; n!=1\cdot 2\cdot 3\cdots n$ 에서 $n$ 범위의 일반화.  

$\left(\dfrac{9}{2}\right)!$ 은 무엇일까.  
자연수 범위를 벗어난 팩토리얼 값이 정의하기가 애매해지는 이유는  
자연수에 대해선 $1!=1$이라고 정의를 내리고 시작하는 것과는 달리,   
$\left(\dfrac{9}{2}\right)! = \left(\dfrac{9}{2}\right)\cdot \left(\dfrac{7}{2}\right)! = \cdots = \left(\dfrac{9}{2}\right)\cdot \left(\dfrac{7}{2}\right)!\cdots \left(\dfrac{1}{2}\right)!$  
로 재귀적으로 자연수가 아닌 팩토리얼의 값을 줄여나갈 때, $\left(\dfrac{1}{2}\right)!$ 과 같은 시작점을 찾아서 정의하기가 참 그렇기 때문이다.  
반대로 말하자면, 어떤 값 $z$에 대해서던 $z! = z\cdot (z-1)!$ 이라고 정의내리는 것은 크게 이상하지 않다. 


[지수 함수](/posts/mathematics/#지수-로그)의 실수 범위로 지수의 확장 session에서 다룬 바와 비슷하게,  
연산 범위를 확장시키기 위하여 기존의 연산 법칙 $n! = n\cdot (n-1)!$를 지정하여 확장된 정의역에 대해 그 연산을 만족하도록 하는 gamma function $\Gamma$ 를 정의해보자.  


1. 우선 팩토리얼의 종특인 $f(1)=1,\; f(x+1)=xf(x)$이라는 recurrence relation 을 만족하는 함수를 $\Gamma(x)$라고 정의하자.
2. $z\in\mathbb{C}:\; Re(z)>0$인 $z$을 정의역으로 두는  
   $\Gamma (z):=\displaystyle\int_{0}^{\infty }x^{z-1}e^{-x}\,dx$ 으로 두면 
3. <br/>  
   <p>$$ \begin{align*}
   \Gamma (z+1)&=\int_{0}^{\infty}x^{z}e^{-x}\,dx \\\\
               &=\left[-x^{z}e^{-x}\right]_{0}^{\infty }+\int _{0}^{\infty }zx^{z-1}e^{-x}\,dx \\\\
               &=\lim _{x\to \infty}(-x^{z}e^{-x})-(0e^{-0})+z\int _{0}^{\infty }x^{z-1}e^{-x}\,dx \\\\
               &=z\int _{0}^{\infty }x^{z-1}e^{-x}\,dx \\\\
               &=z\Gamma(z)
   \end{align*}$$ </p>
4. <br/>
   <p>$$ \begin{align*}
   \Gamma (1)&=\int_{0}^{\infty }x^{1-1}e^{-x}\,dx \\\\
             &=\left[-e^{-x}\right]_{0}^{\infty } \\\\
             &=\lim _{x\to \infty }(-e^{-x})-(-e^{-0}) \\\\
             &=0-(-1) \\&=1
   \end{align*}$$ </p>
5. 와와

$\Gamma(1)=1,\, \Gamma(2)=1\cdot \Gamma(1)=1,\, \Gamma(3)=2\cdot \Gamma(2)=2,\, \cdots$ 와 같이  
$n\in\mathbb{N}$일 때, $\Gamma(n)=(n-1)!$을 만족한다.


![Alt text](/pictures/mathematics/감마함수.png)  
$\Gamma (z)=\int _{0}^{\infty }x^{z-1}e^{-x}\,dx$ 는 복소수 $z$의 실수부가 $0$ 이상인 상황에서 정의되는데,  
이를 해석적인 함수의 정의역을 확장하는 [analytic continuation](https://en.wikipedia.org/wiki/Analytic_continuation)이라는 기법을 사용하여 non-positive integers 를 제외한 모든 복소수 영역으로 확장시킬 수 있다.  
Analytic 함수에 대한 설명은.. 나중에 언젠간..

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_순열조합" %}


### 확률
* `표본 공간`: 모든 outcome 집합, `사건`: 특정 outcome들의 집합 (표본 공간의 부분집합), `확률측도`: 각 사건을 실수값(확률)으로 매핑시키는 함수
* 확률의 정의: `수학적 확률` $\dfrac{n(A)}{n(S)}$, `통계적 확률` $\lim\limits_{N\to\infty} \dfrac{a}{N}=p$, `기하학적 확률`, `베이즈 확률`
* $P(A \cup B)=P(A)+P(B)-P(A \cap B),\; P(A \cap B)=P(A)\cdot P(B\|A)=P(B)\cdot P(A\|B)$
* `독립`: 사건 $A, B$가 $P(B\|A)=P(B\|A^C)=P(B)$를 만족 $\Leftrightarrow P(A\cup B)=P(A)\cdot P(B)$

{% capture context1 %}
### Probability Space $(S, F, P)$ 
* `시행` - 같은 조건 아래에서 반복 가능한, 가능한 모든 결과(outcome)의 집합을 알 수 있는 관찰, 실험
* `표본 공간(Sample space)` $S=\\{e_1, e_2, \cdots, e_n\\}$ - 가능한 모든 outcome 를 모아놓은 집합
* `사건(event)` - 임의의 outcome을 모아놓은 집합
* `사건 공간(Event space)` $F=\\{\varnothing, \\{e_1\\}, \\{e_2\\}, \\{e_1, e_2\\}, \cdots, \\{e_1, e_2, \cdots, e_n\\}\\}$ - 모든 사건의 집합($S$의 가능한 모든 부분집합들의 집합)
  * F의 원소 중 $\\{e_1\\}, \\{e_2\\}$와 같이 하나의 원소만으로 이루어진 사건을 `근원사건`이라고 함.
* `확률 측도` $P$ - $P:\, F \longrightarrow \mathbb{R}$, $F$의 원소(outcome을 모아놓은 집합)를 실수 확률값으로 매핑시키는 함수
 
확률이란, 어떤 event에 할당되는 $[0, 1]$ 사이의 실수값으로 정의되고, 이를 매핑시켜주는 함수가 확률 측도가 된다.
자세한 내용은 다음 단계 참조

<br/>

### 여러 정의, 정리들
사건 $A, B$에 대하여,
* 여사건: $P(A)+P(A^C)=1$
* `덧셈정리`: $P(A\cup B)=P(A)+P(B)-P(A\cap B)$
* `조건부 확률`: $P(B\|A)=\dfrac{P(A\cup B)}{P(A)}$
  * 표본 공간을 구성하는 outcome을 사건 $A$에 속하는 outcome으로 제한하였을 때$(S \leftarrow A)$, $B$의 확률
  * 즉, outcome이 A에 속한다는 사실을 이미 알고 있을 때 $B$의 확률
  * 혹은, 사건 $A$가 일어났다고 가정할 때 $B$가 일어날 확률 
* `곱셈정리`: $P(A \cap B)=P(A)\cdot P(B\|A)=P(B)\cdot P(A\|B)$
* `독립`: $P(B\|A)=P(B\|A^C)=P(B)$
  * 사건 $B$가 일어날 확률은 사건 $A$와 관계가 없다.
  * $P(A\cup B)=P(A)\cdot P(B)$

{% endcapture %}

{% capture context2 %}
### 확률의 정의
확률이란, 어떤 event에 할당되는 $[0, 1]$ 사이의 실수값으로 정의되고, 이를 매핑시켜주는 함수를 확률 측도라고 한다.  
추가적으로, 모든 근원사건에 할당된 확률을 모두 더하면 1이 되어야 하는 제한조건이 붙는다.  
* $P(S)=1, P(\varnothing)=0$
  
<br/>
  
이제 이걸 어떻게 매핑시켜줄 것이냐?  
몇가지 관점에 따른 정의가 있다.
1. 수학적 확률
    * 각각의 근원사건이 일어나는 것이 같은 정도로 확실할 때, 사건 $A$가 일어날 확률은 $\dfrac{A에\; 속하는\; 근원사건\; 수}{전체\; 근원사건\; 수} = \dfrac{n(A)}{n(S)}$ 로 정의
    * **각각의 근원사건이 일어나는 것이 같은 정도로 확실할 때** 라는 조건이 붙는데, 아무런 시행 없이 확실하다고 가정하는 것 자체가 어렵다.  
    * 즉 완전히 이상적인 확률.
2. 기하학적 확률
    * 수학적 확률과 비슷한데, 확률을 (사건 $A$가 일어날 수 있는 영역의 크기)/(모든 영역 크기 로 정의함)
3. 통계적 확률
    * 시행 횟수를 $N$, 사건 $A$가 일어난 횟수를 $a$라 뒀을 때, `상대도수`를 $\dfrac{a}{N}$으로 정의
    * 통계적 확률은 $\lim\limits_{N\to\infty} \dfrac{a}{N}=p$ 로 정의.
    * $N\to\infty$ 가 불가능하므로, 충분히 큰 $N$을 잡는 것으로 타협한다.
4. 베이즈 확률
    * $N\to\infty$ 가 안되서 통계적 확률을 믿을 수 없기 때문에 생김
    * degree of belief 을 도입해서, belief가 강하다면 상대도수 $\dfrac{a}{N}$가 어떤 값을 가지더라도  
      빼애애액 $N$이 충분히 안크잖아 내가 믿는 값이 맞음 애애애애앵앵  
      하지만 그래도 참고 정도는 해 주지 흥  
      ..을 시전할 수 있는 이론. 그게 꼭 나쁘다는건 아니지만.
        * 아주 간단히 요약하자면, 실제 실험 결과 1회와 본인이 믿는 대로 뇌내에서 실험한 결과 1회가 최종 결론에 미치는 영향이 같다. 
        * 이때 degree of belief 는 내뇌 실험 횟수 A를 뜻함.   
    * 가설(belief) $H$와 데이터 $D$에 대하여 뇌피셜 $P(H)$을 이미 가지고 있을 때, 실험 데이터가 주어진 이후의 `사후확률`은 베이즈 정리에 의하여  
      $P(H|D)={\dfrac{P(D|H)\;P(H)}{P(D)}}$가 된다.
    
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_확률" %}

### 확률분포
* `평균` $m=\dfrac{x_1+x_2+\cdots+x_n}{n}=\dfrac{1}{n}\sum\limits_{i=1}^{n} x_i$  
* `분산` $\sigma^2=\dfrac{(x_1-m)^2+(x_2-m)^2+\cdots+(x_n-m)^2}{n}=\dfrac{1}{n}\sum\limits_{i=1}^{n} (x_i-m)^2=\dfrac{1}{n}\sum\limits_{i=1}^{n} x_i^2 -m^2$
* `확률변수` $X$ : 어떤 event 를 어떤 실수값으로 매칭시키는 함수. $X:\, S \longrightarrow \mathbb{R}$
* `확률분포`: $X=x_i$를 가질 확률 $p_i$의 대응 관계. $P(X=x_i)=p_i$
  * 확률분포의 평균 $E(X)=\sum\limits_{i=1}^n {x_i p_i}$
  * 확률분포의 분산 $V(X)=\sum\limits_{i=1}^n {(x_i-m)^2 p_i}=\sum\limits_{i=1}^n {x_i^2 p_i} -m^2=E(X^2)-E(X)^2$
* `이항분포`: 각 시행의 결과가 서로 독립인 시행에서 $P(A)=p$인 사건 $A$가 $r$번 일어날 확률
  * $P(X=r)=_n\mathrm{C}_r p^r (1-p)^{n-r} \Rightarrow X\sim \mathrm{B}(n, p),\; E(X)=np,\, V(x)=np(1-p)$
* `정규분포` $X\sim \mathrm{N}(m, \sigma^2) = \dfrac{1}{\sqrt{2\pi}\sigma} e^{-\frac{(x-m)^2}{2\sigma^2}}$
  * `정규확률변수` $Z=\dfrac{X-m}{\sigma}\sim \mathrm{N}(0, 1^2)$
  * $X\sim B(n, p), \text{ if } np > 5 \text{ and } n(1-p) > 5 \Rightarrow X\sim \mathrm{N}(np, np(1-p))$

{% capture context1 %}

### 확률변수, 확률분포
이전까지 확률 $P(A)$는 어떤 event $A$의 집합을 정의역이 되도록 정의하였는데,   
event 라는 개념을 정의역으로 두기엔 너무 variation이 크고 다루기 어렵기 때문에, 이를 좀 깔끔하게 정리하고자 만든 것이 확률변수라고 생각하면 된다.
  
![Alt text](/pictures/mathematics/확률변수.jpg)  
`확률변수`란, 표본 공간의 원소인 근원사건을 자신이 원하는 임의의 실수값으로 매칭하는 함수이다.  
예를 들면, 주사위를 2번 던져서 눈의 합이 3인 event가 $A=\\{(1, 2), (2, 1)\\}$이라면  
확률변수 $X$를 두 주사위의 눈의 합으로 정의하여, $P(A)=P(X=3)$이 되도록 한다.

이름은 확률변수지만, 확률도 아니고(함수다) 랜덤하지도 않다고 한다.

<br/>

`확률분포`(Probability distribution function, PDF)는 확률변수와 확률의 대응 관계를 나타내는 함수이다.  
* $ P(X=x)=p : \mathbb{R} \longrightarrow [0, 1] (\subset \mathbb{R}) $

  
$X$는 이산형 변수일 수도 있고, 연속일 수도 있으며, 확률분포 역시 이를 따라 `이산확률분포`와 `연속확률분포`로 나뉜다. 

<br/>

### 이항분포
서로 독립인 시행(`독립시행`)을 여러번 반복했을 때, 각 시행이 사건 $A$ 혹은 $A^C$에 속한다고 하면$(P(A)=p)$  
각 시행의 outcome을 $a_i$(: 시행 $i$가 사건 $A$에 포함), $b_i$(: 아님) 이라 두자.  
그럼 $S=\\{(a_1, a_2, \cdots a_n), (b_1, a_2, \cdots a_n), (a_1, b_2, \cdots a_n), \cdots, (b_1, b_2, \cdots b_n)\\}$ 이 되며  
사건 $A$가 $r$회 일어나는 최종 outcome $R=\underset{n(a)=r}{\underbrace{(a_1, b_2, \cdots, b_n)}}$를 $r$로 매핑하는 확률변수 $X$를 정의하면, $X$의 확률분포는 
<p> $$\mathrm{P}(X=r)=\,_n\mathrm{C}_r p^r (1-p)^{n-r}$$ </p>
가 된다.

<br/>

### 정규분포
![Alt text](/pictures/mathematics/정규분포.png)  
$X\sim \mathrm{N}(m, \sigma^2) = \dfrac{1}{\sqrt{2\pi}\sigma} e^{-\frac{(x-m)^2}{2\sigma^2}}$  
정규분포 관련해선 해야될 얘기가 많긴한데 통계 파트에서 나중에 할 예정

{% endcapture %}

{% capture context2 %}
### 이항분포 평균, 분산 계산
$\mathrm{P}(X=r)=\,_n\mathrm{C}_r p^r q^{n-r} (q=1-p)$
* 평균 $m=np$
  * $(q+pt)^n =\sum\limits_{r=0}^n { \displaystyle{n\choose r} p^r t^r q^{n-r}}$
  * $t$에 대하여 미분하면, $np(q+pt)^{n-1} = \sum\limits_{r=0}^n {r\displaystyle{n \choose r}p^r t^{r-1} q^{n-r}}$
  * $t=1 \Rightarrow np=\sum\limits_{r=0}^n {r\displaystyle{n \choose r}p^r q^{n-r}}$
  * $m=\sum\limits_{r=0}^{n} r\mathrm{P}(X=r)=\sum\limits_{r=1}^{n} r_n\mathrm{C}_r p^r q^{n-r}=np$

<br/> 
  
* 분산 $V(X)=npq$
  * $V(X)=\sum\limits_{r=0}^{n} r^2 \mathrm{P}(X=r)-m^2$
  * 평균에서 2번째 식을 한번 더 미분하면, $n(n-1)p^2(q+pt)^{n-2} = \sum\limits_{r=0}^n {r(r-1)\displaystyle{n \choose r}p^r t^{r-2} q^{n-r}}$
  * $t=1 \Rightarrow n(n-1)p^2=\sum\limits_{r=0}^n {r(r-1)\displaystyle{n \choose r}p^r q^{n-r}}=\sum\limits_{r=0}^n r(r-1)\mathrm{P}(X=r)$
  * $\therefore \sum\limits_{r=0}^n r^2 \mathrm{P}(X=r) = n(n-1)p^2+np=np(np-p+1)$
  * $V(X)=np(np-p+1)-(np)^2 = np(1-p)=npq$

<br/>

### 확률변수의 정의
확률변수 $X:\,\Omega\longrightarrow E$ 로 정의가 보통 되는데, 여기서 $\Omega$는 위에서 말한 Sample space $S$이고 $E$는 measurable space 이다.  
Measurable space가 무엇인지에 대해선 좀 찾아봤는데 너무 어려운 관계로 링크만 남긴다.
[위키](https://en.wikipedia.org/wiki/Measurable_space), [Quora](https://www.quora.com/What-is-a-measurable-space), [Encyclopedia](https://www.encyclopediaofmath.org/index.php/Measurable_space)  
간단히 설명하자면, 어떠한 집합에 길이와 같은 성질처럼 measure를 assign할 수 있는 공간이라고 해야되나? 잘 모르겠다.  
아무튼 보통 $E=\mathbb{R}$이다. 


확률 변수 이전까지 확률 측도 $P:A(event) \longrightarrow \mathbb{R}$ 로 표기했었는데,  
확률 변수가 도입되고 갑자기 $P(X=1)=0.1$ 처럼 $P:X(A)=E$(보통 $\mathbb{R}$) $\longrightarrow \mathbb{R}$ 처럼 정의역이 확률변수의 output으로 바뀐다.  
뭐가 맞는 것일까.

<br/>

일단 $P:\text{event} A \longrightarrow \mathbb{R}$가 맞다.  
그리고 확률변수가 들어간 표기는 사실 다음과 같음.
$S \subset E,\; P(X\in S) = P(\\{\omega\in\Omega \| X(\omega)\in S \\})$  
즉, $P$의 정의역은 $X(\omega)\in S$를 만족하는 $\omega$ 들의 집합이며, $\omega$ 는 근원사건들이다. 고로 정의역은 Sample space.  
다만 표기를 간단히 하기 위해서, $\omega$를 생략하여 $P(X\in S)$ 로 표기하는 것. 

예를 들면, $X$를 (주사위 2번 던진 결과) $\longrightarrow$ (주사위 눈금 합) 으로 정의하고, $S=\\{2, 3\\}$으로 두면  
$P(\\{\omega\in\Omega \| X(\omega)\in \\{2, 3\\} \\}) = P(\\{(1, 1), (1, 2), (2, 1)\\})$ 가 원래 표기인데  
$P(X=\\{2, 3\\})$ 으로 간략하게 표기하는 것

<br/>

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_확률분포" %}

### 통계적 추정
* 조사 대상 전체인 `모집단`의 자료 일부를 추출한 것을 `표본`이라 함
* 모집단의 확률분포가 모평균이 $m$, 모분산이 $\sigma^2$ 일 때, 크기가 $n$인 임의표본을 추출하는 경우
  * 복원추출: $E(\bar{X})=m, V(\bar{X})=\dfrac{\sigma^2}{n}$
  * 비복원추출: $E(\bar{X})=m, V(\bar{X}) = \dfrac{\sigma^2}{n}\cdot \dfrac{N-n}{N-1}$
  * 표본평균의 분포: $\bar{X} \sim \mathrm{N}\left(m, \dfrac{\sigma^2}{n}\right)\; (n >\,> 1)$
* 모집단의 확률분포가 $\mathrm{N}(m, \sigma)$이고 $m$을 모를 때, 크기가 $n$인 임의표본을 추출하여 모평균 $m$을 추정할 수 있다
  * 95% `신뢰도`로서, $\bar{X}-1.96\cdot \dfrac{\sigma}{\sqrt{n}} \leq m \leq \bar{X}+1.96\cdot \dfrac{\sigma}{\sqrt{n}}$
* `표본비율` $\hat{p}=\dfrac{X}{n}$에 대하여, $E(\hat{p})=p,\, V(\hat{p})=\dfrac{pq}{n},\, \hat{p}\sim \mathrm{N}(p, \dfrac{pq}{n})$

{% capture context1 %}
### 표본평균
모집단에서의 평균 $m$은 그냥 $m=\dfrac{1}{n}\sum\limits_{i=1}^{n} x_i$ 인 숫자이다.  
하지만 표본에서의 평균은 선택되는 표본에 따라 값이 달라지므로,   
Sample space를 크기가 $n$인 모든 표본의 조합으로 두면, 그 값을 나타내는 확률변수 $\bar{X}$에 대한 확률분포가 존재한다.  
`표본평균` $\bar{X}$의 기대값은 모평균 $m$과 같지만, 그 분산은 크기에 반비례하고, $\bar{X} \sim \mathrm{N}\left(m, \dfrac{\sigma^2}{n}\right)$를 따른다.

주의할 것은, $V(\bar{X})$는 Sample space를 크기가 $n$인 모든 표본의 조합으로 두었을 때 표본평균의 분산값이지, 임의의 표본 자체의 분산은 아니다.  
마찬가지로 $\bar{X} \sim \mathrm{N}\left(m, \dfrac{\sigma^2}{n}\right)$도 표본 자체의 분포가 아니다.

<br/>

### 모평균의 추정
$\bar{X} \sim \mathrm{N}\left(m, \dfrac{\sigma^2}{n}\right)$이므로, $Z=\dfrac{\bar{X}-m}{\frac{\sigma}{\sqrt{n}}} \sim \mathrm{N}(0, 1^2)$  
$\mathrm{P}(-1.96\leq Z\leq 1.96)=0.95$이므로, $\mathrm{P}\left(-1.96\leq \dfrac{\bar{X}-m}{\sigma/ \sqrt{n}}\leq 1.96\right)=0.95$  
정리하면, $\mathrm{P}\left(\bar{X}-1.96\cdot\dfrac{\sigma}{\sqrt{n}} \leq m \leq \bar{X}+1.96\cdot\dfrac{\sigma}{\sqrt{n}}\right)=0.95$  
즉, 구간 $\left[\bar{X}-1.96\cdot\dfrac{\sigma}{\sqrt{n}}, \bar{X}+1.96\cdot\dfrac{\sigma}{\sqrt{n}} \right]$ 안에 $m$이 들어갈 확률은 95%이다.

신뢰도가 $a$일 때, $P(-\alpha\leq Z \leq \alpha)=a$인 $\alpha$가 $\dfrac{\sigma}{\sqrt{n}}$ 앞의 계수가 됨.

<br/>

### 표본비율
모비율이 $p$인 사건이 있을 때, 표본의 크기가 $n$이면 추출된 횟수를 나타내는 확률변수 $X\sim \mathrm{B}(n, p)$이다.  
표본 전체의 비율을 나타내는 확률변수인 표본비율 $\hat{p}=\dfrac{X}{n}$을 정의하면,
* $E(\hat{p})=E\left(\dfrac{X}{n}\right)=\dfrac{1}{n}E(X)=\dfrac{np}{n}=p$
* $V(\hat{p})=V\left(\dfrac{X}{n}\right)=\dfrac{1}{n^2}V(X)=\dfrac{npq}{n^2}=\dfrac{pq}{n}$

마찬가지로, $n$이 커지면 정규분포를 따른다. $\hat{p}\sim \mathrm{N}(p, \dfrac{pq}{n})$

표본비율에 대해서도, 모비율의 추정을 다음과 같이 할 수 있다.  
모비율 $p$의 95% 신뢰구간: $\left[\hat{p}-1.96\sqrt{\dfrac{\hat{p}\hat{q}}{n}}, \hat{p}+1.96\sqrt{\dfrac{\hat{p}\hat{q}}{n}} \right]$

{% endcapture %}

{% capture context2 %}
### 복원추출의 표본분산
* $\mu=\bar{X}=\dfrac{1}{n}\sum\limits_{i=1}^n x_i$  
* $V(\bar{X}) = E((\bar{X}-m)^2)= E\left[\left(\dfrac{1}{n}\sum\limits_{i=1}^n x_i -\mu\right)^2\right]=\dfrac{1}{n^2} E\left[\left(\sum\limits_{i=1}^n (x_i -\mu)\right)^2\right]$
* 전개하면, $V(\bar{X}) =\dfrac{1}{n^2}E[(x_1-\mu)^2+\cdots+(x_n-\mu)^2+(x_1-\mu)(x_2-\mu)+(x_1-\mu)(x_3-\mu)+\cdots]$
* 각 표본은 서로 독립이므로, $E[(x_i-\mu)(x_j-\mu)]=E[x_i-\mu]E[x_j-\mu]=0, E[(x_i-\mu)^2]=\sigma^2$
* $\therefore V(\bar{X}) =\dfrac{1}{n^2}\cdot n\sigma^2 = \dfrac{\sigma^2}{n}$

<br/>

### 표본평균과 표본비율의 분산
표본평균의 분산은 $\dfrac{\sigma^2}{n}$, 즉 모분산 나누기 $n$이다.  
그렇다면 표본비율의 분산도 모분산 나누기 $n$으로 해서, $npq / n = pq$가 되어야 하지 않는가.

<br/>

어.. 일단은 모분산이 $npq$가 아니다. $npq$는 확률이 $p$인 표본을 $n$번 뽑았을 때 분산이지 모분산이 아님  
전체 $N$개 크기의 모집단에서, 확률변수 $Y=1$인 놈의 비율이 $p$, $Y=0$의 비율이 $1-p$라고 생각해보자.  
$E[Y]=p$일 것이고, $Y^2=Y$ 이므로 $V(Y)=E[Y^2]-E[Y]^2=p(1-p)$이다.  
그러니까 모분산이 $p(1-p)$이므로, 표본비율의 분산은 $\dfrac{pq}{n}$이 맞다. 끗

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="적통_통계적_추정" %}

## 기하와 벡터

### 이차곡선
![Alt text](/pictures/mathematics/원뿔곡선.gif)  
#### 포물선
* 정의 : 평면 위에서의 한 정점(`초점`)과 정적선(`준선`)에 이르는 `거리가 같은 점`의 자취
* 방정식 : 초점이 $(p, 0)$, 준선이 $x=-p$일 때, $y^2=4px$


#### 타원
* 정의 : 두 정점(`초점`)으로부터 `거리 합이 일정한 점`의 자취
* 방정식 : $F(k, 0),\, F'(-k, 0)$, 거리 합 $2a$일 때 $\dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} = 1\; (k^2=a^2-b^2)$


#### 쌍곡선
* 정의 : 두 정점(`초점`)으로부터 `거리 차가 일정한 점`의 자취
* 방정식 : $F(k, 0),\, F'(-k, 0)$, 거리 차 $2a$일 때 $\dfrac{x^2}{a^2} - \dfrac{y^2}{b^2} = 1\; (k^2=a^2+b^2)$
* 점근선 : $\dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} = 0, \; y=\pm \dfrac{b}{a}x$


#### 이심률
![Alt text](/pictures/mathematics/이심률.png)  
이차곡선의 일반화. 정적선 $l$과 정점 $F$간의 거리 비인 `이심률` $\epsilon=\dfrac{\overline{PF}}{\overline{PD}}$의 값으로 모든 이차곡선이 정의된다.

{% capture context1 %}
### 포물선
![Alt text](/pictures/mathematics/포물선.png)  
* 평면 위에서 초점과 준선에 이르는 거리가 같은 점의 자취
* $F$를 `초점`, $l$을 `준선`, `초점`을 지나고 `준선`에 수직인 직선을 `축`, 축과 포물선의 교점을 `꼭짓점`이라고 한다.
* 초점이 $(p, 0)$, 준선이 $x=-p$일 때, 포물선의 방정식은 $y^2=4px$
  * $\|x+p\| = \sqrt{(x-p)^2+y^2}$ 양변을 제곱
  * 평행이동에 의하여 $(y-n)^2 = 4p(x-m)$, 축은 $x$축과 평행
  * 일반형 $y^2+2gx+2fy+c=0\; (g\neq 0)$ 
* 초점이 $(0, p)$, 준선이 $y=-p$일 때, 포물선의 방정식은 $x^2=4py$
  * 평행이동에 의하여, $(x-m)^2 = 4p(y-n)$, 축은 $y$축과 평행
  * 일반형 $x^2+2gx+2fy+c=0\; (f\neq 0)$
* 접선의 방정식은
  * $y^2=4px$ 위의 점 $(x_1, y_1)$에서 접선은 $y_1y=2p(x+x_1)$
  * 기울기가 $m$인 접선은 $y=mx+\dfrac{p}{m}$
  * 이지만 어차피 미분해서 구할수 있잖아

<br/>

### 타원
![Alt text](/pictures/mathematics/타원.gif) ![Alt text](/pictures/mathematics/타원2.png)
* 두 초점으로부터 거리 합이 일정한 점의 자취 
* $F$, $F'$를 두 `초점`, 두 `초점`을 지나는 $\overline{AB}$를 `장축`, $\overline{CD}$를 `단축`, 두 축의 교점을 `타원의 중심`이라고 하고, $A,B,C,D$를 `꼭짓점`이라 한다.
* 초점이 $F(k, 0), F'(-k, 0)$, 거리 합 $2a$일 때 타원의 방정식은 $\dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} = 1\; (k^2=a^2-b^2)$
  * $\sqrt{(x-k)^2+y^2} + \sqrt{(x+k)^2+y^2}=2a$ 에서 제곱하여 잘 정리
  * 평행이동에 의하여 $\dfrac{(x-m)^2}{a^2} + \dfrac{(y-n)^2}{b^2} = 1$, `장축`은 $x$축과 평행
  * 일반형 $Ax^2+By^2+Fx+Gy+C=0 (AB>0, A<B)$
* 초점이 $F(0, k), F'(0, -k)$, 거리 합 $2b$일 때 타원의 방정식은 $\dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} = 1\; (k^2=b^2-a^2)$
  * 일반형 $Ax^2+By^2+Fx+Gy+C=0\; (AB>0, A>B)$
* 접선의 방정식은
  * $\dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} = 1$ 위의 점 $(x_1, y_1)$에서 접선은 $\dfrac{x_1x}{a^2} + \dfrac{y_1y}{b^2} = 1$
  * 기울기가 $m$인 접선은 $y=mx\pm \sqrt{a^2m^2+b^2}$
* 타원의 넓이는 $\pi ab$
  
<br/>
  
### 쌍곡선
![Alt text](/pictures/mathematics/쌍곡선.JPG)
* 두 초점으로부터 거리 차가 일정한 점의 자취
* $F, F'$를 두 `초점`, 쌍곡선과 $\overline{FF'}$의 교점을 $A, A'$, $\overline{AA'}$을 `주축`, $\overline{AA'}$의 중점 O를 `쌍곡선의 중심`이라 한다.
* 초점이 $F(k, 0), F'(-k, 0)$, 거리 차 $2a$일 때 쌍곡선의 방정식은 $\dfrac{x^2}{a^2} - \dfrac{y^2}{b^2} = 1\; (k^2=a^2+b^2)$
  * $\sqrt{(x+k)^2+y^2} - \sqrt{(x-k)^2+y^2}=2a$ 에서 제곱하여 잘 정리
  * 평행이동에 의하여 $\dfrac{(x-m)^2}{a^2} - \dfrac{(y-n)^2}{b^2} = 1$, 주축은 $x$축과 평행
  * 일반형 $Ax^2+By^2+Fx+Gy+C=0 (AB<0)$
* 점근선은 $\dfrac{x^2}{a^2} - \dfrac{y^2}{b^2} = 0$
  * 쌍곡선의 방정식을 $y$에 관하여 풀면 $y=\pm\dfrac{b}{a}x\sqrt{1-\left(\dfrac{a}{b}\right)^2},\; x\to\infty$ 일 때 $y\to\pm\dfrac b a x$
  * 변형하면 $\dfrac x a \mp \dfrac y b = 0,\; \left(\dfrac x a - \dfrac y b\right) \left(\dfrac x a + \dfrac y b\right)=\dfrac{x^2}{a^2} - \dfrac{y^2}{b^2}=0$
* 초점이 $F(0, k), F'(0, -k)$, 거리 차 $2b$일 때 쌍곡선의 방정식은 $\dfrac{x^2}{a^2} - \dfrac{y^2}{b^2} = -1\; (k^2=a^2+b^2)$
  * 평행이동에 의하여 $\dfrac{(x-m)^2}{a^2} - \dfrac{(y-n)^2}{b^2} = -1$, 주축은 $y$축과 평행
  * 일반형 $Ax^2+By^2+Fx+Gy+C=0\; (AB<0)$
* 접선의 방정식은
  * $\dfrac{x^2}{a^2} - \dfrac{y^2}{b^2} = 1$ 위의 점 $(x_1, y_1)$에서 접선은 $\dfrac{x_1x}{a^2} - \dfrac{y_1y}{b^2} = 1$
  * 기울기가 $m$인 접선은 $y=mx\pm \sqrt{a^2m^2-b^2}$

<br/>

### 원추곡선
: 대수적으로 표현한 이차곡선을 기하적인 명칭으로 변형  
![Alt text](/pictures/mathematics/원뿔곡선2.gif) ![Alt text](/pictures/mathematics/원뿔곡선3.png){: width="40%" height="40%"}    
원뿔을 평면으로 잘랐을 때 생기는 곡선. 

* $\alpha = \angle(A, L)$을 원뿔의 반 꼭지각이라 둔다  
* 원뿔의 축 $A$와, 절단하는 평면 $H$ 사이의 각 $\beta=\angle(A, H)$을 정의할 때, 원추곡선 $C$는
  * $\beta = 0 \Rightarrow C$는 `원`$(\epsilon < 1)$
  * $\alpha < \beta \Rightarrow C$는 `타원`$(\epsilon < 1)$
  * $\alpha = \beta \Rightarrow C$는 `포물선`$(\epsilon = 1)$
  * $\alpha > \beta \Rightarrow C$는 `쌍곡선`$(\epsilon > 1)$

을 만족한다.  
증명은 `당들렝의 구`를 통하여 한다. 다음 단계 참조

<br/>

### 이심률
원추곡선(이차곡선)의 특성을 나타내는 값으로, 아래 종특이 있다.
1. 점 $P$가 있을 때, 한 정적선 $l$에 내린 수선의 발 $D$와 한 정점 $F$에서 $\dfrac{\overline{PF}}{\overline{PD}} = \epsilon$
1. 두 원추곡선의 이심률이 같다 $\Leftrightarrow$ 두 원추곡선이 서로 닮는다
2. 원추곡선(이차곡선)이 원에서 벗어나는 정도를 나타냄
    * `원`: 0, `타원`: (0, 1), `포물선`: 1, `쌍곡선`: (1, $\infty$), `직선`: $\infty$
3. 원뿔에서, $\epsilon=\dfrac{\sin\beta}{\sin\alpha}$  
  ![Alt text](/pictures/mathematics/이심률2.png)    
4. 이차곡선을 $Ax^2+Bxy+Cy^2+Dx+Ey+F=0$으로 일반화하였을 때, `이심률`은 다음과 같다.
    * $\epsilon=\sqrt{\dfrac{2\sqrt{(A-C)^2 + B^2}}{\eta (A+C) + \sqrt{(A-C)^2 + B^2}}}$
    * $\eta = \text{sign}\left(-det\left(\begin{bmatrix}A & B/2 & D/2\\\\B/2 & C & E/2\\\\D/2&E/2&F\end{bmatrix}\right)\right)$  
    * ㅎㄷㄷ
    
1.번이 3.번이 됨을 보이자면, 정적선 $l: x=-p,\; F(p, 0)$로 두면  
$\overline{PF} = \sqrt{(x-p)^2+y^2},\; \overline{PD} = x+p$이므로  
$\overline{PF}^2 = (x-p)^2+y^2 = \epsilon^2 \overline{PD}^2 = \epsilon^2(x+p)^2$  
$(1-\epsilon^2)x^2+y^2+Dx+F=0$ 꼴이 되기 때문에 각 케이스별로 이차곡선의 일반항 조건을 생각해보면 증명된다.

축이 $x, y$축과 평행하지 않은, 임의의 회전변환을 거친 임의의 이차곡선의 일반항 $Ax^2+Bxy+Cy^2+Dx+Ey+F=0$이 어떤 곡선인지의 판별을
5.번의 이심률 공식을 통해 계산하여 구할 수 있다... 있는데 별로 그러고싶진 않다

{% endcapture %}

{% capture context2 %}
### 이차곡선 일반화
위에서 말했듯이, 이차곡선의 일반항에서 `이심률`을 구함으로서 이차곡선의 분류뿐만 아니라 형태까지 구할 수 있다(이심률이 같으면 닮은꼴이므로)  
하지만 솔직히 저걸 이해하긴 좀 힘들고, 다른 방식으로 접근해 보자.

* $Ax^2+Bxy+Cy^2+Dx+Ey+F=0$에서, $A=B=C=0$인 경우 식은 일차식이 되며 직선의 방정식이 된다. 와의미없당  
* $B=0$인 경우, 이차곡선의 축은 $x$ 혹은 $y$축과 평행하며 식을 정리하면 간단하게 판별할 수 있다. 
  * $AC > 0$ 이면 `타원(원)`, $AC=0$이면 `포물선`, $AC < 0$ 이면 `쌍곡선`이다.
* $B\neq 0$인 경우.. 회전변환이 들어간 상태이며 3가지 방법이 있다.
 
<br/>

1. 멍청한 방법: 곡선을 $\theta$ 만큼 `회전변환`시킨다. [참조](https://wiki.mathnt.net/index.php?title=%EC%9D%B4%EC%B0%A8%EA%B3%A1%EC%84%A0%EA%B3%BC_%ED%9A%8C%EC%A0%84%EB%B3%80%ED%99%98)
    * $x \to X\cos(\theta)−Y\sin(\theta),\; y\to X\sin(\theta)+Y\cos(\theta)$을 대입하여 $A'X^2+B'XY+C'Y^2+D'X+E'Y+F'=0$을 얻는다
    * $B'=−a\sin(2\theta)+b\cos(2\theta)+c\sin(2\theta)$ 가 되는데, $\cot(2\theta)=\dfrac{a−c}{b}$가 되도록 $\theta$를 바꿔서 $B'$을 조진다.
    * $A'X^2+C'Y^2+D'X+E'Y+F'=0$ 이 되어 쉽게 형태를 구할 수 있다. 해-피
    
2. 어려운 방법: `선형대수`를 이용한 일반화를 통한 판별식 도출. [참조](http://goodmath.tumblr.com/post/76467577056/%EC%9B%90%EB%BF%94%EA%B3%A1%EC%84%A0%EC%9D%98-%ED%8C%90%EB%B3%84%EC%8B%9D-discriminant-of-a-conic-section)
    * [주축정리](https://en.wikipedia.org/wiki/Principal_axis_theorem)의 증명과 비슷한 과정을 거친다.
    * $x:=\begin{bmatrix}x \\\\ y\end{bmatrix},\; Q:=\begin{bmatrix}A & \dfrac B 2\\\\ \dfrac B 2 & C\end{bmatrix},\; K:=\begin{bmatrix} D & E\end{bmatrix}$ 
      로 두면 $S(x,y)=x^TQx+Kx+F=0$ 으로 표현할 수 있다.
    * $Q$를 직교대각화하는 행렬 $P$를 구한다. 
      * 즉, $Qx = \lambda x$를 만족하는 `고윳값` $\lambda_1, \lambda_2$를 구하고, 각각의 `단위고유벡터`를 구하여 합쳐 $P$를 만든다.
      * 이때 $P^T Q P=\begin{bmatrix} \lambda_1 & 0 \\\\ 0 & \lambda_2 \end{bmatrix}$ 가 성립한다.  
    * $det(P) = 1$이므로, 선형변환 $P$는 `회전변환`이 된다. $x=Px'$
    * $x=Px'$를 원래 식에 대입하면, $x'^T (P^TQP) x' + (KP)x' + F = 0$,
      즉 $S(x', y')=\lambda_1 x'^2 + \lambda_2 y'^2+ D'x'+E'y'+F=0$ 인 
      혼합항의 계수 $B'=0$인 식을 구할 수 있다.
    * $B'=0$이므로, $\lambda_1 \lambda_2$ 의 부호에 따라 이차곡선의 형태를 결정할 수 있으며, $\lambda_1 \lambda_2$는 $AC-(B/2)^2$와 같다!
      * $det(Q−\lambda I)=0$ 조건으로부터, $\lambda−(A+C)\lambda+\dfrac{4AC−B^2}{4}=0$ 이며 근과 계수의 관계에 따라 둘이 같음. 

3. 얍삽한 방법: 2번의 결실을 날먹한다.
    * $B^2−4AC < 0 \Rightarrow$ `타원`
    * $B^2−4AC = 0 \Rightarrow$ `포물선`
    * $B^2−4AC > 0 \Rightarrow$ `쌍곡선`
    * 해----피    


추가로, 2.번 증명을 통해 $y=\dfrac 1 x$와 같은 유리식은 쌍곡선의 한 형태임이 증명된다.

<br/>

### 당들렝의 구
![Alt text](/pictures/mathematics/당들렝.gif)  
이차곡선의 기하학적 표현인 원추곡선을 증명하기 위해서 당들렝이 원뿔에 구를 넣어서 노오력한 결과  
자세한 증명은 여기를 보십시오 - [http://mathseodang.com/220696726122](http://mathseodang.com/220696726122)  
기타 모든 그림이나 gif들도 위 블로그에서 따왔습니다.

<br/>

#### 포물선
![Alt text](/pictures/mathematics/당들렝_포물선1.gif) ![Alt text](/pictures/mathematics/당들렝_포물선2.gif)  
$\overline{PF}=\overline{PR}$(구면 접선의 길이)$=\overline{QT}$(원뿔대 모선의 길이)$=\overline{MX}(\alpha=\beta)=\overline{PH}$

<br/>

#### 타원
![Alt text](/pictures/mathematics/당들렝_타원1.gif) ![Alt text](/pictures/mathematics/당들렝_타원2.jpg)  
$\overline{PF}=\overline{PR}, \overline{PF'}=\overline{PR'},\, \therefore \overline{PF}+\overline{PF'}=\overline{RR'}$ : 원뿔대의 길이로 항상 일정  
$\overline{PF}=\overline{PR}=\overline{QT},\; \overline{MX}=\overline{PH},\; \overline{TL}=\overline{XK}$,  
$\sin\alpha=\dfrac{\overline{TL}}{\overline{QT}}=\dfrac{\overline{TL}}{\overline{PF}},\; \sin\beta=\dfrac{\overline{XK}}{\overline{MX}}=\dfrac{\overline{XK}}{\overline{PH}}$  
$\therefore \epsilon=\dfrac{\overline{PF}}{\overline{PH}} = \dfrac{\sin\beta}{\sin\alpha}$ 

<br/>

#### 쌍곡선
![Alt text](/pictures/mathematics/당들렝_쌍곡선1.gif){: width="60%" height="60%"} ![Alt text](/pictures/mathematics/당들렝_쌍곡선2.jpg){: width="60%" height="60%"}  
$\overline{PF}=\overline{PR},\; \overline{PF'}=\overline{PR'},\; \therefore \overline{PF}-\overline{PF'}=\overline{RR'}$ : 원뿔대의 길이로 항상 일정  
타원과 같은 방법으로 (+ $\overline{QL}=\overline{MK}$),
$\sin\alpha=\dfrac{\overline{QL}}{\overline{QT}}=\dfrac{\overline{QL}}{\overline{PF}},\; \sin\beta=\dfrac{\overline{MK}}{\overline{MX}}=\dfrac{\overline{MK}}{\overline{PH}},\; \epsilon=\dfrac{\overline{PF}}{\overline{PH}} = \dfrac{\sin\beta}{\sin\alpha}$ 

<br/>

### 극좌표계와 이심률
같은 블로그 [참조](http://mathseodang.com/220621141953)  

위에서 언급했듯이 준선의 방정식 $x=-p$, 초점을 $(p, 0)$으로 두고 정리하면, $x^2+y^2=\epsilon^2(x+p)^2$가 된다.  
극좌표계로 변환하면($r=\sqrt{x^2+y^2},\, x=r\cos\theta$), $r^2=\epsilon^2(r\cos\theta+p)^2,\; r=\dfrac{pe}{1-\epsilon\cos\theta}=\dfrac{l}{1-\epsilon\cos\theta}$ 가 된다($l=p\epsilon$).  
반대로 준선을 $x=p$, 초점을 $(-p, 0)$으로 두면, $r=\dfrac{p\epsilon}{1+\epsilon\cos\theta}=\dfrac{l}{1+\epsilon\cos\theta}$가 된다.

정리하면, $r=\dfrac{p\epsilon}{1\pm \epsilon\cos\theta}=\dfrac{l}{1\pm \epsilon\cos\theta}$이며,  
타원의 경우 장축의 길이 $2a=\dfrac{p\epsilon}{1-\epsilon}+\dfrac{p\epsilon}{1+\epsilon}=\dfrac{2p\epsilon}{1-\epsilon^2}$에서 $p\epsilon=l=a(1-\epsilon^2)$가 되어 $r=\dfrac{a(1-\epsilon^2)}{1\pm \epsilon\cos\theta}$가 된다.  
$\epsilon\to 0$일 때, $p\to \infty$ 이며, $r=a$가 된다.
  * $x^2+y^2=\epsilon^2(x+p)^2$ 에서 $\epsilon\to 0$이면 반지름이 항상 0이 되지 않나 싶은데 $p\to\infty$ 로 발산하면서 장축 $2a$는 유지된다.

<br/>

### 잡소리
* 포물선의 축과 평행하게 들어온 빛은 포물선에서 반사되어 모두 초점으로 모인다.  
  ![Alt text](/pictures/mathematics/포물선.png)  
  * 반대로, 초점에서 나간 빛은 포물선에서 반사되어 모두 축과 평행하게 나간다.
  * 반사망원경이나 안테나(전파가 겁나 먼 곳에서 들어오므로 다 평행하게 들어옴), 손전등(초점에서 빛을 보냄) 등에 우려먹는다.
* [기타 성질들](https://m.blog.naver.com/yh6613/220881307005)
  
* 타원의 매개변수 방정식은 $x=a\cos t,\, y=b\sin t,\, 0\leq t < 2\pi$ 이다.
* 한 초점에서 출발한 빛이 타원에 반사되면 [페르마의 최소 시간 원리](https://ko.wikipedia.org/wiki/%ED%8E%98%EB%A5%B4%EB%A7%88%EC%9D%98_%EC%9B%90%EB%A6%AC)에 의하여 다른 초점을 지나게 된다.
  * 반대로 타원의 외부에서 초점을 향해 진행하는 빛이 타원의 점에 의해 반사되면, 그 점과 다른 초점을 연결한 직선에 따라 반사됨.  


* 쌍곡선에서 각 점근선에 내린 수선의 발의 길이 곱은 일정함.
* 초점이 일치하는 쌍곡선과 타원의 교점에서 각각 접선은 수직함

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="기벡_이차곡선" %}

### 일차변환
* $f:(x, y) \longrightarrow (x', y'),\; \begin{cases} x'=ax+by \\\\ y'=cx+dy \end{cases} \Leftrightarrow 
  \begin{pmatrix} x' \\\\ y' \end{pmatrix} = \begin{pmatrix} a & b \\\\ c & d \end{pmatrix} \begin{pmatrix} x \\\\ y \end{pmatrix}$
  * 일차변환 $f$의 행렬 $A=\begin{pmatrix} a & b \\\\ c & d \end{pmatrix}$
* `닮음변환` $\begin{pmatrix} k & 0 \\\\ 0 & k \end{pmatrix}$, `회전변환` $\begin{pmatrix} \cos\theta & -\sin\theta \\\\ \sin\theta & \cos\theta \end{pmatrix}$
* 일차변환의 합성: $f \leftrightarrow A, g \leftrightarrow B \Rightarrow g \circ f \leftrightarrow BA$
* 일차변환의 역변환: $f \leftrightarrow A \Rightarrow f^{-1} \leftrightarrow A^{-1}$
* $A^{-1}$이 존재할 때 A는 평면 위의 모든 점을 일대일 대응시킴. 존재하지 않는다면 원점을 지나는 직선으로 옮기거나($A\neq O$), 원점으로 옮김($A=O$)
* $A$로 옮긴 도형의 넓이는 `det(A)`배가 됨.

{% capture context1 %}  
### 일차변환과 행렬
행렬과 일차변환에 대한 연관관계는 [행렬](/posts/mathematics/#행렬) 파트를 참조  
한줄요약하자면 - 행렬과 일차변환은 같다(일대일 대응)

그런의미에서 일차변환은 행렬의 성질을 죄다 만족한다.  
항등변환? ㅇㅋ $I=\begin{pmatrix} k & 0 \\\\ 0 & k\end{pmatrix}$  
닮음변환? ㅇㅋ $kI$  
합성? ㅇㅋ $g(=B) \circ f(=A) = BA$  
역변환? ㅇㅋ $A^{-1}$  
^^

회전변환은 $\begin{pmatrix} \cos\theta & -\sin\theta \\\\ \sin\theta & \cos\theta \end{pmatrix}$으로 계산되며, 증명은 다음단계에

<br/>

{% endcapture %}

{% capture context2 %}
### 회전변환행렬의 증명 + 좌표축의 회전이동
![Alt text](/pictures/mathematics/회전이동.png){: width="65%" height="65%"}  
앗 증명하려고 했는데 그림이 너무 잘 되있었다. [ㄳ](http://suhak.tistory.com/387)  
$\begin{pmatrix} x' \\\\ y'\end{pmatrix} = \begin{pmatrix} \cos\theta & -\sin\theta \\\\ \sin\theta & \cos\theta \end{pmatrix} \begin{pmatrix} x \\\\ y\end{pmatrix}$

그런김에 다른 얘기나 해보자  
좌표축을 $\theta$만큼 회전이동할 때 점 $P(x, y) \to P(X, Y)$로 변한다면,
$\begin{pmatrix} X \\\\ Y\end{pmatrix} = \begin{pmatrix} \cos\theta & \sin\theta \\\\ -\sin\theta & \cos\theta \end{pmatrix} \begin{pmatrix} x \\\\ y\end{pmatrix}$ 로 기존 변환 $A$의 역변환인 $A^{-1}$이 취해진다.  
직관적이긴 하지만, 증명 가능한가?

지금까지 정의한, 같은 좌표계에서 점의 위치를 옮기는 변환을 `active transformation`,  
반대로 점을 그대로 둔 채 좌표계를 옮기는 변환을 `passive transformation` 이라고 한다.
  
원래 점의 좌표 $\mathbf{v}=(v_x, v_y, v_z)^T$, active transformation $T$, 그리고 기저 $\hat{e_x}, \hat{e_y}, \hat{e_z}$가 있다고 생각해보자.  
`Active transformation` 이란, 점의 좌표를 $T$로 변환하는 것을 뜻한다. 즉 $\mathbf{v}'=T\mathbf{v}=T(v_x, v_y, v_z)^T$.   
`Passive transformation` 이란, 점이 아닌 좌표계의 기저를 $T$로 변환하는 것을 뜻한다. 즉 $\hat{e'_i}=T\hat{e_i}$.
  
Passive transformation 이후, 점의 벡터 $v_x\hat{e_x}+ v_y\hat{e_y}+ v_z\hat{e_z}$는 새로운 기저 $v'_x\hat{e'_x}+ v'_y\hat{e'_y}+ v'_z\hat{e'_z}$로 표현된다.  
$v_x\hat{e_x}+ v_y\hat{e_y}+ v_z\hat{e_z} = v'_x\hat{e'_x}+ v'_y\hat{e'_y}+ v'_z\hat{e'_z} = v'_x T\hat{e_x}+ v'_y T\hat{e_y}+ v'_z T\hat{e_z}$  
(주의, $\hat{e_x}$은 벡터, $v'_x$는 계수이고 $T$는 행렬이다.)  
즉, $(v_x, v_y, v_z)^T = T(v'_x, v'_y, v'_z)^T, \mathbf{v}'= T^{-1}(v_x, v_y, v_z)^T = T^{-1}\mathbf{v}$ 이 된다.
  
위의 active transformation 에서의 변환관계와 비교해 보면, $T$ 대신 $T^{-1}$가 들어가 있음을 알 수 있으며,  
따라서 일차변환 $T$로 좌표변환(passive transformation)을 하였을 때 점의 좌표변화는 $T^{-1}$로 직접 변환(active transformation)한 것과 동치임이 증명된다. 와와  

<br/>

### 일차변환과 도형의 넓이 
행렬 $A=\begin{pmatrix} a&b\\\\c&d \end{pmatrix}$ 로 변환한 도형의 넓이가 $det(A)=\|ad-bc\|$배가 된단다. 왤까.  
일단 임의의 벡터 $u, v$가 생성하는 평행사변형의 넓이를 $S(u, v)$라고 표기하자.  
($u, v$가 반시계방향으로 배치되어야 양수, 시계방향으로 배치되면 음수이다)  
![Alt text](/pictures/mathematics/일차변환_영역.JPG)  
$S(u+w, v) = S(u, v) + S(w, v)$가 된다. 마찬가지로 $S(u, v+w) = S(u, v) + S(u, w), S(au, v)=aS(u, v)$도 성립한다.

일단 $u=\hat{e_1}=(1, 0),\, v=\hat{e_2}=(0, 1)$과 같은, 단위정사각형을 생각해 보자.  
그렇다면 $u, v$를 일차변환한 값 $u'=(a, c)=a\hat{e_1} + c\hat{e_2},\, v'=(b, d)=b\hat{e_1}+d\hat{e_2}$를 평행사변형의 변으로 하는 넓이 $S(u', v')$은  
$S(u', v')=S(a\hat{e_1} + c\hat{e_2}, b\hat{e_1}+d\hat{e_2})$가 되는데...  
$S(\hat{e_1}, \hat{e_1}) = S(\hat{e_2}, \hat{e_2}) = 0$과 같이, $x$나 $y$방향의 벡터 2개에 대한 넓이는 0이니까, 이를 소거해서 정리하면  
$\|S(u', v')\|=adS(\hat{e_1}, \hat{e_2}) +  bcS(\hat{e_2}, \hat{e_1})= \|(ad-bc)S(\hat{e_1}, \hat{e_2})\|=\|ad-bc\|$가 된다.  
단위정사각형에 대해서 넓이 변화가 $\|ad-bc\|$배가 되는 것을 확인했으니, 이제 $u, v$를 $d\hat{e_1}, d\hat{e_2}$로 무한히 작게 만들고 합치면 어떤 영역에 대해서도 넓이비가 $\|ad-bc\|$배가 된다.

이는 3차원에서도 성립한다. 정사각형->평행사면체가 아닌 정육면체->평행사면체 박스 정도가 되겠지만, 암튼 단위정육면체의 넓이 변화는 정확히 행렬식과 같다.  
[참고](https://twlab.tistory.com/44)

-------------------------------------

여기까지가 인터넷을 좀 뒤져 보면 나와 있는 내용들이다.  
음 근데 솔직히 막 마음에 들진 않았다.  
일단 기본이 원점을 한 꼭짓점으로 두는 평행사변형에 기반한 증명이라, 원점을 벗어난 부분에 대해서는 평행이동이 계속 들어가야 한다던가,  
아무튼 막 명쾌하진 않았다.  
그래서 나름 머리를 굴렸고, 내 기준 어느 정도 괜찮은 해답을 얻은 것 같다.

일단 넓이나 부피, 아니 더 일반적으로 어떤 `물리량`이란 어떻게 정의되는가.  
예를 들어 기체 상수 $R$이라는, 어떤 불변인 상수가 $J\cdot mol^{-1}\cdot K^{-1}$ 단위로 나타내지면 $8.314472$가 되고,  
$L\cdot atm\cdot mol^{-1}\cdot K^{-1}$ 단위로 나타내지면 $0.008205784$가 되듯이,  
기체 상수의 물리량은 $1J,\, 1mol^{-1},\, 1K^{-1}$을 하나씩 곱한 것 보다 $8.314472$배가 크고, $1L,\, 1atm,\, 1mol^{-1},\, 1K^{-1}$을 하나씩 곱한 것의 $0.00820$어쩌고배가 된다는 것을 의미한다.  

> 이렇듯 어떤 물리량을 정의하기 위해선 `단위`라는게 필요하고, 어떤 물리량은 그 단위를 구성하는 각 `차원`의 `기저`를 모두 곱한 것의 몇 배가 되는지를 뜻한다.  

이러한 관점에서, 머리 아프게 넓이를 구성하는 점 자체를 active transform 시키지 말고, 반대로 단위 변환에 해당되는, 기저를 변환시키는 passive transform 관점에서 생각해보자.  
아이디어는 이거다 - Active transform $A$ 대신 passive transform $A^{-1}$을 사용하면, 단위 영역의 크기가 $\dfrac{1}{\|ad-bc\|}$가 되니까, 영역의 크기는 $\|ad-bc\|$배가 되지 않겠는가?  
한줄로 요약되는 단순한 아이디어지만, 언젠가 까먹을 때를 대비해서 좀 자세히 풀어서 설명해 보자.
  
![Alt text](/pictures/mathematics/일차변환_영역2.JPG)  
우선 넓이라는 것은, 좌표계를 구성하는 차원들의 기저 $\hat{e_1}=(1, 0),\, \hat{e_2}=(0, 1)$가 이루는 영역의 몇배인지를 나타내는 값이다.  
  * 넓이 = $S\times\text{Area}(\hat{e_1}, \hat{e_2}) = S[\hat{e_1} \hat{e_2}]$로 표기하자. (대괄호 안의 값은 단위계이고, 단위계는 각 기저의 곱으로 표기된다.)
  
기저를 일차변환 $A$로 변환시키면 변환된 좌표계는 $\hat{e'_1}, \hat{e'_2}$를 기저로 가지게 되는데,  
$\hat{e_1}$은 $\hat{e'_1}=a\hat{e_1} + c\hat{e_2}$로, $\hat{e_2}$은 $\hat{e'_2}=b\hat{e_1} + d\hat{e_2}$로 변환되고,  
변환된 단위계에서 넓이 1을 나타내는 회색 영역은, 원래 단위계에서는 위에서 구했듯이 $\|ad-bc\|$이라는 넓이 값을 가지게 된다. 
  * 회색 넓이 = $1[\hat{e'_1} \hat{e'_2}] = \|ad-bc\|[\hat{e_1} \hat{e_2}]$
  
자 이제 임의의 파란색 영역의 넓이를 생각해 보자.  
임의의(파란색) 넓이 = $S[\hat{e_1} \hat{e_2}] = S[\hat{e_1} \hat{e_2}] \times \dfrac{1[\hat{e'_1} \hat{e'_2}]}{\|ad-bc\|[\hat{e_1} \hat{e_2}]} = \dfrac{S}{\|ad-bc\|}[\hat{e'_1} \hat{e'_2}] = S'[\hat{e'_1} \hat{e'_2}]$  
즉 $S' = \dfrac{S}{\|ad-bc\|}$, 변환된 단위(좌표계)에서의 넓이는 변환에 사용된 passive transform에 사용된 행렬의 행렬식을 나눈 값과 같다.  
그런데 우리가 처음 생각한 문제는, 어떤 영역을 $A$로 active trasnform시켰을 때 영역의 변화이다.
  
> 어떤 영역을 $A$로 active trasnform시키는 것은, $A^{-1}$로 passive transform시키는 것과 동일하고, $det(A^{-1})=\dfrac{1}{det(A)},\, S'= \dfrac{S}{1/det(A^{-1})}=S \times det(A)$.
  
됬다.


3줄요약하자면
1. 일차변환 $A$는 좌표계를 $A^{-1}$로 변환시키는 것과 같고, 이는 기존 좌표계의 기저벡터를 $A^{-1}$ 변환시킨다는 의미이며  
3. 기저벡터가 이루는 영역(정사각형->평행사변형)은 곧 영역의 단위이며, 영역의 단위는 기존의 $det(A^{-1})$배, 즉 $\dfrac{1}{det(A)}$배가 되며 
4. 단위가 $m \to cm$로 100분의 1로 줄면 키를 나타내는 숫자는 1.8에서 180으로 100배가 되듯이, $det(A)$분의 1로 줄어든 단위에서 영역은 기존의 $det(A)$배가 된다.

-----------------------------------------------------

끝내려고 했는데 쓸만한게 하나 더 생각났다.  
행렬식의 정의가 인터넷에 나와있는건 좀 뭔가 좀 그런데  
위 아이디어에 따라서, 행렬 $A$의 행렬식을 다음과 같이 생각해보자.  

> $n$차 정사각행렬 $A$의 행렬식은, 벡터 공간의 기저를 $A$로 변환시켰을 때 변환된 기저가 이루는 영역을 의미한다. 

3차원을 예로 들어보자. $A$에 의해 변환된 기저 $\hat{e'_1}, \hat{e'_2}, \hat{e'_3}$는 평행사변형 박스를 이룰 것인데,  
이 박스의 부피가 곧 행렬식을 의미한다는 것이다.  

2차원에서 두 벡터가 이루는 평행사변형의 넓이 $S(u+w, v)=S(u, v)+S(w, v)$에서 봤듯이,  
3차원에서도 이 선형성이 성립한다는 합리적 의심 하에(어차피 행렬이 곧 일차변환이고, 일차가 선형이니까) 한번 전개해 보자.  

$A=\begin{pmatrix}a_{11}&a_{12}&a_{13}\\\\a_{21}&a_{22}&a_{23}\\\\a_{31}&a_{32}&a_{33}\end{pmatrix}, A\bar{e_i}=\begin{pmatrix}a_{1i}\\\\a_{2i}\\\\a_{3i}\end{pmatrix}$,  
$S(A\bar{e_1}, A\bar{e_2}, A\bar{e_3}) = S(a_{11}\bar{e_1}+a_{21}\bar{e_2}+a_{31}\bar{e_3}, a_{12}\bar{e_1}+a_{22}\bar{e_2}+a_{32}\bar{e_3}, a_{13}\bar{e_1}+a_{23}\bar{e_2}+a_{33}\bar{e_3})$  
$\;= a_{11}S(\bar{e_1}, a_{12}\bar{e_1}+a_{22}\bar{e_2}+a_{32}\bar{e_3}, a_{13}\bar{e_1}+a_{23}\bar{e_2}+a_{33}\bar{e_3})$  
$\quad + a_{21}S(\bar{e_2}$, 어쩌고저쩌고$) + a_{31}S(\bar{e_3}$, 어쩌고저쩌고)  
첫번째 항만 생각해보자. $S$의 첫번째 벡터가 $\bar{e_1}$이니까 넓이 구하는데 있어서 $\bar{e_1}$항은 아무런 의미가 없으니 빼보면  
$a_{11}S(\bar{e_1}, a_{22}\bar{e_2}+a_{32}\bar{e_3}, a_{23}\bar{e_2}+a_{33}\bar{e_3}) = a_{11}(a_{22}a_{33}-a_{32}a_{23})S(\bar{e_1}, \bar{e_2}, \bar{e_3})$.  
뭔가 익숙한 냄새가 난다. 뒤에 항에 대해서도 해 보면 최종 넓이가 $det(A)$이 됨을 확인할 수 있다.  
와와 
* [Wedge product](http://mathworld.wolfram.com/WedgeProduct.html)에서 비슷한 그런게 있는듯하다.  
  Volume element를 $dV=dx_1\wedge dx_2\wedge \cdots \wedge dx_n$ 으로 나타내고 어쩌고 하는듯하다.

<br/>

### 변환행렬(탈급식)
변환행렬 관련해선 쓸 얘기가 (상당히)많기 때문에,  
우선 큰 흐름 위주로만 던져놓고, 나중에 좀 더 자세히 다루도록 함.

<br/>

#### Affine transformation 
- [수학적으로는](https://ko.wikipedia.org/wiki/%EC%95%84%ED%95%80_%EB%B3%80%ED%99%98): 공선점을 보존하는(즉, 변환 전에 같은 선 위에 있으면 변환 후에도 같은 선 위에 있다) 두 아핀 공간 사이의 변환이며,  
- 쉽게 말해서: 그냥 선형 변환 + 평행 이동이다.

본인이 `아핀 변환`을 접하게 된 계기는, 그러니까 음 내 시야로부터 어떤 물체가 $\vec{X_{eye}}$ 만큼 떨어져 있다고 치고,    
이걸 잡고 싶다면, 팔꿈치로부터 내 손을 얼마나 움직여야되는가, 즉 $\vec{X_{elbow}}$ 를 어떻게 구하느냐 의 문제이다.  
즉, 눈의 좌표계 원점을 팔꿈치 좌표계까지 이동해야되고(`평행 이동`) + 동시에 좌표축도 회전시켜야 한다(`선형 변환`).  
물론 점의 변환과 좌표변환은 다르지만, 위에서 언급했듯이 변환에 inverse만 취하면 되니까..  


##### 평행 이동
$\begin{bmatrix}x'\\\\y'\\\\z'\end{bmatrix}=\begin{bmatrix}t_x\\\\t_y\\\\t_z\end{bmatrix} + \begin{bmatrix}x\\\\y\\\\z\end{bmatrix}$  
즉, $X'=X+T$
쉽다.

##### 선형 변환
우선, `선형성`이란 $f(ax+y)=af(x)+f(y)$를 의미한다.  
그렇기 때문에 `선형 변환`은 원점을 보존해야 하며($f(O) = O \because f(O)=f(O+O)=2f(O)$),  
원점을 어딘가 밖으로 날려버리는 평행이동은 당연히 제외된다.  
앗 그런데 `선형 변환`(일차변환)은 `행렬`이다. 어디보자. $A(aX+Y)=aAX+AY$. 굿.  
그러니까 $X'=AX$. 좋다.   

그러면, 선형 변환엔 어떤 것들이 있는가  
![Alt text](/pictures/mathematics/선형변환.png)  
스케일이 같은 2차원 변환에 대해선 그림과 같으며, 스케일은 $\begin{bmatrix}x'\\\\y'\\\\z'\end{bmatrix}=\begin{bmatrix}s_x&0&0\\\\0&s_y&0\\\\0&0&s_z\end{bmatrix} \begin{bmatrix}x\\\\y\\\\z\end{bmatrix}$과 같이 각 축에 대해 바꿀 수 있다.
얘들을 잘 곱하면, 임의의 행렬을 만들 수 있다. 

--------------------------------------------------   

이제 두 식을 합쳐보면, $X'=AX+T$ 로 임의의 affine transform을 2개의 행렬($A,\, T$)로 나타낼 수 있다.  
하지만 하나의 변환에 2개의 행렬이 필요하다니. 기분이 나쁘다.  
이 affine transform을 하나의 행렬로 깔끔하게 결합하기 위해서, `homogeneous coordinate`를 도입해야 할 필요가 있다.

<br/>

#### Homogeneous Coordinates
$[x, y, z] = [x, y, z, 1] = [wx, wy, wz, w]$ 로 표현하는 것. 일반적으론 좌표계에 한 차원을 더 붙이는 것(ex: $[x_1, x_2, \cdots, x_n] \to [x_1, x_2, \cdots, x_n, 1]$)  
영상학적으로는 아래와 같은 해석이 가능하다.  
![Alt text](/pictures/mathematics/homogeneous_coord_1.png){: width="45%" height="45%"} ![Alt text](/pictures/mathematics/homogeneous_coord_2.png){: width="45%" height="45%"}    
즉, $w$는 거리이자 동시에 스케일이다(거리가 $w$로 늘어나면 영상의 스케일이 $w$만큼 커진다).  

하지만 그런건 잘 모르겠고, affine transformation의 표현을 살펴보자.  
$X=[x, y, z, 1]$으로 둔다면, $X'=\begin{bmatrix}a_{11}&a_{12}&a_{13}&t_x\\\\a_{21}&a_{22}&a_{23}&t_y\\\\a_{31}&a_{32}&a_{33}&t_z\\\\0&0&0&1\end{bmatrix}X =MX$ 로 
$T$와 $A$가 하나의 행렬 $M=\begin{pmatrix}A&T \\\\ 0&1\end{pmatrix}$으로 합쳐진다!

#### 문제 해결?
그래서, 처음 문제인 $\vec{X_{eye}} \to \vec{X_{elbow}}$ 를 어케 구하느냐?  
눈 좌표계와 팔꿈치 좌표계의 위치 관계를 알고 있다면(즉, 눈 좌표계에서 잰 팔꿈치의 원점 $T_{eye2elbow}$, 그리고 눈 좌표계로부터 팔꿈치 좌표축의 회전행렬 $A_{eye2elbow}$를 알고 있다면)  
$\vec{X_{elbow}} = M_{eye2elbow}^{-1}\vec{X_{eye}}$가 된다! (다시 말하지만, 좌표변환은 점의 평행이동과 변환 방향이 반대임)

와! 근데 그래서 회전행렬 $A_{eye2elbow}$ 가 대체 뭐죠?  
와!~~~~~~~

<br/>

#### 3d rotation matrix 구하기..
일단 원점이 떨어져 있는 문제는 평행이동 벡터(translation vector)를 구해서 해결했으니, 일단 원점이 같은 상황을 생각하자.  
좌표계의 회전을 어떻게 행렬로 표기할 것인가? 그 전에, 행렬이 아니라 뭐던 간에 좌표계의 회전을 어떻게 표기할 것인가?  

![Alt text](/pictures/mathematics/RPY_1.png) ![Alt text](/pictures/mathematics/RPY_2.png)  
$x$축 하나만 생각해서, 바뀐 $x'$축의 위치를 구면좌표계처럼 각도 2개로 표현하는 것이 맨 처음 떠오르겠지만,  
안타깝게도 $x'$축을 결정한 뒤로는 $y'$축과 $z'$축을 어떻게 배열할 것인지의 문제가 또 남는다. 즉 3차원 좌표축 회전은 자유도가 3인 문제이다.

오일러는 `euler angle`이라는 걸 언제 또 만들어서, 이러한 좌표축 회전을 표기하려 했는데,  
아이디어는 일단 $x'=x, y'=y, z'=z$인 상황에서, 
* $z$축을 중심으로 한번 회전($\alpha, \psi$)시키고, 
* 회전된 $x$축($x'$축)을 기준으로 한번 회전($\beta, \theta$)시키고,
* 다시 회전된 $z$축($z'$축)을 기준으로 순서대로 회전($\gamma, \phi$)시키면, 

임의의 좌표축 회전을 나타낼 수 있다는 것이다.  
이를 변형한 것이 `RPY` 표기법인데, X축 회전을 `Roll`, Y축 회전을 `Pitch`, Z축 회전을 `Yaw` 로 두고 순서대로(R->P->Y) 회전시켜서 표현하는 것이다. (YPR처럼 순서가 바뀌면 각도 바뀐다!)
 
아무튼 눈 좌표계로부터 팔꿈치 좌표계까지의 회전행렬을 구하고 싶다?
1. 일단 RPY 각도를 구해라
2. 아래 그림이 각 축에 대한 회전변환 행렬인데, 얘들을 하나씩하나씩 차근차근 구해라  
   ![Alt text](/pictures/mathematics/회전변환.JPG)
3. $X_R = A_R^{-1} X_0, X_RP=A_P^{-1} X_R, X_RPY=A_Y^{-1} X_RP$,  
   즉 $X_RPY=A_Y^{-1} A_P^{-1} A_R^{-1} X_0$ 가 된다...

하지만 이러한 표기법은 짐벌 락 등 문제점들이 있다.  
짐벌 락은 얘가 뭐가 문젠지는 저어도 자세히는 모름  
아무튼 사실 RPY 각도를 구하는것도 말이 쉽지 썩 와닿지는 않는다. 구글에 검색해 보면 3차원 회전행렬(rotation matrix)을 구하는 갖가지 방법이 나오지만 토나온다.  
여기선 3차원 행렬을 구하는 방법 대신, 또 다른 표기법인 `quaternion`에 대해서 마지막으로 살펴보자.


#### quaternion
`Quaternion`, 그러니까 `사원수`는.. 일단 복소수를 확장한 대수적인 그런 개념이다... 그러니까 음....
![Alt text](/pictures/mathematics/복소평면.png)  
복소평면을 보면, 실수항을 기저로 하나($x$축), 복소수항을 기저로 하나($y$축) 그렇게 그리듯이  
![Alt text](/pictures/mathematics/quaternion.png){: width="50%" height="50%"}  
얜 그런 $r$(실수), $i$같은 기저가 $r, i, j, k$ 4개임. 엌ㅋㅋ  
그러니까 기본적으로 $i^2=-1$처럼 $j^2=-1,\, k^2=-1$이고, 동시에 $i, j, k$ 끼리도 직교하기 때문에 $ij=k$ 같은 성질도 만족함.  

일단 더 자세한 quaternion 에 대한 설명은 위키를 뒤져보시던 아니면 [이 갓영상](https://www.youtube.com/watch?v=d4EgbgTm0Bg&t=0s) 을 참조하시고  
quaternion 과 3d rotation과의 연관관계는 [이 영상](https://www.youtube.com/watch?v=d4EgbgTm0Bg&t=0s) 을 참조..   
직접 쓰는건 나중에 쓰던가 해야.. 어차피 고등학교 섹션에 들어갈 내용은 아니잖아 이미 망했지만 

간단히 요약하면, quaternion 은 하나의 회전변환에 대응되고, 하나의 rotation matrix를 표현하는 것이 가능함.  
그러니 난 회전행렬을 알고싶은데 왠 q자로 시작하는 듣보벡터가 나오네? 싶으면 당황하지 말자. 

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="기벡_일차변환" %}

### 공간도형과 정리
공간도형에 관한 정리는 4가지 섹션으로 구분되어 있다.
1. 점, 직선, 평면을 결정하는 조건
2. 직선과 평면의 위치 관계
3. 직선과 평면이 이루는 각
4. 직선과 평면의 수직에 관한 정리

* 정사영: 도형 $F$를 이루는 점 $P$에서 평면 $\alpha$에 내린 수선의 발로 이루어진 도형 $F'$, 
  * 평면 $\alpha$와 각도 $\theta$를 이루는 평면 $\beta$ 위의 넓이 $S$인 도형의 정사영의 넓이 $S'=S\cos\theta$

{% capture context1 %}
### 점, 직선, 평면을 결정하는 조건
1. 공간도형의 기본 성질
    * 한 직선 위에 있지 않은 서로 다른 세 점을 지나는 평면은 단 하나 존재한다.
    * 한 평면 위의 서로 다른 두 점을 지나는 직선 위의 모든 점은 이 평면 위에 있다.
    * 서로 다른 두 평면이 한 점을 공유하면 이 두 평면은 그 점을 지나는 한 직선을 공유한다.
2. 평면을 결정하는 조건
    * 한 직선 위에 있지 않은 세 점은 단 하나의 평면을 결정한다.
    * 한 직선과 그 위에 있지 않은 한 점은 단 하나의 평면을 결정한다.
    * 서로 만나는 두 직선은 단 하나의 평면을 결정한다.
    * 평행한 두 직선은 단 하나의 평면을 결정한다.
3. 직선을 결정하는 조건
    * 서로 다른 두 점은 단 하나의 직선을 결정한다.
    * 서로 만나는 서로 다른 두 평면은 단 하나의 직선을 결정한다.
4. 점을 결정하는 조건
    * 서로 만나는 두 직선은 단 하나의 점을 결정한다.
    * 평면과 그 평면에 포함되지 않은 직선이 만나면 단 하나의 점을 결정한다.
    * 교선이 평행하지 않은 서로 다른 세 평면은 단 하나의 점을 결정한다.


### 직선과 평면의 위치 관계
1. 평면과 평면의 위치 관계
    * 한 직선에서 만난다
    * 만나지 않는다 (평행)
2. 평면과 직선의 위치 관계
    * 직선이 포함된다
    * 한 점에서 만난다
    * 만나지 않는다 (평행)
3. 직선과 직선의 위치 관계
    * 한 점에서 만난다 - 한 평면 위에 있다
    * 평행하다 - 한 평면 위에 있다, 만나지 않는다
    * 꼬인 위치에 있다 - 만나지 않는다


### 직선과 평면이 이루는 각
1. 꼬인 위치에 있는 두 직선($a, b$)이 이루는 각
    * 점 $O$를 지나고 $a, b$와 평행한 $a', b'$를 그을 때, $a', b'$가 이루는 각
2. 직선과 평면의 수직
    * 직선 $l$이 평면 $\alpha$와 점 $O$에서 만나고, $O$를 지나는 $\alpha$ 위의 모든 직선과 수직일 때 $l\perp\alpha$
    * $l$을 $\alpha$의 수선, $O$를 수선의 발이라고 함
3. 직선과 평면이 이루는 각
    * 직선 $a$가 평면 $\alpha$와 점 $O$에서 만나고, $a$위의 임의의 점 $A$에서 내린 수선의 발 $B$에서 $a$와 $\alpha$가 이루는 각도는 $\angle AOB$이다.
4. 두 평면이 이루는 각
    * 두 평면의 교선을 공유하는 두 반평면이 이루는 도형을 이면각, 두 평면의 교선을 이면각의 변이라 한다. 
    * 각 면에서, 이면각의 변 위의 한 점 $O$를 지나고 이면각의 변과 수직한 직선 $OA, OB$를 그을 때, 이면각의 크기 = $\angle AOB$
    * $\angle AOB=90$도 일 때 $\alpha \perp \beta$


### 직선과 평면의 수직에 관한 정리
1. 평면 $\alpha$ 위의 평행하지 않은 두 직선 $a, b$에 모두 수직인 직선 $l$은 $l\perp \alpha$이다.
2. 삼수선의 정리
    * $P$를 평면 $\alpha$밖의 점, $a$를 평면 $\alpha$ 위의 직선이라 할 때
    * $P$에서 $\alpha$에 내린 수선의 발을 $M$, $M$에서 $a$에 내린 수선의 발을 $N$이라 하면 $\overline{PN}\perp a$ 
    * $P$에서 $\alpha, a$에 내린 수선의 발을 $M, N$이라 하면 $\overline{MN}\perp a$
    * $P$에서 $a$에 내린 수선의 발을 $N$, $\alpha$ 위에서 $a$에 수직이고 $N$을 지나는 직선을 $b$라 하면 $P$에서 $b$에 내린 수선 $\overline{PM}\perp \alpha$
3. 기타
    * 직선 $l$이 평면 $\alpha$에 수직일 때, $l$을 포함하는 모든 평면은 $\alpha$에 수직
    * 한 점 $P$를 지나고 평면 $\alpha$에 수직인 직선은 단 하나
    * 한 점 $P$를 지나고 직선 $l$에 수직인 평면은 단 하나
    * 한 평면에 수직인 두 직선은 서로 평행하다
    * 한 직선에 수직인 두 평면은 서로 평행하다
    * 한 평면에 수직인 두 평면의 교선은 처음 평면에 수직

<br/>
    
### 정사영
![Alt text](/pictures/mathematics/정사영.png){: width="60%" height="60%"}  
정사영같은 경우에는, 두 평면에서 이면각의 변과 평행한 선은 줄어들지 않고, 이면각의 변과 수직인 부분만 $\cos\theta$만큼 줄어든다.  
증명까진 필요없을거같고, 그냥 이면각의 변과 평행, 수직한 기저를 가지는 기존 좌표계 $\beta$에서  
수직한 기저에서의 값만 $\cos\theta$배로 줄이는 active transform이 가해져서 $\alpha$로 간다라고 보면 될듯?   

{% endcapture %}

{% capture context2 %}

내가 참.. 이 단원은 보면서 이걸 어떻게 할지 고민이 많았다.  
솔직히 하나하나 다 증명할 만한 가치는 있는데, 아 이건 너무 많잖아  
그리고 뭐 어차피 이거 하나하나 다 증명해봤자 어차피 그냥 책에 다 있는 내용 옮겨쓰는거랑 똑같은데 굳이 해야하나 싶어서  
그냥 증명은 패스하고 나중에 필요하다 싶으면 미래의 내가 해주겠지 몰라 

### 유클리드 원론(Euclid's Elements)
대신 유클리드 원론을 드리겠습니다.  
와와

유클리드 원론이란, 이성과 합리성의 노예들인 고오대그리스인들 답게  
각 개념에 대한 `정의`,  
그 개념들이 만족하는 증명없이 받아들일 수 있는 사실상 자명하게 성립하는 명제인 `공리` 5개
그리고 사실상 공리와 같으나, 부정될 가능성을 생각하며 이 이론체계에서 가정된 전제로서의 성격을 가지는 5개의 `공준`을 기반으로  
항상 성립하는 명제인 `정리`들을 총 13권의 책에서 총합 465개를 하나하나씩 쌓아서 만든(물론 수학이 다 그렇지만) 세계 최초의 수학 교과서라고 한다. 

1~4권에서는 2차원 기하학, 5~10권에서는 기초적인 수론, 11~13권에서는 3차원 기하학을 다루는데  
그 중 1권에서는 5개의 공리와 5개의 공준, 그리고 48개의 정리를 증명한다.
자세한 부분은 [링크](https://mathcs.clarku.edu/~djoyce/java/elements/bookI/bookI.html#posts)나 [번역본](http://suhak.tistory.com/153)을 참고하고, 간단하게만 다뤄보자. 

#### 정의
23개의 정의가 있는데,  
점, 선, 선의 끝(점), 직선, 면, 면의 모서리(선), 평면, 평면각, 직선각, 직각과 수선, 둔각, 예각, 경계, 도형, 원, 원의 중심, 지름, 반원, 직선 도형과 다변형(다각형), 정삼각형과 이등변 삼각형, 직각삼각형, 둔각삼각형, 예각삼각형, 정사각형, 직사각형, 평행사변형, 평행선  
을 정의한다. 자세한 정의는 링크 ㄱㄱ  

#### 공리
공통 관념이라고도 하는 것 같다. 얘들은 양(magnitude)에 대한 것을 다룬다.

1. 똑같은 것과 같은 것들은 서로 같다. (삼단논법, $A=B \wedge B=C \Rightarrow A=C$)
2. 같은 것에 같은 것을 더하면 그 더한 전체는 여전히 같다($A=B \Rightarrow A+C=B+C$)
3. 같은 것에 같은 것을 덜어내도 그 나머지들은 여전히 같다($A=B \Rightarrow A-C=B-C$)
4. 포개어서(평행이동, 대칭이동) 같은 것들은 서로 같다.
5. 전체는 부분을 포함한다.  
   (그러니까, $B$가 $A$의 부분이라면 다른 나머지 $C$가 있다, 즉 $A=B+C$인 $C$가 존재한다 라는 것을 말하고 싶었단다..) 

#### 공준
1. 임의의 점에서 임의의 점으로 직선을 그릴 수 있다. (두 점은 한 직선을 결정한다)
2. 선분을 이어서 직선을 만들 수 있다.
3. 임의의 중심과 반지름을 가진 원을 그릴 수 있다.
4. 모든 직각은 서로 같다.
5. 두 직선과 한 직선이 만날 때, 두 직선을 한없이 늘린다면 같은 쪽에 있는 내각을 더해서 직각 둘(180도)보다 작은 쪽에서 만난다.  
   (한 직선 밖의 한 점을 지나면서 평행을 이루는 직선은 오직 하나이다) 


여기서, 진짜 트집잡고 싶어도 잡을게 없는 다른 공준에 비하여 좀 추한 5번 공준을,  
공준이 아닌 증명 가능한 정리로 둬서 증명해볼 수 있지 않을까 싶은 생각이 들어서 달려들었지만 결국 실패하고  
아예 유클리드 기하학이 아닌 새로운 공리계를 이루는 타원기하학(오직 하나->없음)과 쌍곡선 기하학(오직 하나->개많음)과 같은 비유클리드 기하학을 찾았다는 것은 
너무 유명한 일례라서 굳이 넣어야되나 싶긴 했는데 그래도 예의상 넣어줌.  
애초에, 공준의 정의 자체가 부정될 가능성을 생각했지만 일단 이 이론체계에서는 성립한다고 가정을 해놓은 '전제' 라는 것을 다시 한번 상기하자.


정리는.. 너무 많아서 패스할건데 대충 인상적인 것들만 뽑아보자면  
* 20 - 어떤 삼각형이든 두 변의 합은 나머지 한 변보다 크다.  
* 32 - 어떤 삼각형이든 한 변으로 만들어지는 외각은 맞은 편 두 내각의 합과 같고 삼각형 세 내각의 합은 180이다.  
* 47 - 직각삼각형에서 직각과 마주 보는 변을 가지고 정사각형을 만들면, 넓이는 나머지 다른 변으로 만든 정사각형 넓이를 더한 것과 같다(피타고라스 정리)
  
등 뽑고나니까 다 삼각형이네 작성자 삼각형성애자로 밝혀져 충격

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="기벡_공간도형" %}

### 벡터
> 이 항목은 교육과정을 족갑니다.  
> > 솔직히 공대생이라면 여기 교육과정 내용은 까먹는게 더 힘들기 때문에

* `벡터`는 `벡터공간`의 원소이다. 
* `벡터공간`이란
  * 일단 집합이고,
  * 스칼라 배가 잘 정의되며
  * '+' 연산에 대하여 가환군을 이루는 집합이다.
* 대표적으로 공간을 구성하는 벡터공간이 있으나, 함수들로 이루어진 벡터공간이라던가(함수->벡터) 행렬로 이루어진 벡터공간이라던가(행렬->벡터) 범위가 무지하게 높은듯하다.

{% capture context1 %}
### 수학적 정의
[위키](https://en.wikipedia.org/wiki/Vector_space), [나무위키](https://namu.wiki/w/%EB%B2%A1%ED%84%B0) 참조.  
`군`이나 `가환군`에 대한 설명은 [실수 체계](/posts/mathematics/#실수-체계) 참조  

> `체(field)` $F$에 대해, $V$가 $F$의 `$F$-가군(module)`이라면, $F$를 $V$의 `스칼라`라고 하고 집합 $V$를 $F$위의 `벡터 공간`이라 한다.

* `체`란 아래 성질을 만족하는 집합이다.
  * 덧셈에 대하여 가환군을 이룸 (덧셈에 대한 역원이 존재하므로 뺄셈이 항상 가능)
  * 곱셈에 대하여 가환군을 이룸 (0 제외) (곱셈에 대한 역원이 존재하므로 나눗셈이 항상 가능)
  * 덧셈과 곱셈에 대하여 분배법칙 성립 
  * 그니까 쉽게 말해서 유리수 실수 복소수같은놈들. 어디서 실수체 같은 말을 들어봤다면 이 체(field)를 뜻한다.

* $V$가 $F$의 `F-module`인 것이란, $V$가 $F$에 대하여 아래 성질을 만족하는 것을 뜻한다.
  * $(V, +)$는 가환군이다.
  * 함수 $f:F \times V \longrightarrow V,\; f(a, v)=a\cdot v$가 존재하고, 분배법칙과 교환법칙이 성립한다. 즉 $a, b\in F, u, v\in V$에 대하여,
    * $a\cdot(u+v)=a\cdot u+b\cdot v$
    * $(a+b)\cdot v=a\cdot v+b\cdot v$
    * $(ab)\cdot v=a\cdot(b\cdot v)$
    * $1\cdot v = v$
  * 쉽게 말해서, 가환군을 이루면서 실수같은 수 집합과 관계가 잘 정의되는 집합.
    
요약하자면, 벡터 공간이란 같은 집합 내에서도 연산이 잘 정의되고, 스칼라에 대해서도 연산이 잘 정의되는 집합이다.  
표기의 경우 $\vec{v}$와 같은 표기는 벡터가 방향을 나타내는 개념이 실제로 아니기 때문에(coordinate space에 대해서만 방향을 나타냄) 굵은 문자로 $\mathbf{v}$로 표기한다.

### 연산
암튼 벡터공간의 종류는 다양하지만(행렬을 생각해 보자. 저거 다 만족한다), 가장 대표적이고 간단한 케이스인 `coordinate space`을 예시로 들어서 설명한다.
  
* coordinate space: $(a_1, a_2, \cdots, a_n)$을 원소로 하는 집합. $a_i\in F$
* 벡터 표기: $\mathbf{A}=a_1\mathbf{e}_1+a_2\mathbf{e}_2+\cdots+a_n\mathbf{e}_n=(a_1, a_2, \cdots, a_n)$

연산을 살펴보자면
1. 덧셈: $\mathbf{A}+\mathbf{B}=(a_1+b_1, a_2+b_2, \cdots)$
2. scalar multiplication: $kA=(ka_1, ka_2, \cdots)$
3. `dot product`: $\mathbf{A}\cdot\mathbf{B}=a_1b_1+a_2b_2+\cdots$
4. `cross product`: 벡터 공간이 $\mathbb{R}^3$일 때 한정. $\mathbf{A}\times\mathbf{B}=(a2_b3-a_3b_2, a_3b_1-a_1b_3, a_1b_2-a_2b_1)$
    * 일반적인 벡터 공간에서 대응되는 개념은 [wedge product](http://mathworld.wolfram.com/WedgeProduct.html) 인데... 아직 제대로 정리가 안되서 보류.
    * 아닌가.. 텐서에 대해서는 cross product가 $(\mathbf{u}\times\mathbf{v})_i=\epsilon _{ijk}u_j v_k$(아인슈타인 표기법 사용)이라는거같기도 하고.. 역시 보류.
5. [del operator](https://namu.wiki/w/%EB%8D%B8(%EC%97%B0%EC%82%B0%EC%9E%90)): $\nabla$, 미분에 대응되는 연산자인데 사실상 벡터와 같이 취급된다.
    * `Gradient`: $\nabla f$
    * `Divergence`: $\nabla \cdot \mathbf{F}$
    * `Curl`: $\nabla \times \mathbf{F}$

{% endcapture %}

{% capture context2 %}
### 텐서
[괜찮은 유튜브](https://www.youtube.com/watch?v=f5liqUk0ZTw)  
텐서도 일단 보류. 아씨 모르겠다 난스레기야  
텐서는 씨 물리학부에선 제대로 알려주지도 않고 갑툭튀하다가 존재감없이 사라짐.  
누구는 0-rank tensor가 스칼라고 1이 벡터고 2가 matrix고 3-rank 이상까지 커버하는게 텐서다 라고는 하는데 내가 아는건 그게 전부는 아니다라는거 정도까지..
 
<br/>

### cross product의 기하학적 성질
드디어 좀 고등수학다운걸 합니다. 와와  
음 그러니까, $\mathbf{a}\cdot\mathbf{b}=a_1b_1+a_2b_2$(2차원에서) 으로 정의된건 알겠는데  
왜 그게 기하학적으로 $a$를 $b$로 정사영시킨 것이 되느냐, 그러니까 왜 $ab\cos\theta$가 되느냐. 를 다뤄보자.  

우선 $\mathbf{a}=(a\cos\alpha, a\sin\alpha),\, \mathbf{b}=(b\cos\beta, b\sin\beta)$로 두자.  
그럼 $\mathbf{a}\cdot\mathbf{b}=ab\cos\alpha\cos\beta+ab\sin\alpha\sin\beta$이고,
$\cos(\alpha-\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta$에 의해 $\mathbf{a}\cdot\mathbf{b}=ab\cos(\alpha-\beta)=ab\cos\theta$가 된다. 끝
  
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="기벡_백터" %}

### 벡터방정식
* 직선의 벡터방정식: 
  * $\mathbf{a}$를 포함하고 $\mathbf{b}$에 평행: $\mathbf{x}=\mathbf{a}+t\mathbf{b} \;\to\; \dfrac{x-a_1}{b_1}=\dfrac{x-a_2}{b_2}=\dfrac{x-a_3}{b_3}$
  * $\mathbf{a}, \mathbf{b}$를 포함: $\mathbf{x}=(1-t)\mathbf{a}+t\mathbf{b} \;\to\; \dfrac{x-a_1}{b_1-a_1}=\dfrac{x-a_2}{b_2-a_2}=\dfrac{x-a_3}{b_3-a_3}$
* 평면의 벡터방정식:
  * $\mathbf{a}$를 포함하고 $\mathbf{h}$에 수직: $\mathbf{h}\cdot(\mathbf{x}-\mathbf{a})=0 \;\to\; h_1(x-a_1)+h_2(x-a_2)+h_3(x-a_3)=0$
  * $\mathbf{a}, \mathbf{b}, \mathbf{c}$를 포함: $\mathbf{x}=\mathbf{a}+s(\mathbf{b}-\mathbf{a})+t(\mathbf{c}-\mathbf{a}) \;\to\; h_1x+h_2y+h_3z+d=0$ 
* 구의 벡터방정식:
  * $(\mathbf{x}-\mathbf{a})\cdot(\mathbf{x}-\mathbf{a})=r^2\, (\|\mathbf{x}-\mathbf{a}\|=r) \;\to\; (x-a_1)^2+(x-a_2)^2+(x-a_3)^2=r^2$
* 영역:
  $\overline{OA}, \overline{OB}$를 변으로 하는 평행사변형: $\mathbf{p}=m\mathbf{a}+n\mathbf{b}\; (m,\,n\in[0, 1])$ 

# 미적분학
TBD

# TO BE DONE!
