
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
명제는 참/거짓을 내릴 수 있는 문장이며, 조건은 변수 $$ x $$에 값을 대입하면 명제가 되는 문장.
p이면 q이다: p -> q, p->q가 참이면 p => q, 진리집합 P, Q에 대해 P Q이면 p=>q 

{% capture context1 %}
#### 조건
조건에 포함된 변수 x는 U\neq 공집합 을 정의역으로 함. 전체집합 U에서의 조건 p(x)를 간단히 조건 p라고 표기함.
U의 원소 a를 대입한 p(a)가 참인 명제라면, 명제 p(a)가 성립한다, a는 조건 p(x)를 만족한다 라고 함.

#### 부정
명제 p 혹은 조건 p(x)에 대해 'p(x)가 아니다' 를 p(x)의 부정이라 하고, ~p(x)로 표기함.
~(p or q) <=> (~p and ~q), ~(p and q) <=> (~p or ~q)
~(모든 x, p(x)) <=> (어떤 x, ~p(x)), ~(어떤 x, p(x)) <=> (모든 x, ~p(x))

#### 진리집합
p(x)를 만족하는 x 전체의 집합 P를 조건 p(x)의 진리집합이라고 한다.
P={x|x in U, p(x)}. 표기시 전체집합 U를 씹으려는 경향이 강하므로 P={x|p(x)}로도 표기.

#### 조건과 집합
집합 P, Q를 조건 p, q의 진리집합이라고 둘 때,
P Q <=> (p => q), P / Q <=> (p =/> q), 
p or q <=> P U Q, p and q <=> P cup Q, ~p <=> P^c
{% endcapture %}

{% capture context2 %}
두 조건 p, q를 p -> q 꼴로 연결하면 명제가 되어버림.
4의 약수는 8의 약수이다 를 풀어서 x가 4의 약수이면 x는 8의 약수이다 로 표현가능.
P in Q => x in P 이면 x in Q => p 이면 q
~(p or q) => (PUQ)^c => P^c cup Q^c => ~p and ~q
~(모든 x에 대하여 p(x)이다) => ~(p(x1) and p(x2) and ... and p(xn)) => ~p(x1) or ~p(x2) or ... or ~p(xn) => 어떤 x에 대하여 ~p(x)
비슷한 방법으로 모두 증명 가능
{% endcapture %}

{% include blocks.html context1=context1 context2=context2 topic="명제" %}

#### 