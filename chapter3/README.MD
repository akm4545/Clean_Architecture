# **패러다임 개요**  
# **구조적 프로그래밍**  
최초로 적용된 패러다임(하지만 최초로 만들어진 패러다임은 아닌)은 구조적 프로그래밍으로 1968년 에츠허르 비버 데이크스트라가 발견했다. 데이크스트라는 
무분별한 점프(goto 문장)는 프로그램 구조에 해롭다는 사실을 제시했다. 데이크스트라는 이러한 점프들을 if/then/else와 do/while/until과 같이 더 익숙한 
구조로 대체했다.  
  
구조적 프로그래밍 패러다임은 아래와 같이 요약할 수 있다.  
  
- 구조적 프로그래밍은 제어흐름의 직접적인 전환에 대해 규칙을 부과한다.  
  
# **객체 지향 프로그래밍**  
두 번째로 도입된 패러다임은 구조적 프로그래밍보다 사실 2년 앞선 1966년 올레 요한 달과 크리스텐 니가드에 의해 등장했다. 이들은 알골(ALGOL) 언어의 
함수 호출 스택 프레임(stack frame)을 힙(heap)으로 옮기면 함수 호출이 반환된 이후에도 함수에서 선언된 지역 변수가 오랫동안 유지될 수 있음을 발견했다. 
바로 이러한 함수가 클래스의 생성자가 되었고 지역 변수는 인스턴스 변수 그리고 중첩 함수는 메서드가 되었다. 함수 포인터를 특정 규칙에 따라 사용하는 
과정을 통해 필연적으로 다형성이 등장하게 되었다.  
  
객체 지향 프로그래밍 패러다임은 아래와 같이 요약할 수 있다.  
  
- 객체 지향 프로그래밍은 제어흐름의 간접적인 전환에 대해 규칙을 부과한다.  
  
# **함수형 프로그래밍**  
세 번째 패러다임은 최근에 들어서야 겨우 도입되기 시작했지만 세 패러다임 중 가장 먼저 만들어졌다. 사실 함수형 프로그래밍은 컴퓨터 프로그래밍 자체보다 
먼저 등장했다. 알론조 처치는 앨런 튜링도 똑같이 흥미를 느꼈던 어떤 수학적 문제를 해결하는 과정에서 람다(lambda) 계산법을 발명했는데 함수형 프로그래밍은 
이러한 연구 결과에 직접적인 영향을 받아 만들어졌다. 1958년에 존 매카시가 만든 LISP 언어의 근간이 되는 개념이 바로 람다 계산법이다. 람다 계산법의 
기초가 되는 개념은 불변성(immutability)으로 심볼(symbol)의 값이 변경되지 않는다는 개념이다. 이는 함수형 언어에는 할당문이 전혀 없다는 뜻이기도 하다. 
사실 대다수의 함수형 언어가 변수 값을 변경할 수 있는 방법을 제공하기는 하지만 굉장히 까다로운 조건 아래에서만 가능하다.  
  
함수형 프로그래밍 패러다임은 아래와 같이 요약할 수 있다.  
  
- 함수형 프로그래밍은 할당문에 대해 규칙을 부과한다.  
  
# **생각할 거리**  
각 패러다임은 프로그래머에게서 권한을 박탈한다. 어느 패러다임도 새로운 권한을 부여하지 않는다. 각 패러다임은 부정적인 의도를 가지는 일종의 추가적인 
규칙을 부과한다. 즉 패러다임은 무엇을 해야 할지 말하기보다는 무엇을 해서는 안 되는지를 말해준다.  
  
이러한 논의를 바라보는 또 다른 방법은 각 패러다임이 우리에게서 무언가를 빼앗는다는 사실을 인지하는 것이다. 세 가지 패러다임 각각은 우리에게서 goto문, 
함수 포인터, 할당문을 앗아간다.  
  
앞으로 가져갈 수 있는것은 아마 없을 것이다. 따라서 프로그래밍 패러다임은 앞으로도 딱 세 가지밖에 없을 것이다. 최소한 부정적인 의도를 가진 패러다임으로는 
이 세 가지가 전부일 것이다. 이 밖에 다른 패러다임이 없다는 또 다른 증거로는 이들 패러다임이 1958년부터 1968년에 걸친 10년 동안 모두 만들어졌다는 
사실이다. 이후로 수십 년이 지났지만 새롭게 등장한 패러다임은 전혀 없다.  
  
# **결론**  
패러다임의 역사로부터 얻을 수 있는 이러한 교훈은 아키텍처와 모두 다 관계가 있다. 우리는 아키텍처 경계를 넘나들기 위한 메커니즘으로 다형성을 이용한다. 
우리는 함수형 프로그래밍을 이용하여 데이터의 위치와 접근 방법에 대해 규칙을 부과한다. 우리는 모듈의 기반 알고리즘으로 구조적 프로그래밍을 사용한다.  
  
세 가지 패러다임과 아키텍처의 세 가지 큰 관심사(함수, 컴포넌트 분리, 데이터 관리)가 어떻게 서로 연관되는지에 주목하자.