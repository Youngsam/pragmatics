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
* 귀납추론은 경험 데이터를 일반화하는 방식의 추론을 말한다.
  * 까마귀 관찰 => 까마귀는 모두 까맣다.
* 귀추는 관찰에 근거해 가설들을 만들고 가장 그럴듯한 가설을 선택하는 방식의 추론을 가리킨다.
  * "도로가 젖었다"(관찰) & "비가 내리면 도로가 젖는다"(지식) => "비가 내렸었다"(판단)
