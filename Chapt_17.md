# Chapter 17. Computational Pragmatics 
by Harry Bunt

## 17.1 General and Computational Pragmatics
* 계산 화용론은 발화의 언어적 속성과 발화가 사용된 맥락의 측면(aspects)간의 관계를 말뭉치 데이터, 맥락모형, 알고리즘과 같은 계산적 방법을 통해 연구하는 분야로, 맥락-의존적 발화생성과 해석을 중요하게 다룬다.
* 맥락과 언어형식과의 관계는 분명하다.
  * 전제(presupposition)
      <br/>명사구의 한정사의 사용은 화자가 청자와 공유한다고 믿는 가정에 대한 정보를 드러낸다.
   * Given-new structuring
      <br/>문장구조를 통해 화자는 청자가 이미 알고 있다고 생각하는 바와 모른다고 생각하는 것을 구분하여 제시하려 한다.
   * Topic-focus mapping
      <br/>어순을 통해 화자는 청자가 주목해야 할 내용을 표시한다.
* 대화에서 발화의 맥락이란 이전의 내용과 상호작용에 의해 구성되지만, 또한 사회적 예의나 인지적 맥락에 의해서도 영향을 받는다.
* 사회적 예의나 인지적 맥락과 같은 지각적 정보는 본질적으로 다이내믹하다. 대화가 진행되면서 그 정보는 변화하고 대화의 결과가 된다. 따라서 대화맥락은 소통의 효과와 함께 연속적으로 변화한다.
* 대형 말뭉치 자료가 소프트웨어를 통해 분석이 가능해지면서 화용론 연구는 보다 체계적이고 경험적 분석이 가능하게 되었다. '대화행위 이론'이 하나의 예인데, 현대 대화행위 이론은 전통적인 화행이론보다 더 많은 action type과 더 다양한 소통행위 개념들을 갖고 잇다.
* 대화함축과 간접화행은 청자의 추론능력에 의존하는데, 이는 듣는 이가 맥락정보와 발화정보를 종합하여 화자가 의도한 의미를 파악할 수 있다고 가정한다는 것을 뜻한다.
* 맥락기반 추론은(context-based inference) 대화의 발화를 이해하기 위해선 반드시 필요하다. 가장 간단한 예는 '예' 혹은 '아니오'로, 이런 응답은 앞선 발화의 의미를 이해하지 못한다면 이해될 수 없는 발화이다.
* 에제 1: Declarative question
  <br/> C: What departure times do you have for flights to Munich early in the morning?
  <br/> I: I have Lufthansa at 07:15, KLM at 07:25, again KLM at 07:50, and another Lufthansa at 08:20
  <br/> C: **and that's on Saturday too**
  <br/> I: and that's on Saturday too
* 예제 1에서와 같은 형태의 질문은 information-seeking dialogue 말뭉치에서 20%의 적지 않은 비중을 차지한다.(Beun, 1989) 이 예제는 대화에서 일어나는 발화의 해석은 추리(inferencing)을 요한다는 것을 보여준다.
* 추리란 예외처리가 아니라 규칙에 의한 것이며, 해석과 추리는 서로 맞물리는 과정이다.

## 17.2 Inferencing in Computational Pragmatics
* 추론의 3가지 형태
  * Deductive inference
  * Inductive inference
  * Abductive inference
* 연역추론은 주어진 전제와 사실들을 통해 새로운 판단을 논리적으로 도출하는 방식의 판단을 말한다.
  * 까마귀에는 '검다'는 의미가 있다 & 대상의 이름은 그 속성을 반영한다 => 까마귀는 모두 검은색이다
* 귀납추론은 경험 데이터를 일반화하는 방식의 추론을 말한다.
  * 까마귀 관찰 => 까마귀는 모두 검은색이다
* 귀추는 관찰에 근거해 가설들을 만들고 가장 그럴듯한 가설을 선택하는 방식의 추론을 가리킨다.
  * "도로가 젖었다"(관찰) & "비가 내리면 도로가 젖는다"(지식) => "비가 내렸었다"(귀추적 판단)
* 연역추론은 과학에서는 널리 쓰이나 일상적 추론에서는 잘 쓰이지 않는다. 반면에 귀납과 귀추는 우리가 일상적으로 쓰는 직관적 방식의 추론이다.
* 귀납은 세계에 대한 모델을 구성할 때 특히 많이 쓰이고, 귀추는 관찰의 해석에 대해 중요하게 쓰인다. 특히 귀추적 판단은 대화상황의 해석에서 중요하다.
* 여기서 떠오르는 중요한 문제는 그 해석들 중 어떤 해석이 다른 해석보다 어떻게 선호되는지를 밝히는 것이다.
  * wet_street(O) <= raining(P1) or pipe_burst(P2)
* Weighted abduction (Stickel, 1988)
  * 짧은 증명은 긴 증명보다 비용이 더 적다 => 적은 비용의 증명이 보다 그럴듯한(plausible) 설명이다
  * 'Interpretation as abduction' (Hobbs, 1990b; Hobbs et al., 1993)
* 예제 (Hobbs et al., 1993)
  > (2) The Boston office called
  * 이해되어야 할 요소들
    * 정관사 'the'
    * 'Boston office'에서 'Boston'과 'office'의 관계
    * 'office'와 'making a phone call'의 환유적 관계
  * 지식기반을 이용한 해석
    <br/>(3) boston'(x) EXT office'(y) EXT NN(y, x)
    <br/>(4) office'(B1), located-in(B1, B), boston'(B)
  * 일반지식
    <br/>located-in(x, y) => NN(x, y)
* 예문 (2)의 해석은 지식기반과 일반지식의 귀추적 조합을 통해 도출될 수 있다. 만일 Boston에 위치한 다른 office들이 지식기반에 있다면, 가중치(weights) 계산을 통해 가장 그럴듯한 대안을 선택하면 된다.
* NLU 시스템에선 이와같이 특정 상황정보와 일반적 지식을 종합한 형태의 추론이 필요하다.
* Mini-TACITUS (Ovchinnikova, 2014) 시스템은 weighted abduction을 이용한 시스템으로, WordNet과 FrameNet과 같은 말뭉치 자료를 적극적으로 활용하였다.
* 계산 화용론이 필요로 하는 세 가지 도구
  * 추론을 위한 계산 알고리즘
  * 화용적 속성이 주석된 말뭉치 자료
  * 지식과 맥락에 대한 계산적 표현체계
  
## 17.3 Language as Action in Context
### 17.3.1 Speech acts and dialogue acts
* 계산 화용론에서 '대화행위'는 행위의 수행으로서의 언어사용을 모델링한다. 이것은 의사소통 행위를 모형화하고자 하는 경험기반 접근법을 취한다.(ISO 24617-2:2012)
* 대화행위 이론은 '정보-상태 갱신' 혹은 '맥락-변화' 접근방식을 취한다. 이 접근법은 대화 참여자들의 정보상태에 갱신작용을 함으로써 소통행위의 의도된 의미를 밝히고자 한다.
* "Do you know what time it is?"
 * 대화행위의 두 주요 요소: semantic content, communicative function
 * 대화행위의 소통적 기능은 위 예제의 질문이 '질문'의 기능을 하는지 아니면 '힐난'의 기능을 위한 것인지를 구분해준다. 만일 전자라면, 대화의 의미적 내용을 이용해 청자의 정보상태를 질문자가 현재시간을 모르며 그것을 알기 원한다는 정보로 갱신하게 된다. 반면 후자라면, 질문자는 현재 시간을 알고 있으며 그 정보를 요구하는 것이 아니라는 정보를 정보상태에 입력하게 된다.
