# Chapter 5. Formal Pragmatics
by Reinhard Blutner

## 15.2 Optimality-Theoretic Pragmatics
* 최적성 이론은 통합적 인지 이론으로, 기호처리 모형의 장점과, 신경망 모형을 이용하는 제약만족(constraint-based) 모형의 장점을 종합하여 취하는 것이 특징이다.(Smolensky and Legendre, 2006)
* 최적성 이론은 언어학 분야에서 음운론, 형태론, 통사론과 자연어 습득과 그 외 현상적 특징을 성공적으로 설명해왔다.
* 최적성 이론은 적합성 이론과 유사하게 언어현상에 자연주의적 관점을 취하고 있으며, 다음과 같은 급진적 화용론의 주장을 받아들인다.(Jaszczolt, 2010)
  * There is a level of logical form or semantic representation. The representations of this level do not necessarily provide truth conditions. Rather, they underspecify truth-conditional content in a number of ways. -> 진리조건이 커버하지 못하는 의미표상 수준이 존재한다.
  * There is a mechanism of enriching underspecified representations; sometimes this mechanism is called development of logical form. The result of this development is propositional content. It expresses the utterance meaning of the expression under discussion. -> 논리형식이 변환되는 기제가 존재한다.
  * There is a level of implicatures proper, understood as separate thoughts implied by the utterance. It is implicit propositional content that can be inferred from the explicit content mentioned in 2. -> 함축을 통해 처리되는 해석의 수준이 존재한다.
* 위에서 볼 수 있듯이, 최적성 이론도 논리형식이 문자적 의미와 일치된다는 전통적 입장을 거부하고 논리형식은 표현된 의미내용에 따라 명시되고 함축은 어떤 논리형식과 다른 논리형식보다 더 멀거나 가까울 수 있다는 입장을 받아들인다.

### 15.2.1 Three Variations on Grice
* 최적성 이론은 그라이스 화용론의 세 가지 변형모형(relevance theory, Levinson's (2000) theory of presumptive meaning, Neo-Gricean approach)을 모두 체계적으로 통합하는 이론이다.
* 대화함축 접근법의 두 가지 구별
  * Global (neo-Gricean) view: 문장의 일반적 의미를 처음에 파악하고 함축을 통해 적합한 대안을 고려한다.
  * Local view: 부분적으로 화용적 가설들을 적용한 다음 제약기반적 방식으로 이들을 조합한다.
* Global view는 합리적 담화해석에 적합한 반면, local view는 실시간 처리과정을 설명하는데 이점을 지닌다.
* OT는 위 두 입장의 장점을 체계적으로 통합한다.
* 적합성 이론(RT)은 *communicative principle of relevance* 에 기초하여 모든 발화는
  * 첫째, 적어도 청자의 처리 노력에 걸맞게 적합해야 하며.
  * 둘째, 화자의 현재 지식상태와 목적/선호에 맞도록 최대한 적합해야 한다.
* 위 두 가정에 기초하여, RT 이론은 발화를 처리하는 인지 시스템은 다음의 일반적 과정을 갖는다고 본다.
  1. 접근하는 순서에 따라 가능한 해석들을 테스트한다.
  2. 최적 적합도에 도달하면 처리과정을 멈춘다.
* Levinson’s (2000) theory of presumptive meaning은 RT와 유사한 측면과 유사하지 않은 측면을 동시에 활용하는 이론이다.
* 레빈슨은 의미의 세 가지 수준을 가정한다:
  * 문장 유형의 의미
  * 발화 유형의 의미
  * 발화 토큰의 의미
* 발화 수준의 의미는 그라이스의 기존 대화함축과 유사하며 다음의 세 가지 휴리스틱에 따라 처리된다.
  * Q-휴리스틱: 언급되지 않은 것은 해당되지 않는다.
  * I-휴리스틱: 단순하게 표현된 것은 전형적으로 예시된 것이다.
  * M-휴리스틱: 비정상적으로 언급된 것은 정상적이지 않은 것이다.
* 하지만 그라이스의 global view 와는 달리, presumptive meanings는 local하게 구성된다.(예를 들면, 'some'이란 단어는 Q-휴리스틱을 통해 NOT ALL 이란 디폴트 해석을 일으킨다.)
* 이와 같은 local 화용론적 자질들은 인공지능을 위한 화용론에는 중요한 요소이다.
* 신-그라이스식의 화용론은 Q-원리와 R-원리를 가정하는데, 이 둘은 서로 상충되면서 상호보완적으로(화용론적 작업분담) 작동한다고 본다.

### 15.2.2 Bidirectional OT
* 쌍방향 최적성 이론은 언어형식과 언어의미 간의 최적점을 찾는데 있어 일반적 절차를 제공한다.
* 의미-형식 쌍에 대한 쌍방향 최적성은 (1) 강한 방식과, (2) 약한 방식으로 나누어진다.
* Formalism of Bidirectional OT
  * Generator: **Gen** &#8838; **F** X **M** gives the set of all potential form-meaning pairs
  * &#12296;**GEN**, **&#8827;**&#12296;: OT-system for form-meaning paris
