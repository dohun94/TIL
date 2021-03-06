# 프레임워크 VS 라이브러리  

결론적으로, 프레임워크와 라이브러리의 차이는 코드가 수동적으로 사용되냐, 능동적으로 사용되냐 차이이다.  

**프레임워크란?**  
>프로그래밍에서 특정 운영 사례를 위한 응용프로그램 표준 구조를 구현하는 클래스와 라이브러의 모임이다.
>\- 위키백과  

**라이브러리란?**  
>소프트웨어를 만들 때 쓰이는 클래스나 서브 루틴들의 모임을 가리키는 말이다.
>\- 위키백과  

**제어의 역전?**  
라이브러리를 사용하는 애플리케이션 코드는 능동적으로 실행되다가 라이브러리의 기능이 필요하면 라이브러리를 호출해서 사용한다.  

반면, 프레임워크는 거꾸로 애플리케이션 코드가 프레임워크에 의해 사용된다. 보통 프레임워크 위에 개발한 클래스를 등록해두고, 프레임워크가 흐름을 주도하는 중에 개발자가 만든 애플리케이션 코드를 사용하도록 하는 방식이다.

출처 : http://asfirstalways.tistory.com/25

https://kldp.org/node/124237 에서 참조한 글  

일단 모든 소스코드든 라이브러리든 메모리에 들어가는 정보는, 컴파일러나 인터프리터에게는 호출가능한 모듈일 뿐입니다.  
이런 물리적인 계층을 보지말고, 그 위의 논리적인 계층을 봐야합니다.  

라이브러리는 톱, 망치, 삽같은 연장입니다.  
사람이 들고 썰고, 바꿔들고 내려치고, 다시 바꿔들고 땅을 파는 겁니다.  

프레임워크는 차, 비행기, 배같은 탈것입니다.  
사람이 타서 엔진 켜고, 기어 넣고, 핸들 돌리고, 운전하거나, 조종하거나 해야합니다.  

도구를 쓸 때, 급하면 썰어야 할 곳에 망치를 쳐도 됩니다. 땅 파야할 때 톱으로 땅을 긁어내도 됩니다.  
사람은 도구를 선택하는 입장이기 때문에, 어떤 도구를 사용하든 원하는 것을 만들어낼 수 만 있으면 됩니다.  

반면에, 탈것은 정해진 곳으로만 다녀야 합니다. 차를 타고 하늘을 날거나, 배를 타고 땅으로 갈 수는 없습니다.  
하지만, 그 목적에 맞게 만들어져 있기 때문에, 톱이나 망치를 들고 먼저 탈것을 만들어야할 필요가 없습니다.  
그저 정해진 규칙에 맞춰서 엔진, 기어, 핸들만 잘 돌리면 됩니다.  

라이브러리와는 달리 프레임워크는 이미 프로그래밍할 규칙이 정해져 있습니다.  
예를 들어, 설정파일로 사용되는 XML에 어떤 태그를 써야하며, 어떤 함수를 추가적으로 작성해야하고,
소스 파일을 어느 위치에 넣어야하며, DB와 연동하기 위해 무엇을 써넣어야 하는지 정해져 있습니다.  
보통 이런 대부분의 작업은 프레임워크가 하고자 하는 일에 비하면 아주 작은 일이며, 사람은 극히 일부분만 조정함으로써 목적을 달성할 수 있습니다.  

만약 프레임워크가 담당하는 부분이 내가 하고자 하는 목적과 다를 경우에는 어떻게 할까요?  
그럼 그냥 프레임워크를 잘못쓴겁니다.  
더 목적에 가까운 프레임워크를 찾아보면 대부분 있을겁니다.  
없거나 구하기 힘들다면, 비슷한 프레임워크를 라이브러리 단계에서 변경해서 다른 프레임워크로 만들면 됩니다.  
차를 튜닝한다음, 차를 다시 운전하면 된다는 말이지요.  
