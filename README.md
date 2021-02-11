# 스프링 핵심 원리 - 기본편
인프렁 강좌 '스프링 핵심 원리-기본편'(김영한)을 수강하며 정리한 내용들입니다.

---
---

## 객체 지향 설계와 스프링

---

### 이야기 - 자바 진영의 추운 겨울과 스프링의 탄생
<BR>

스프링 역사
- 2002년 로드 존슨 책 출간
- EJB의 문제점 지적
- BeanFactory, ApllicationContext, POJO, 제어의 역전, 의존관계 주입

---

### 스프링이란?

- 필수
  - 스프링 프레임워크
  - 스프링 부트

- 선택
  - 스프링 데이터 : 기본적인 CRUD는 어떤 데이터베이스든 비슷한데, 이런걸 편리하게 사용할 수 있도록 도와주는 것이 '스프링 데이터'라는 기술이다. 그 중 많이 사용하는 것이 '스프링 데이터 JPA'를 많이 사용함.
  - 스프링 세션 : 세션 기능을 편리하게 사용할 수 있도록 도와줌.
  - 스프링 시큐리티 : 보안과 관련
  - 스프링 Rest Docs : API문서랑 test를 편리하게 엮어서 API문서화를 편리하게 해줌.
  - 스프링 배치 : 배치처리(1000만건 업데이트를 한번에 하는게 아닌 나누어서 업데이트하는 느낌)에 특화된 기술
  - 스프링 클라우드 : 클라우드에 특화된 기술

- 스프링 프레임워크
  - 핵심 기술 : 스프링 DI 컨테이너, AOP, 이벤트, 기타
  - 웹 기술 : 스프링 MVC, 스프링 WebFlux
  - 데이터 접근 기술 : 트랜잭션, JDBC, ORM 지원, XML 지원
  - 기술 통합 : 캐시, 이메일, 원격접근, 스케쥴링
  - 테스트 : 스프링 기반 테스트 지원
  - 언어 : 코틀린, 자바
  - 최근에는 스프링 부트를 통해서 스프링 프레임워크의 기술들을 편리하게 사용.

- 스프링 부트
  - <strong>스프링을 편리하게 사용할 수 있도록 지원, 최근에는 기본으로 사용</strong>
  - 단독으로 실행할 수 있는 스프링 애플리케이션을 쉽게 생셩
  - Tomcat 같은 웹 서버를 내장해서 별도의 웹 서버를 설치하지 않아도 됨.
  - 손쉬운 빌드 구성을 위한 starter 종속성 제공
  - 스프링과 3rd parth(외부) 라이브러리 자동 구성
    - 과거에는 버전 통일이 힘들었었다. 지금은 외부 라이브러리 버전에 대해서는 고민X
  - 메트릭, 상태 확인, 외부 구성 같은 프로덕션 준비 기능 제공
    - 운영환경에서 모니터링은 중요. 이런 부분을 스프링부트가 기본적으로 제공해줌.
  - 관례에 의한 간결한 설정
    - 예전에는 스프링 프레임워크 설정이 힘들었지만, 스프링부트가 이를 편리하게 해줌.

- 스프링 단어?
  - 스프링이라는 단어는 문맥에 따라 다르게 사용된다.
    - 스프링 DI 컨테이너 기술
    - 스프링 프레임워크
    - 스프링 부트, 스프링 프레임워크 등을 모두 포함한 스프링 생태계

- 스프링의 핵심 개념, 컨셉
  - 스프링은 자바 언어 기반의 프레임워크
  - 자바 언어의 가장 큰 특징 - <strong>객체 지향 언어</strong>
  - 스프링은 객체 지향 언어가 가진 강력한 특징을 살려내는 프레임워크
  - 스프링은 <strong>좋은 객체 지향</strong> 애플리케이션을 개발할 수 있게 도와주는 프레임워크

---

### 좋은 객체 지향 프로그래밍?

- 객체 지향 특징
  - 추상화
  - 캡슐화
  - 상속
  - <strong>다형성</strong>

- 객체 지향 프로그래밍
  - 객체 지향 프로그래밍은 프로그램을 명령어의 목록으로 보는 시각에서 벗어나 여러 개의 독립된 단위, 즉 <strong>"객체"</strong>들의 <strong>모임</strong>으로 파악하고자 하는 것이다. 각각의 <strong>객체</strong>는 메시지를 주고받고, 데이터를 처리할 수 있다.<strong>(협력)</strong>
  - 객체 지향 프로그래밍은 프로그램을 <strong>유연</strong>하고 <strong>변경</strong>이 용이하게 만들기 때문에 대규모 소프트웨어 개발에 많이 사용된다.

- 유연하고, 변경이 용이?
  - 레고 블럭 조립하듯이
  - 키보드, 마우스 갈아 끼우듯이
  - 컴퓨터 부품 갈아 끼우듯이
  - 컴포넌트를 쉽게 유연하게 변경하면서 개발할 수 있는 방법
  > 다형성(Polymorphism)

- 다형성의 실세계 비유
  - 실세계와 객체 지향을 1:1로 매칭은 잘 안됨.
  - 그래도 비유하면 이해하기 좋음
  - <strong>역할</strong>과 <strong>구현</strong>으로 세상을 구분
    - 역할 : 인터페이스
    - 구현 : 인터페이스를 구현한 객체

- 운전자 - 자동차 예시
  - ![car](./readme_img/car.JPG)
  - 자동차 역할을 3개의 다른 자동차로 구현
  - 만약 운전자가 K3를 타다가 다른 자동차인 아반떼로 차를 바꿔도 당연히 운전을 할 수 있음.
    - 왜냐하면 자동차 역할에 대한 구현만 바뀌었을 뿐이기 때문이다.
  - <strong>그래서 자동차가 바뀌어도 운전자한테 영향을 주지 않는다.</strong>
    > 유연하고 변경이 용이하다.
  - 운전자는 자동차 역할에 대해서는 의존하고 있다.
  - 이렇게 자동차 역할를 만들고 자동차 구현을 분리한 이유는 '운전자'(client)를 위해서 이렇게 함.
    - client는 자동차의 내부 구조를 몰라도 됨.
    - 자동차 구현이 바뀌어도 client에게는 영향이 없음.
  - client에 영향을 주지않고 새로운 기능을 제공할 수 있다.
  - 즉, 새로운 자동차가 나와도 client는 새로운 것을 안배워도 됨.

- 공연 무대 예시
  - ![show](./readme_img/show.JPG)
  - 배우는 대체가 가능하다.
  - 역할과 구현으로 나눔 = 변경가능한 대체 가능성이 생김
    - 유연하고 변경이 용이하다라는 뜻

- 다형성의 실세계 비유 예시
  - 운전자 - 자동차
  - 공연 무대
  - 키보드, 마우스, 세상의 표준 인터페이스들
  - 정렬 알고리즘(정렬만 되면 더 좋은 기능의 알고리즘으로 교체)
  - 할인 정책 로직

- <strong>역할과 구현을 분리</strong>
  - <strong>역할</strong>과 구현으로 구분하면 세상이 <strong>단순</strong>해지고, <strong>유연</strong>해지며 <strong>변경</strong>도 편리
  - 장점
    - <strong>클라이언트</strong>는 대상의 역할(인터페이스)만 알면 된다.
    - <strong>클라이언트는</strong> 구현 대상의 <strong>내부 구조를 몰라도</strong> 된다.
      - ex> 운전자 - 자동차
    - <strong>클라이언트</strong>는 구현 대상의 <strong>내부 구조가 변경</strong>되어도 영향을 받지 않는다.
      - 기름차에서 전기차로 바뀌어도 운전자는 운전 가능
    - <strong>클라이언트</strong>는 구현 <strong>대상 자체를 변경</strong>해도 영향을 받지 않는다.
      - K3에서 테슬라로 바꿔도 운전자는 영향을 받지 않음.

- 역할과 구현을 분리_자바 언어
  - 자바 언어의 다형성을 활용
    - 역할 = 인터페이스
    - 구현 = 인터페이스를 구현한 클래스, 구현 객체
  - 객체를 설계할 때 <strong>역할</strong>과 <strong>구현</strong>을 명확히 분리
  - 객체 설계시 역할(인터페이스)을 먼저 부여하고, 그 역할을 수행하는 구현 객체 만들기

- 객체의 협력이라는 관계부터 생각
  - 혼자 있는 객체는 없다
  - 클라이언트 : <strong>요청</strong>, 서버 : <strong>응답</strong>
  - 수 많은 객체 클라이언트와 객체 서버는 서로 협력 관계를 가진다.
  - ![client_server](./readme_img/client_server.JPG)

- 자바 언어의 다형성
  - ![overriding](./readme_img/overriding.JPG)
    - MemberService가 save()를 호출하면, interface의 MemberRepository의 save()를 호출하면, 실제로는 밑의 구현체들의 save()가 호출이된다.(예를 들면 현재 MemoryMemberRepository가 들어가있으면 해당 save()가 호출)
  - <strong>오버라이딩</strong>을 떠올려보자
  - 오버라이딩은 자바 기본 문법
  - 오버라이딩 된 메서드가 실행
  - 다형성으로 인터페이스를 구현한 객체를 실행 시점에 유연하게 변경할 수 있다.
  - 물론 클래스 상속 관계도 다형성, 오버라이딩 적용가능
  - ![client](./readme_img/client.JPG)
    - client(MemberService)는 MemberRepository에 의존한다.
      - 의존한다 == 내가 쟤를 알고 있다.
  - ![overriding](./readme_img/overriding.JPG)
    - MemberRepository에 구현체(MemoryMemberRepository, JdbcMemberRepository)들을 할당할 수 있다.
      - ![interface](./readme_img/interface.JPG)

    - 코드 예시
        <details>
        <summary>MemoryMemberRepository</summary>

            ```java
            public class MemberService{
                private MemberRepository memberRepository = new MemoryMemberRepository();
            }
            ```

        </details> 

        <details>
        <summary>JdbcMemberRepository</summary>

            ```java
            public class MemberService{
                //private MemberRepository memberRepository = new MemoryMemberRepository();
                private MemberRepository memberRepository = new JdbcMemberRepository();
            }
            ```

        </details> 

    - 어떤 구현체를 넣냐에 따라 다름
      - ![who](./readme_img/who.JPG)


- <strong>다형성의 본질</strong>
  - 인터페이스를 구현한 객체 인스턴스를 <strong>실행 시점</strong>에 유연하게 <strong>변경</strong>할 수 있다.
  - 다형성의 본질을 이해하려면 <strong>협력</strong>이라는 객체사이의 관계에서 시작해야함.
  - <strong>클라이언트를 변경하지 않고, 서버의 구현 기능을 유연하게 변경할 수 있다.</strong>

- 역할과 구현을 분리_정리
  - 실세계의 역할과 구현이라는 편리한 컨셉을 다형성을 통해 객체 세상으로 가져올 수 있음
  - 유연하고, 변경이 용이
  - 확장 가능한 설계
  - 클라이언트에 영향을 주지 않는 변경이 가능
  - 인터페이스를 안정적으로 잘 설계하는 것이 중요

- 역할과 구현을 분리_한계
  - 역할(인터페이스) 자체가 변하면, 클라이언트, 서버 모두에 큰 변경이 발생한다.
    - 자동차를 비행기로 변경해야 한다면?
    - 대본 자체가 변경된다면?
    - USB 인터페이스가 변경된다면?
  - 인터페이스를 안정적으로 잘 설계하는 것이 중요


- 스프링과 객체 지향
  - 다형성이 가장 중요!
  - 스프링은 다형성을 극대화해서 이용할 수 있게 도와준다.
  - 스프링에서 이야기하는 제어의 역전(IoC), 의존관계 주입(DI)은 다형성을 활용해서 역할과 구현을 편리하게 다룰 수 있도록 지원한다.
  - 스프링을 사용하면 마치 레고 블럭 조립하듯이! 공연 무대의 배우를 선택하듯이! 구현을 편리하게 변경할 수 있다.

---

### 좋은 객체 지형 설계의 5가지 원칙(SOLID)

- SOLID
    > 클린코드로 유명한 로버트 마틴이 좋은 객체 지향 설계의 5가지 원칙을 정리
  - SRP : 단일 책임 원칙(Single Responsibility Principle)
  - OCP : 개방-폐쇄 원칙(Open/Closed Principle)
  - LSP : 리스코프 치환 원칙(Liskov Substitution Principle)
  - ISP : 인터페이스 분리 원칙(Interface Segregation Principle)
  - DIP : 의존관계 역전 원칙(Dependency Inversion Principle)

- SRP 단일 책임 원칙
  - 한 클래스는 하나의 책임만 가져야 한다.
  - 하나의 책임이라는 것은 모호하다.
    - 클 수 있고, 작을 수 있다.
    - 문맥과 상황에 따라 다르다.
  - <strong>중요한 기준은 변경</strong>이다. 변경이 있을 때 파급 효과가 적으면 단일 책임 원칙을 잘 따른 것
  - EX> UI 변경, 객체의 생성과 사용을 분리

- OCP 개방-폐쇄 원칙(중요)
  - 소프트웨어 요소는 <strong>확장에는 열려</strong> 있으나 <strong>변경에는 닫혀</strong> 있어야 한다.
    - 코드의 변경없이 기능을 추가할 수 있다??
- <strong>다형성</strong>을 활용해보자
- 인터페이스를 구현한 새로운 클래스를 하나 만들어서 새로운 기능을 구현
- 지금까지 배운 역할과 구현의 분리를 생각해보자.
    - 코드 예시
        <details>
        <summary>MemoryMemberRepository</summary>

            ```java
            public class MemberService{
                private MemberRepository memberRepository = new MemoryMemberRepository();
            }
            ```

        </details> 

        <details>
        <summary>JdbcMemberRepository</summary>

            ```java
            public class MemberService{
                //private MemberRepository memberRepository = new MemoryMemberRepository();
                private MemberRepository memberRepository = new JdbcMemberRepository();
            }
            ```

        </details> 

    - MemberService를 보면,
      - 1번코드) field에 MemberRepository 인터페이스를 알고 있고 new 해서 MemoryMemberRepository를 넣음.
      - 2번코드) field에 MemberRepository 인터페이스를 알고 있고 new 해서 JdbcMemberRepository를 넣음.
    - 위 코드를 보면 JDBC로 바꿀려면 결국 코드를 변경해야한다.

- OCP 개방-폐쇄 원칙_문제점
  - MemberService 클라이언트가 구현 클래스를 직접 선택
    - 
    ```java
    MemberRepository m = new MemoryMemberRepository();//기존코드
    ```
    - 
    ```java
    MemberRepository m = new JdbcMemberRepository();//변경 코드
    ```
  - <strong>구현 객체를 변경하려면 클라이언트 코드를 변경해야 한다.</strong>
  - <strong>분명 다형성을 사용했지만 OCP 원칙을 지킬 수 없다.</strong>
  - 이 문제를 어떻게 해결해야 하나?
  - 객체를 생성하고, 연관관계를 맺어주는 별도의 조립, 설정자가 필요하다.
    - 스프링 컨테이너가 해줌.

- LSP 리스코프 치환 원칙
  - 프로그램의 객체는 프로그램의 정확성을 깨뜨리지 않으면서 하위 타입의 인스턴스로 바꿀 수 있어야 한다.
    - EX> 자동차 인터페이스의 엑셀은 앞으로 가라는 기능이다. 그러나, 뒤로 가게 구현하면 LSP 위반, 느리더라도 앞으로 가야함.(그래도 컴파일 오류가 나지 않고 성공을 하지만 안됨. 기능적으로 보장을 해줘야함.)
  - 다형성에서 하위 클래스는 인터페이스 규약을 다 지켜야 한다는 것, 다형성을 지원하기 위한 원칙, 인터페이스를 구현한 구현체는 믿고 사용하려면, 이 원칙이 필요하다.
  - 단순히 컴파일에 성공하는 것을 넘어서는 이야기
  
- ISP 인터페이스 분리 원칙
  - 특정 클라이언트를 위한 인터페이스 여러 개가 범용 인터페이스 하나보다 낫다.
  - 자동차 인터페이스 -> 운전 인터페이스, 정비 인터페이스로 분리.(자동차 인터페이스가 너무 크니까 분리, 이는 사용자 클라이언트를 운전자 클라이언트와 정비사 클라이언트로 분리할 수 있다.)
  - 사용자 클라이언트 -> 운전자 클라이언트, 정비사 클라이언트로 분리.
  - 분리하면 정비 인터페이스 자체가 변해도 운전자 클라이언트에 영향을 주지 않음.
  - 인터페이스가 명확해지고, 대체 가능성이 높아진다.


- <strong>DIP 의존관계 역전 원칙(중요)</strong>
  - 프로그래머는 "추상화에 의존해야지, 구체화에 의존하면 안된다." 의존성 주입은 이 원칙을 따르는 방법 중 하나다.
  - 쉽게 이야기해서 구현 클래스에 의존하지 말고, 인터페이스에 의존하라는 뜻.(즉, 클라이언트 코드가 구현 클래스를 바라보지 말고 인터페이스만 바라보게 하기, MemberService가 MemberRepository interface만 바라보게하고, MemoryMemberRepository나 JdbcMemberRepository에 대해서는 몰라야한다.)
  - 앞에서 이야기한 <strong>역할(Role)에 의존하게 해야 한다는 것과 같다.</strong> 객체 세상도 클라이언트가 인터페이스에 의존해야 유연하게 구현체를 변경할 수 있다! 구현체에 의존하게 되면 변경이 아주 어려워진다.
  - 그런데 OCP에서 설명한 MemberService는 인터페이스에 의존하지만, 구현 클래스도 동시에 의존한다.
  - MemberService 클라이언트가 구현 클래스를 직접 선택
    ```java
    MemberRepository m = new MemoryMemberRepository();
    ```
  - <strong>DIP 위반</strong>

- 정리
  - 객체 지향의 핵심은 다형성
  - 다형성 만으로는 쉽게 부품을 갈아 끼우듯이 개발할 수 없다.
  - 다형성 만으로는 구현 객체를 변경할 땓 클라이언트 코드도 함께 변경된다.
  - <strong>다형성 만으로는 OCP, DIP를 지킬 수 없다.</strong>
  - 뭔가 더 필요함.


---

### 객체 지향 설계와 스프링

- 스프링 이야기에 왜 객체 지향 이야기가 나오는가?
  - <strong>스프링은 다음 기술로 다형성 + OCP, DIP를 가능하게 지원</strong>
    - DI(Dependency Injection): 의존관계, 의존성 주입
    - DI 컨테이너 제공
      - 자바 객체들을 어떤 컨테이너안에 넣어두고 이 안에서 서로 의존관계를 연결해주고 주입해주는 기능들을 제공해줌.
  - <strong>클라이언트 코드의 변경 없이 기능 확장</strong>
  - 쉽게 부품을 교체하듯이 개발.

- 스프링이 없던 시절
  - 옛날 어떤 개발자가 좋은 객체 지향 개발을 하려고 OCP, DIP 원칙을 지키면서 개발을 해보니, 너무 할일이 많았다. 배보다 배꼽이 크다. 그래서 프레임워크로 만들어버림.
  - 순수하게 자바로 OCP, DIP 원칙들을 지키면서 개발을 해보면, 결국 스프링 프레임워크를 만들게 된다,(더 정확히는 DI 컨테이너)
  - DI 개념은 말로 설명해도 이해가 잘 안됨 -> 코드로 짜봐야 필요성을 알게된다!

- 정리
  - 모든 설계에 <strong>역할</strong>과 <strong>구현</strong>을 분리하자.
  - 자동차, 공연의 예를 떠올려보자.
  - 애플리케이션 설계도 공연을 설계 하듯이 배역만 만들어주고, 배우는 언제든지 <strong>유연</strong>하게 <strong>변경</strong>할 수 있도록 만드는 것이 좋은 객체 지향 설계다.
  - 이상적으로는 모든 설계에 인터페이스를 부여하자.

- 정리_실무 고민
  - 하지만 인터페이스를 도입하면 추상화라는 비용이 발생한다.
    - 단순하게는, 인터페이스 클래스와 구현 클래스를 만들어야 함.
    - 추상화가 되버리면 개발자가 코드를 한번 더 열어봐야함.(인터페이스도 보고, 구현체도 보고)
  - 기능을 확장할 가능성이 없다면, 구현체 클래스를 직접 사용하고, 향후 꼭 필요할 때 리팩터링해서 인터페이스를 도입하는 것도 방법이다.

- 책추천
  - 객체지향 책 추천 : 객체지향의 사실과 오해
  - 스프링 책 추천 : 토비의 스프링(필수)
  - JPA 책 추천 : 자바 ORM 표준 JPA 프로그래밍

