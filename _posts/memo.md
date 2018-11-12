## 테스트
* ㅁㄴㅇㄹ
  * ㅁㄴㅇㄻ

* ㄴㅁㄹㅇ

* ㅁㄴㅇㄹ

실험1

ㄴㅁㄹㅇ

실험2 <br>

<br/>
sfda

* 실험
  * Minor matrix
  * 원래 행렬에서 $i$행 $j$열을 제거한 행렬. <br/>
<br/>

* 실험
  * Minor matrix
  * 원래 행렬에서 $i$행 $j$열을 제거한 행렬. <br/>

* 시험

줄나누기
줄나누기2<br/>
줄나누기3\
줄나누기4
ㅈ믐

## 고등수학

### 집합
서로 구별될 수 있는 것의 모임 전체. 집합을 구성하고 있는 개개의 대상은 원소라고 함.
<p> $$ 원소나열법, 조건제시법 $$ </p>

{% capture context1 %}
좀 더 엄밀한 정의?
집합의 포함 관계
<p> $$ 포함 관계 $$ </p>
부분집합
{% endcapture %}

{% capture context2 %}
집합의 연산
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="set" %}

### 명제와 조건
명제는 참/거짓을 내릴 수 있는 문장이며, 조건은 변수 $$ x $$에 값을 대입하면 명제가 되는 문장. <br/>
$$p$$이면 $$q$$이다: $$p \rightarrow q$$,
$$p \rightarrow q$$가 참이면 $$p \Rightarrow q$$,
진리집합 $$P$$, $$Q$$에 대해 $$P \subset Q$$ 이면 $$p \Rightarrow q$$

{% capture context1 %}
#### 조건
조건에 포함된 변수 $$x$$는 $$U \neq \varnothing$$ 을 정의역으로 함. <br/>
전체집합 $$U$$에서의 조건 $$p(x)$$를 간단히 조건 $$p$$라고 표기함. <br/>
$$U$$의 원소 $$a$$를 대입한 $$p(a)$$가 참인 명제라면, 명제 $$p(a)$$가 성립한다, $$a$$는 조건 $$p(x)$$를 만족한다 라고 함.

#### 부정
명제 $$p$$ 혹은 조건 $$p(x)$$에 대해 $$p(x)가 아니다$$ 를 $$p(x)$$의 부정이라 하고, $$\sim p(x)$$로 표기함. <br/>
<p> $$ \sim (p \vee q) \Leftrightarrow (\sim p \wedge \sim q), \sim (p \wedge q) \Leftrightarrow (\sim p \vee \sim q) $$ </p>
<p> $$ \sim (\forall x, p(x)) \Leftrightarrow (\exists x, \sim p(x)), \sim (\exists x, p(x)) \Leftrightarrow (\forall x, \sim p(x)) </p>

#### 진리집합
$$p(x)$$를 만족하는 $$x$$ 전체의 집합 $$P$$를 조건 $$p(x)$$의 진리집합이라고 한다. <br/>
$$P = \left\{ x | x \in U, p(x) \right\}$$. 표기시 전체집합 $$U$$를 씹으려는 경향이 강하므로 $$P=\left\{ x | p(x) \right\}로도 표기.

#### 조건과 집합
집합 $$P$$, $$Q$$를 조건 $$p$$, $$q$$의 진리집합이라고 둘 때, <br/>
<p> $$ P \subset Q \Leftrightarrow (p \Rightarrow q), P \nsubset Q \Leftrightarrow (p \nLeftarrow q), \\
p \vee q \Leftrightarrow P \cup Q, p \wedge q \Leftrightarrow P \cup Q, \sim p \Leftrightarrow P^c $$ </p>

#### 필요 · 충분 조건
$$p \Rightarrow q$$일 때, $$p$$는 $$q$$이기 위한 충분조건이고 $$q$$는 $$p$$이기 위한 필요조건이 된다. </br>
$$p \Leftrightarrow q$$ 면 서로 필요충분조건(동치). </br>
집합과의 관계는 $$P \subset Q \Rightarrow (p \Rightarrow q) $$임.

#### 귀류법
어떤 명제 $$p \rightarrow q$$임을 증명하려 할 때, 대우 $$\sim q \rightarrow \sim p$$를 증명하는 방법 </br>
명제의 결론을 부정하여 공리, 정리, 가정 등에 모순이 됨을 이끌어내면 된다.
{% endcapture %}

{% capture context2 %}

두 **조건** $$p$$, $$q$$를 $$p \rightarrow q$$ 꼴로 연결하면 명제가 되어버림. </br>
'4의 약수는 8의 약수이다' 를 풀어서 '$$x$$가 4의 약수이면 $$x$$는 8의 약수이다' 로 명제와 같이 표현가능. </br>

$$(P \subset Q) \Rightarrow (x \in P \Rightarrow x \in Q) \Rightarrow (p \Rightarrow q)$$ </br>

<p> $$ \sim (p \vee q) \Rightarrow (P \cup Q)^c \Rightarrow P^c \cup Q^c \Rightarrow \sim p \wedge \sim q $$ </p>
<p> $$ \sim (모든 x에 대하여 p(x)이다) \Rightarrow \sim (p(x1) and p(x2) and ... and p(xn)) \Rightarrow \sim p(x1) or \sim p(x2) or ... or \sim p(xn) \Rightarrow 어떤 x에 대하여 \sim p(x) $$ </p>
비슷한 방법으로 모두 증명 가능 </br>

귀류법이 옳다는 것을 증명하는 방법 : </br>
$$(p \rightarrow q) \Leftrightarrow (p \wegde \sim q) \rightarrow c$$ 임을 보이면 됨 ($$c$$는 항상 False)
가장 쉬운 방법으로는 진리표가 있음
https://m.blog.naver.com/PostView.nhn?blogId=da91love&logNo=220375037913&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F 참조

{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="명제" %}

### 실수 체계
일반적 연산에 대한 닫혀 있다(closed under) 의 개념과 항등원과 역원의 개념

{% capture context1 %}
#### 일반적 연산
집합 M의 두 원소 a, b의 순서쌍 (a, b)에 대응하는 M의 원소 c가 하나 정해질 때,
이 대응을 집합 M의 이항연산 또는 연산이라고 함.
기호 \bullet 등을 써서 a \bullet b = c 등으로 표기.

#### 교환, 결합법칙
교환법칙이 성립 <=> a \bullet b = b \bullet a
결합법칙이 성립 <=> (a \bullet b) \bullet c = a \bullet (b \bullet c)

#### 항등원, 역원
임의의 a \in N, 존재 e \in N, a \bullet e = e \bullet a = a일 때
원소 e를 연산 \bullet에 대한 항등원이라고 하며
임의의 a \in N, 존재 x \in N, a \bullet x = x \bullet a = e일 때
원소 x를 연산 \bullet에 대한 역원이라고 한다.
{% endcapture %}

{% capture context2 %}
할말없워요
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="실수체계" %}

### 정수 문제
최대공약수(GCD)와 최소공배수(LCM), 유클리드 호제법
기수법(p진법)의 정의

{% capture context1 %}
#### GCD, LCM
두 개 이상의 정수의 공통인 약수를 공약수라 하고, 그 중 가장 큰 수를 최대공약수라 함
두 개 이상의 정수의 공통인 배수를 공배수라 하고, 그 중 가장 큰 수를 최소공배수라 함

gcd{A, B} = G, lcm{A, B} = L이라 두면,
A = Ga, B = Gb (단, gcd{a, b} = 1)
L = Gab, LG = AB 를 만족함.

### 다항식의 GCD, LCM
다항식 A, B, Q 사이에 A=BQ이면 B를 A의 약수라고 표현한다.
2개 다항식 사이 공통인 약수를 공약수, 가장 차수가 높은 것을 최대공약수라고 함.
배수도 똑같
정수에서와 똑같은 성질을 가짐

#### 유클리드 호제법 (Euclidean algorithm)
맨날까먹음
A > B인 임의의 자연수 A, B가 있을 때, A = BQ + R로 몫과 나머지를 분리하면
gcd{A, B} = gcd{B, R} 임이 성립한다는 것

이를 확장한 Extended Euclidian Algorithm은 다음과 같다
as + bt=gcd{a,b} 인 정수쌍 s, t가 존재함
모듈러 연산의 역원을 구하는데 우려먹힌다.

#### 기수법
양의 정수 N_p = a_n p^n + a_n-1 p^n-1 + ... + a_1 p + a_0
양의 소수 N_p = a_1/p + a_2/p^2 + ... + a_n/p^n
{% endcapture %}

{% capture context2 %}
#### Euclidean algorithm으로 gcd 찾기
r0←a,r1←b
r_i+1=r_i−1−q_i r_i,  q_i=[r_i−1/r_i]

만약 r_i+1=0 이라면 r_i 가 바로 gcd(a,b) 이다.

#### Euclidean algorithm 증명
A=Ga, B=Gb (a, b 는 서로소) 를 A=BQ+R에 대입해보면
Ga=Gb Q + R, R=G(a-Qb)
이제 b와 a-Qb가 서로소임을 보이면 되는데, b=mk, a-bQ=mk'으로 두자(k, k'는 서로소)
a=bQ+mk'=m(kQ+k')이므로 m은 a, b의 공약수인데, 서로소이므로 1임
따라서 m=1이 되며 b와 a-Qb는 서로소가 되서 gcd{B, R}=G가 되어버림

#### Extended Euclidean algorithm 증명
r0←a,r1←b
초기값들을 넣으면
as_i+bt_i=r_i   for i=0,1
이제 i>1일 때 참이라고 가정하고 수학적 귀납법을 쓰면

ri+1=ri−1−riqi=(asi−1+bti−1)−(asi+bti)qi=a(si−1−siqi)+b(ti−1−tiqi)=asi+1+bti+1

따라서 ri+1=0 일 때 asi+bti=ri 는 as+bt=gcd(a,b) 가 된다.

https://codeonwort.tistory.com/295 참조

{% endcapture %}
{% include blocks.html context1=context1 context2=context2 topic="" %}

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

### 유리수, 무리수, 복소수
할말없음

### 이차방정식
ax^2 + bx + c = 0 => x = (-b +- root(b^2-4ac))/2a
ax^2 + 2bx + c = 0 => x = (-b +- root(b^2-ac))/a
D(Determinant) = B^2 -4ac
가끔씩 가물가물해서 빡친다

