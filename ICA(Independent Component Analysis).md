## ICA(Independent Component Analysis)

rs-fMRI 데이터에서 ICA를 사용해서 개인기준, 뇌의 영역간의 기능적 연결성을 밝혀낼 수 있다. ICA는 주어지는 raw data에서 순수한 BOLD signal을 추출해낸다. 

사용되는 원리를 좀더 풀어서 말해보면, ICA를 사용해서 순수한 신호를 복원해내고, 뇌의 A와 B영역에서 유사한 '순수한' 패턴이 나타나면 해당 영역이 기능적 연결성이 있는지를 분석하는 것이다.

ICA 개념 자체를 이해하는 것은 어렵지 않다.(어렵다면 미리 죄송합니다.) 가령, 예를 들어 어떤 파티자리에 내가 갔다고 해보자. 나는 내 옆의 사람이 말하는 것을 들어야 하는데 여러가지 소리가 섞여 쉽지 않다.

이때 ICA를 사용해서 옆자리 사람이 말하는 음성만을 추출해내는 것이 바로 ICA의 목적이다.

S1(Source)는 여러가지 환경적인 요인에 의해서 X1이 되는데, 우리는 환경적인 요인을 가중치라고 하고, X1에서 가중치를 제거하여 S1를 찾아내는 것이 목적이다.

수식은 다음과 같다.