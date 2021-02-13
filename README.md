# 스프링 핵심 원리 - 기본편
인프렁 강좌 '스프링 핵심 원리-기본편'(김영한)을 수강하며 정리한 내용들입니다.<br>
https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-%ED%95%B5%EC%8B%AC-%EC%9B%90%EB%A6%AC-%EA%B8%B0%EB%B3%B8%ED%8E%B8

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

### 객체 지향 설계와 Spring

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

---
---

## 스프링 핵심 원리 이해1 - 예제 만들기

이 단원에서는 순수한 Java로만 작성해볼거임.(프로젝트 환경설정을 편리하게 하려고 스프링 부트를 사용하긴 함. 그외에는 순수한 자바로만 개발)

---
---

### 프로젝트 생성

- 환경
  - Java11
  - IntelliJ
- start.spring.io에서 아래와 같이 프로젝트 생성
  - Gradle Project
  - Java
  - 2.4.2
  - Project Metadata
    - Group : hello
    - Artifact(빌드명) : core
    - Packaging : Jar
    - Java : 11
  - Dependencies : 아무것도 선택안할거임(only 자바로 작성할거라서)

- 위 설정 후 다운 받기 -> 압축 풀기 -> IntelliJ에서 open -> 압축 푼 경로로가서 build.gradle 열기 -> Open as Project

- build.gradle
  ```java
  dependencies {
    implementation 'org.springframework.boot:spring-boot-starter'
    testImplementation 'org.springframework.boot:spring-boot-starter-test'
  }
  ``` 
  - 의존관계가 spring-boot-starter와 test관련된 라이브러리 이렇게 두가지만 들어가있다.

- 실행방법
  - src/main/java/hello.core/CoreApplication을 실행하면 됨.
    - 실행하면 바로 끝나야함(왜냐 spring web project를 넣은게 아니기때문에)

- Preferences -> gradle 입력 -> Build and run using : IntelliJ IDEA, Run tests using : IntelliJ IDEA로 수정
  - 이렇게하면 IntelliJ 에서 Java를 바로 실행하기때문에 체감상 더 빠르다.

---

### 비즈니스 요구사항과 설계

- 회원
  - 회원 가입, 회원 조회
  - 회원에는 일반과 VIP 등급이 있다.
  - 회원 데이터는 자체 DB를 구축할 수도 있고, 외부 시스템과 연동할 수 있다.(미확정)
- 주문과 할인 정책
  - 회원은 상품 주문 가능
  - 회원 등급에따라 할인 정책 적용
  - 할인 정책
    - 모든 VIP는 1,000원 할인해주는 고정 금액 할인 적용(나중에 변경될 수도 있음)
  - 할인 정책은 변경 가능성이 높다.
    - 회사의 기본 항린 정책을 아직 정하지 못함, 오픈 직전까지 고민을 미루고 싶다. 최악의 경우 할인을 적용하지 않을 수 있다(미확정)

- 미확정인 부분때문에 개발을 무기한 기다릴 수는 없다.
- <strong>인터페이스를 만들고 구현체를 언제든지 갈아끼울 수 있도록 설계하면 된다.</strong>
  
---

### 회원 도메인 설계

- 회원 도메인 협력 관계
  - 기획자들도 볼 수 있는 그림
  - ![member_domain](./readme_img/member_domain.JPG)
  - 클라이언트(역할)가 회원 서비스 호출
  - 회원 서비스(역할)는 두가지 기능을 제공함,
    - 회원가입
    - 회원조회
  - 회원 저장소(역할)라는 인터페이스를 별도로 생성
    - 왜냐하면 회원 db를 자체 구축할 수도 있고, 외부 시스템과 연동할 수 있기 때문.
    - 회원 데이터에 접근하는 계층을 따로 만듦.
  - 회원 저장소의 구현
    - 메모리 회원 저장소(구현)
    - DB 회원 저장소(구현)
    - 외부 시스템 연동 회원 저장소(구현)
    - 위 셋 중하나를 회원 저장소 인터페이스에 꼽으면 된다.
    - 일단은, 메모리 회원 저장소(간단함)를 만들어서 개발을 진행하기로 함.(단, 메모리이기때문에 서버가 재부팅되면 데이터가 날라가니까 개발할때만 사용)

- 회원 클래스 다이어그램
  - 도메인 협력 관계를 바탕으로 개발자들이 구체화하여 클래스 다이어그램을 생성
  - interface랑 구현체들이 보임
  - 실제 구현 level
  - 서버를 실행하지 않고 클래스들만 분석해서 볼 수 있는 그림
  - ![class_diagram](./readme_img/class_diagram.JPG)
  - MemberService(역할)(interface)
    - 회원 서비스
    - MemberServiceImpl(구현체)
  - MemberRepository(역할)(interface)
    - 회원 저장소
    - MemoryMemberRepository(구현체)
    - DbMemberRepository(구현체)

- 회원 객체 다이어그램
  - 구현체들은 서버가 뜰때 동적으로 결정이 됨. 이를 표현하고자 함.
  - 실제 서버에 올라오면 객체간의(메모리 간의) 참조들이 어떻게 되는지 그린거임.
  - ![entity_diagram](./readme_img/entity_diagram.JPG)
  - 클라이언트는 회원 서비스를 바라 봄.
  - 회원 서비스(정확히는 회원 서비스 구현체)는 메모리 회원 저장소를 바라봄.

- 설계 순서
  - 도메인 -> 클래스 다이어그램 -> 객체 다이어그램

---

### 회원 도메인 개발

- 위에서 작성한 회원 클래스 다이어그램을 바탕으로 개발하기.
- member package 생성
  - Grade(enum)
    - 회원 등급을 나타낸다
    - BASIC, VIP
  - Member(Class, Entity)
    - 3가지 속성을 가짐
      - id, name, grade
      ```java
      private Long id;
      private String name;
      private Grade grade;
      ``` 
    - 생성자 만들기
      ```java
      public Member(Long id, String name, Grade grade) {
        this.id = id;
        this.name = name;
        this.grade = grade;
      }
      ``` 
    - Getter & Setter 생성
      - 데이터를 가져오고 꼽아주는 역할
      - Getter 와 Setter를 통해 private의 값들을 설정해줄 수 있다.  
  - MemberRepository(interface)
    ```java
    public interface MemberRepository {

      void save(Member member);

      Member findById(Long memberId);
    }
    ```
    - save()
      - 회원 저장
    - findById()
      - 회원의 id로 회원을 찾는 기능
  - MemoryMemberRepository(구현체)
    - 보통은 따로 package만들어서 구현체끼리 묶어두나 간편한 예제니까 같은 member package에 넣어둠
    - 구현체니까 아래와 같이 해야함
      ```java
      public class MemoryMemberRepository implements MemberRepository
      ```
    - 저장소니까 Map같은 저장소가 있어야함
      ```java
      private static Map<Long, Member> store = new HashMap<>();
      ```
      - HashMap<>()은 동시성 이슈가 있을 수 있어서 사실은 ConcurrentHashMap을 써야한다.
    - save(Member member)
    - findById(Long memberId)
      - store에서 get()해서 넘어온 memberId를 가지고 찾는기능.
    - 이렇게 간단하게 메모리로 사용하는 db를 만들었고 개발을 진행할 수 있다. 물론 메모리로만 진행하기 때문에 test용도로만 써야한다.

  - MemberService(interface)
    - 2가지 기능이 있음.
    - join()
      - 회원 가입
    - findMember()
      - 회원 조회
  - MemberServiceImpl(구현체)
    - 가입을하고 조회를 할려면 필요한 것이 MemberRepository이다. 그러나, MemberRepository는 interface이므로 구현 객체를 선택해서 넣어줘야함.
      ```java
      private final MemberRepository memberRepository = new MemoryMemberRepository();
      ``` 
    - 회원 가입
      ```java
      @Override
      public void join(Member member) {
        memberRepository.save(member);
      }
      ``` 
      - join()에서 save()를 호출하면 다형성에 의해서 MemoryMemberRepository에 있는 save()가 호출이 된다.
    - 회원 조회
      ```java
      @Override
      public Member findMember(Long memberId) {
        return memberRepository.findById(memberId);
      }
      ``` 

---

### 회원 도메인 실행과 테스트

- 회원 객체 다이어그램의 그림을 만들거임.
- 런타임에 동작 -> 클라이언트는 MemberServiceImpl을 사용하게 됨 -> 회원 서비스는 메모리 회원 저장소를 참조함.
- src/main/java/hello.core에 MemberApp 생성
  - 여기서 잘되는지 test할 예정
  - MemberService를 만들어서 구현체로 new MemberServiceImpl()해서 선택해줌.
  - join() test
    - member를 생성자를 통해 객체 생성
    - join(member)
    - memberService.findMember()를 통해 가입한 멤버랑 찾은 멤버가 똑같으면 원하는데로 test가 된거임
  - 위 방식대로 test한 것은 순수한 자바코드로 진행한거임(spring 관련X)
  - 그런데, 애플리케이션 로직으로 main method를 test하는것은 한계가 있음.(좋은 방법이 아님)
  - <strong>그래서, Junit이라는 test framework를 사용한다.</strong>

- test(junit)
  - src/test/java/hello.core/ 에 member package 생성
  - src/test/java/hello.core/member/ 에 MemberServiceTest class 생성
    -join() Test
      ```java
      MemberService memberService = new MemberServiceImpl();

      @Test
      void join(){
        //given
        Member member = new Member(1L,"memberA",Grade.VIP);

        //when
        memberService.join(member);
        Member findMember = memberService.findMember(1L);

        //then
        Assertions.assertThat(member).isEqualTo(findMember);
      }
      ``` 
    - given
      - ~~한것들이 주어졌을때
    - when
      - 이렇게 햇을때
    - then
      - 요렇게 된다.
    - 검증
      - Assertions(org.assertj.core.api)를 통해 검증하면 됨
  - join test를 실행하면 성공한 모습을 볼 수 있다.
  - 위에서 순수 자바코드로 검증하면 눈으로 직접(출력된 결과를 보면서) 검증했었지만, junit으로 검증하면 출력된 결과를 직접 보면서 검증하는 것이 아니라 성공, 실패의 유무를 바로 확인 가능하다.
  - test code 작성은 필수적이다.

- 회원 도메인 설계의 문제점
  - 다른 저장소로 변경할 때 OCP 원칙을 준수하지 못함.
  - DIP 원칙을 준수하지 못함.
  - 즉, <strong>의존관계가 인터페이스 뿐만 아니라 구현까지 모두 의존하는 문제점이 있음</strong>
    - 코드에서는 아래 부분이 구현체를 의존하는 부분이다.
    ```java
    public class MemberServiceImpl implements MemberService{
      private final MemberRepository memberRepository = new MemoryMemberRepository();
      ...
      ...
      ...
    ``` 
      - 앞의 MemberRepository라는 interface에 의존을 하지만, 뒤에 실제 할당하는 부분인 new MemoryMemberRepository()부분에서 구현체를 의존한다.
      - 그래서 MemberServiceImpl은 MemberRepository(추상화) 뿐만 아니라 MemoryMemberRepository(구체화)도 의존한다.

---

### 주문과 할인 도메인 설계

- 주문과 할인 정책(only 역할에 대한 그림)
  - [비즈니스 요구사항과 설계](#비즈니스-요구사항과-설계) 에서 주문과 할인 정책 확인하고 오기.
- 주문 도메인 협력, 역할, 책임
  - ![order_domain](./readme_img/order_domain.JPG)
  - `클라이언트`는 주문 생성을 할 수 있음.
    - 클라이언트는 Spring MVC에서 Controller가 될 듯.
  - `주문 서비스 역할`는 주문 생성의 역할을 함.
    - 회원 등급이 필요하기 때문에 `회원 저장소 역할`에서 회원 조회해서,
    - 그 회원의 등급을 가지고 `할인 정책 역할`에다가 물어보고, 할인의 결과를 주문 서비스 역할에다가 전달해주고,
  - `주문 서비스 역할`은 최종적으로 할인이 적용된 결과를 `클라이언트`에게 반환한다.
  - 참고: 실제로는 주문 데이터를 DB에 저장하겠지만, 예제가 너무 복잡해 질 수 있어서 생략하고, 단순히 주문 결과를 반환.

- 주문 도메인 전체(역할 + 구현에 대한 그림)
  - ![all_order_domain](./readme_img/all_order_domain.JPG)
  - 위 그림을 잘 보면 `역할` 먼저 만들고, `구현`을 그 다음에 만듦.
    - `역할`과 `구현`을 분리했기 때문에, 자유롭게 `구현 객체`를 조립할 수 있게 설계가 된거다.(유연하게 변경 가능)

- 주문 도메인 클래스 다이어그램
  - 위에서 만든 그림을 가지고 아래와 같은 클래서 다이어그램 만듦.
  - ![order_domain_class](./readme_img/order_domain_class.JPG)

- 주문 도메인 객체 다이어그램1
  - 클래스 다이어그램과 다르게 실제 내가 애플리케이션을 끼워서 동적으로 객체들의 연관관계가 맺어지는 그림
  - ![order_domain_entity1](./readme_img/order_domain_entity1.JPG)
  - `클라이언트`가 `주문 서비스 구현체`를 호출하면, `메모리 회원 저장소`를 호출 + `정액 할인 정책`을 호출한다.
  - 즉, 회원을 메모리에서 조회하고, 정액 할인 정책(고정 금액)을 지원해도 주문 서비스를 변경하지 않아도 된다. 역할들의 협력 관계를 그대로 재사용 할 수 있다.

- 주문 도메인 객체 다이어그램2
  - ![order_domain_entity2](./readme_img/order_domain_entity2.JPG)
  - 나중에 바뀌면 구현체를 위와같이 바꿔서 끼우면 됨.
  - 회원을 메모리가 아닌 실제 DB에서 조회하고, 정률 할인 정책(쭈문 금액에 따라 % 할인)을 지원해도 주문 서비스를 변경하지 않아도 된다.
  - 따라서, <strong>협력 관계를 그대로 재사용 할 수 있다.</strong>

---

### 주문과 할인 도메인 개발

- discount 관련 개발
  - src/main/java/hello.core/discount package 생성
  - DiscountPolicy interface 생성
    - 할인 대상 금액을 반환해줌
  - FixDiscountPolicy Class 생성(정액할인정책 구현체)
    ```java
    private int discountFixAmount = 1000; // 1000원 할인

    @Override
    public int discount(Member member, int price) {
      if (member.getGrade() == Grade.VIP){
          return discountFixAmount;
      }else{
          return 0;
      }
    }
    ``` 
    - VIP면 1000원 할인, 그 외는 0원 할인
- order 관련 개발
  - src/main/java/hello.core/order package 생성
  - Order class 생성
    - 주문에서 할인이 다 끝나고 만들어지는 객체
    - field에 memberId, itemName, itemPrice,discountPrice(할인 금액)
    - 그 후, 생성자 생성
    - 그리고, getter, setter 생성
    - calculatePrice()(계산 로직)
      ```java
      public int calculatePrice(){
        return itemPrice - discountPrice;
      }
      ``` 
    - toString()
      - Generate->toString()해서 생성
      - 편하게 객체의 데이터를 보기 위해서 생성
      - 객체를 출력하면 toString()의 결과가 나옴

  - OrderService interface 생성
    - createOrder()
      - OrderService에는 주문을 생성할때 회원 id, 상품명, 상품 가격을 파라미터로 넘겨야함. 그러면, return으로 주문 결과를 반환한다.

  - OrderServiceImpl class 생성
    - OrderService는 MemberRepository에서 회원을 찾아야하고, DiscountPolicy가 필요함.
      ```java
      private final MemberRepository memberRepository = new MemoryMemberRepository();
      private final DiscountPolicy discountPolicy = new FixDiscountPolicy();
      ```
       
    - createOrder구현
      ```java
      @Override
      public Order createOrder(Long memberId, String itemName, int itemPrice) {
        Member member = memberRepository.findById(memberId);
        int discountPrice = discountPolicy.discount(member, itemPrice);

        return new Order(memberId, itemName, itemPrice, discountPrice);
      }
      ```
      - OrderService 입장에서는 할인에 대해서는 잘 모르지만 할인에 대한 부분은 discountPolicy가 알아서 해주고 그에 대한 결과만 얻어옴.
        - 단일 체계 원칙을 잘 지킴
        - 만약, 할인에 대한 변경이 필요하면 할인 부분만 고치면 됨.(주문까지는 안건들여도 됨.)

---

### 주문과 할인 도메인 실행과 테스트

주문이 원하는대로 동작하는지 main method 생성해봄.(물론 좋은 방법이 아님.)
- src/main/java/hello.core/order/OrderApp class 생성
  - 임의의 VIP member를 생성하고 이를 메모리DB에 넣어줌(그래야 주문에서 찾아 쓸 수 있으니까)
    ```java
    Long memberId = 1L;
    Member member = new Member(memberId, "memberA", Grade.VIP);
    memberService.join(member);
    ``` 
  - createOrder를 통해 10000원짜리 itemA를 memberId가 order를 생성함.
    ```java
    Order order = orderService.createOrder(memberId,"itemA",10000);
    ```
  - order를 출력하면 Order Class의 toString으로 인해 아래와 같은 출력물이 나온다.
    - ![print_order](./readme_img/print_order.JPG)
    <br/>


junit을 통해 test하기
- 위와 같이 비슷하게 만들면 됨.
  ```java
  @Test
  void createOrder(){
    Long memberId = 1L;
    Member member = new Member(memberId, "memberA", Grade.VIP);
    memberService.join(member);

    Order order = orderService.createOrder(memberId, "itemA", 10000);
    Assertions.assertThat(order.getDiscountPrice()).isEqualTo(1000);
  }
  ``` 
  - @Test 해줘야함.
  - sysout 대신 Assertions으로 확인.

- 단위 test를 잘 만드는 것이 중요함.
  - 단위 test란 spring이나 컨테이너의 도움 없이 순수하게 자바코드로 test를 하는 것.


---
---

## 스프링 핵심 원리 이해2 - 객체 지향 원리 적용

---
---

### 새로운 할인 정책 개발

>할인 정책을 고정할인금액(VIP는 1000원 할인)보다는 주문 금액당 정률% 할인으로 바꾸고자 한다.

- 애자일 고프트웨어 개발 선언
  >공정과 도구보다 `개인과 상호작용`을<br> 
  포괄적인 문서보다 `작동하는 소프트웨어`를<br> 
  게약 협상보다 `고객과의 협력`을<br> 
  계획을 따르기보다 `변화에 대응하기`를<br> 
  가치 있게 여긴다.

- RateDiscountPolicy 개발
  - ![ratediscount](./readme_img/ratediscount.JPG)
  - 아래와 같이 일단 작성
  ```java
  private int discountPercent = 10;

  @Override
  public int discount(Member member, int price) {
    if(member.getGrade() == Grade.VIP){
      return price * discountPercent / 100;
    }else{
      return 0;
    }
  }
  ```

- RateDiscountPolicyTest 생성
  - 아래와 같이 코드 작성(성공 test)
  ```java
  @Test
  @DisplayName("VIP는 10% 할인이 적용되어야 한다")
  void vip_o(){
    //given
    Member member = new Member(1L, "memberVIP", Grade.VIP);
    //when
    int discount = discountPolicy.discount(member, 10000);
    //then
    Assertions.assertThat(discount).isEqualTo(1000);
  }
  ``` 
  - @DisplayName() : junit5에서 부터 지원하면 test 실행 결과를 vip_o 대신 괄호안에 적힌 문자로 나옴.
  - test를 할때에는 `성공 test`도 중요하나 `실패 test`도 중요하다.
  - 아래와 같이 코드 작성(실패 test)
  ```java
  @Test
  @DisplayName("VIP가 아니면 할인이 적용되지 않아야 한다")
  void vip_x(){
    //given
    Member member = new Member(2L, "memberBASIC", Grade.BASIC);
    //when
    int discount = discountPolicy.discount(member, 10000);
    //then
    Assertions.assertThat(discount).isEqualTo(1000);
  }
  ``` 

---

### 새로운 할인 정책 적용과 문제점

- 위에서 만든 새로운 할인 정책을 적용을 할려면 OrderServiceImpl로 들어가 아래와 같이 코드를 고쳐야한다.
  ```java
  //private final DiscountPolicy discountPolicy = new FixDiscountPolicy();
  private final DiscountPolicy discountPolicy = new RateDiscountPolicy();
  ...
  ...
  ```
  - 할인 정책을 변경할려면 클라이언트인 `OrderServiceImpl` 코드를 고쳐야 한다.

- 위에서 `문제점`을 발견함!!
  - 역할과 구현 분리 O
  - 다형성 활용, 인터페이스와 구현 객체 분리 O
  - OCP, DIP와 같은 객체지향 설계 원칙 준수? X
    - 그렇게 보이지만 아님!
  - DIP: 주문서비스 클라이언트 `OrderServiceImpl`는 인터페이스(추상)뿐만 아니라 `구현체 클래스에도 의존`하고 있다.
    - interface 의존 : `DiscountPolicy`
    - 구현체 의존 : `FixDiscountPolicy`, `RateDiscountPolicy`
    - 실제 의존 관계
      ![real](./readme_img/real.JPG)
  - OCP : 변경하지 않고 확장해야함
    - 지금 코드는 `기능을 확장해서 변경`하면, `클라이언트 코드에 영향을 줌`.
    - 정책 변경
      ![change_policy](./readme_img/change_policy.JPG)

<br/>
<strong> 위와 같은 문제를 어떻게 해결할 수 있을까?</strong><br/>

- `인터페이스에만 의존하도록 설계를 변경하자`
  - ![only_interface](./readme_img/only_interface.JPG)
  - 아래와 같이 코드 변경
  ```java
  //private final DiscountPolicy discountPolicy = new FixDiscountPolicy();
  //private final DiscountPolicy discountPolicy = new RateDiscountPolicy();
  private DiscountPolicy discountPolicy;
  ``` 
  - DiscountPolicy는 interface이다. 즉, OrderServiceImpl은 추상화인 DiscountPolicy에만 의존한다.

- 위와 같이 코드를 수정한 뒤, OrderServiceTest를 돌리면 `NullPointerException`이 발생
  - 구현체 없이 인터페이스만 가지고 돌렸기 때문.

<strong>해결 방안</strong>

- 누군가 클라이언트인 `OrderServiceImpl`에 `DiscountPolicy`의 구현 객체를 대신 생성하고 주입해주어야 한다.

---

### 관심사의 분리

>중요

- 애플리케이션을 하나의 공연이라고 생각해보자
  - 각각의 `인터페이스` == `배역(배우 역할)`
  - 이 배역에 맞는 `배우를 선택`하는 것은 `누가`하는가?
  - 배역을 정하는 것은 배우들이 정하는게 아닌 `공연 기획자`가 정하는 거다.
  - 이전 코드는 마치 `로미오 역할(인터페이스)`을 하는 `레오나르도 디카프리오(구현체,배우)`가 `줄리엣 역할(인터페이스)`을 하는 `여자 주인공(구현체, 배우)`을 직접 초빙하는 것과 같다.

  - `OrderServiceImpl`은 `OrderService와 관련된 로직만 `해야하는데, discountPolicy를 자기가 직접 선택까지 함.(관심사 분리 X)

`관심사를 분리하자`(공연 기획자를 만들고, 배우와 공연 기획자의 책임을 확실히 분리하자.)

<strong>AppConfig 등장</strong>

- 애플리케이션의 전체 동작 방식을 구성(or 설정)(config)하기 위해, <strong>구현 객체를 생성</strong>하고, <strong>연결</strong>하는 책임을 가지는 별도의 설정 클래스를 만들자.
  - src/main/java/hello.core/AppConfig class 생성

- MemberServiceImpl class로 가서 코드를 아래와 같이 수정
  ```java
  //private final MemberRepository memberRepository = new MemoryMemberRepository();
  private final MemberRepository memberRepository;

  public MemberServiceImpl(MemberRepository memberRepository) {
    this.memberRepository = memberRepository;
  }
  ``` 
  - 생성자를 통해서 이 MemberRepositoryImpl에 뭐가 들어갈지를 선택함.
- AppConfig class에서 아래와 같이 코드 작성.
  ```java
  public MemberService memberService(){
    return new MemberServiceImpl(new MemoryMemberRepository());
  }
  ``` 
  - 어디선가 `AppConfig`를 통해서 `memberService`를 불러다 사용한다.
  - 그러면, `MemberService` 구현체 객체가 생성이 되는데, 그 때 `MemoryMemberRepository`가 들어간다.
- 위와 같이 코드를 수정할 경우, `MemberServiceImpl`에 `MemoryMemberRepository`(즉 구현체)에 대한 코드는 없어진다!
  - 즉, `추상화에만 의존한다`

-  위와 같은 과정을 `생성자 주입`이라고 한다.
   -  생성자를 통해서 객체가 들어간다

- 마찬가지로 OrderService도 바꿔준다.
  - `OrderServiceImpl`은 사용하는 field가 2개이다.
    - `MemberRepository`,`DiscountPolicy`
  - `OrderServiceImpl` 코드 수정
    ```java
    //private final MemberRepository memberRepository = new MemoryMemberRepository();
    //private final DiscountPolicy discountPolicy = new FixDiscountPolicy();
    //private final DiscountPolicy discountPolicy = new RateDiscountPolicy();
    private final MemberRepository memberRepository;
    private final DiscountPolicy discountPolicy;

    public OrderServiceImpl(MemberRepository memberRepository, DiscountPolicy discountPolicy) {
      this.memberRepository = memberRepository;
      this.discountPolicy = discountPolicy;
    }
    ```
  - `AppConfig` 코드 추가
    ```java
    public OrderService orderService(){
      return new OrderServiceImpl(new MemoryMemberRepository(), new FixDiscountPolicy());
    }
    ``` 
  - `AppConfig`를 통해서 누군가가 OrderService를 조회하면 `OrderServiceImpl`이 반환이 되는데 거기에 `MemoryMemberRepository`랑 `FixDiscountPolicy`가 들어간다.
  - 그러면, `OrderServiceImpl`은 인터페이스에만 의존하게 된다.

- `AppConfig`는 애플리케이션의 실제 동작에 필요한 <strong>구현 객체를 생성</strong>한다.
  - `MemberServiceImpl`
  - `MemoryMemberRepository`
  - `OrderServiceImpl`
  - `FixDiscountPolicy`
- `AppConfig`는 생성한 객체 인스턴스의 참조를 <strong>생성자를 통해서 주입(연결)</strong> 해준다.
  - `MemberServiceImpl` -> `MemoryMemberRepository`
  - `OrderServiceImpl` -> `MemoryMemberRepository`, `FixDiscountPolicy`

정리
- 설계 변경으로 `MemberServiceImpl`은 `MemoryMemberRepository`를 의존하지 않는다!
- 단지 `MemberRepository` interface에만 의존.
- `MemberServiceImpl` 입장에서 `생성자`를 통해 어떤 구현 객체가 들어올지(주입될지)는 알 수 없다.
- `MemberServiceImpl의 생성자`를 통해서 어떤 구현 객체를 주입할지는 오직 외부 `AppConfig`에서 결정.
- `MemberServiceImpl`은 이제부터 <strong>의존관계에 대한 고민은 외부</strong>에 맡기고 <strong>실행에만 집중</strong>하면 된다.

클래스 다이어그램
![class_diagram2](./readme_img/class_diagram2.JPG)
- `MemberService`는 interface이다. 
- 이 interface를 구현하는 것이 `MemberServiceImpl`이다.
- 이 `MemberServiceImpl`은 `MemberRepository`라는 interface에 의존한다.
- `AppConfig`가 `MemberServiceImpl`와 `MemoryMemberRepository`를 생성한다.
- 그렇게하여, 객체의 생성과 연결은 `AppConfig`가 담당한다.
- <strong>DIP 완성</strong>
  - `MemberServiceImpl`은 `MemberRepository`인 추상에만 의존하면 된다. 이제 구현체 클래스를 몰라도 됨.
- <strong>관심사 분리</strong>
  - 객체를 생성하고 연결하는 역할(Config)과 실행하는 역할(Impl)이 명확히 분리.

회원 객체 인스턴스 다이어그램
![instance_diagram](./readme_img/instacne_diagram.JPG)
- `AppConfig`가 `MemoryMemberRepository` 객체를 생성.
- 그 다음, `MemberServiceImpl`을 생성할 때, `MemoryMemberRepository`의 참조 값을 같이 생성자에 넘겨줌.
- 그리하여, `MemberServiceImpl`은 생성한 `MemoryMemberRepository`에 대한 값을 주입을 받게 됨.

- <strong>DI(Dependency Injection)</strong>
  - 클라이언트인 `MemberServiceImpl`의 입장에서 보면 의존관계를 마치 외부에서 주입해주는 것 같다고하여 `의존관계 주입` 또는 `의존성 주입`이라고 한다.

`AppConfig` 실행

- `MemberApp` 코드 수정
  ```java
  public static void main(String[] args) {
    AppConfig appConfig = new AppConfig();
    MemberService memberService = appConfig.memberService();
    //MemberService memberService = new MemberServiceImpl();
    ...
    ...
  }
  ``` 
  - 그러면 `AppConfig`로 들어가 `MemberServiceImpl`을 만들고 내가 만든 `MemberServiceImpl`은 `MemoryMemberRepository` 를 사용한다는 의미로 주입해줌.
    ```java
    public class AppConfig {

    public MemberService memberService(){
      return new MemberServiceImpl(new MemoryMemberRepository());
    }
    ```

- `OrderApp` 코드 수정
  ```java
  AppConfig appConfig = new AppConfig();
  MemberService memberService = appConfig.memberService();
  OrderService orderService = appConfig.orderService();
  ``` 
- MemberApp과 OrderApp test를 실행해보면 각각 성공하는 모습을 볼 수 있다.

Test 코드 수정
- `MemberServiceTest`를 아래와 같이 수정
  ```java
  //MemberService memberService = new MemberServiceImpl();
  MemberService memberService;

  @BeforeEach
  public void beforeEach(){
    AppConfig appConfig = new AppConfig();
    memberService = appConfig.memberService();
  }
  ``` 
  - 실행을 하기 전에 `AppConfig`를 만들고, `memberService`를 할당해준다. 그 후, test가 돌아간다. 
- 마찬가지로 `OrderServiceTest`도 수정
  ```java
  //MemberService memberService = new MemberServiceImpl();
  //OrderService orderService = new OrderServiceImpl();
  MemberService memberService;
  OrderService orderService;

  @BeforeEach
  public void beforeEach(){
    AppConfig appConfig = new AppConfig();
    memberService = appConfig.memberService();
    orderService = appConfig.orderService();
  }
  ``` 

#### 정리
- `AppConfig`를 통해서 관심사를 분리.
- 배역, 배우를 생각해보기.
- `AppConfig`는 공연 기획자
- `AppConfig`는 구현체 클래스를 선택.(배약에 맞는 담당 배우 선택). 애플리케이션이 어떻게 동작해야 할지 전체 구성을 책임짐.
- 이제 각 구현체들은(각 배우들은) 담당 기능들을 실행하는 책임만 지면 됨.
- `OrderServiceImpl`은 기능을 실행하는 책임만 지면 됨.

---

### AppConfig 리팩터링

현재 `AppConfig`를 보면 <strong>중복</strong>이 있고, <strong>역할</strong>에 따른 <strong>구현</strong>이 잘 안보인다.(나름 설정 정보니까...)(역할들을 드러나게 하는게 중요함.)

- `AppConfig`를 아래와 같이 수정.
  ```java
  public MemberService memberService(){
    return new MemberServiceImpl(memberRepository());
  }

  private MemberRepository memberRepository() {
    return new MemoryMemberRepository();
  }

  public OrderService orderService(){
    return new OrderServiceImpl(memberRepository(), discountPolicy());
  }

  public DiscountPolicy discountPolicy(){
    return new FixDiscountPolicy();
  }
  ``` 
- `AppConfig`에서 method 이름을 통해서 역할들이 전부 드러남.
  - `MemberService`,`MemberRepository`,`OrderService`,`DiscountPolicy`
- `memberService`는 `MemberServiceImpl`을 사용할거다.
- `memberRepository`에 대한것은 `MemoryMemberRepository`를 사용할거다.
- 'orderService'에 대한 구체적인 것은 현재 내 application에서 `memberRepository`쓰는 것을 가져오고, 현재 내 application에서 `discountPolicy`쓰는 것을 가져온다.
- `discountPolicy`에 대한 것은 `FixDiscountPolicy`를 사용할거다.

- ![config](./readme_img/config.JPG)
  - 그리하여 설계에 대한 그림이 Config에 그대로 드러나게 된다.(역할 + 구현이 한 눈에 들어옴)

- `new MemoryMemberRepository()` 이 부분이 중복 제거되었다. 이제 `MemoryMemberRepository`를 다른 구현체로 변경할 때 한 부분만 변경하면 된다.
- `AppConfig`를 보면 역할과 구현 클래스가 한눈에 들어온다. 애플리케이션 전체 구성이 어떻게 되어있는지 빠르게 파악할 수 있다.


---
---

## IntelliJ 단축키 모음집 & 참고
- 기본적으로 `Preferences -> keymap` 으로 들어간 뒤 본인이 사용하고자하는 단축키 이름일 입력하면 환경에 맞게(window,mac..) 단축키가 나옴
- Preferences(or Settings) 바로가기 : `ctrl+alt+s`
- Generate(생성자,Getter,Setter 등...) : `alt+insert` (나같은 경우 alt+function+delete)
- `Compact middle Package`
- 자동완성(세미콜론까지 포함해서) : `ctrl+shift+enter`
- public static void main(String[] args) 생성 : `psvm + enter`
- 값 추출해서 변수에 넣기 : `ctrl+alt+v`
- Print a value to System.out : `soutv+enter`
- main에서의 함수에서 test 바로 생성하기: `ctrl+shift+t`
- test를 할때 Assertions는 static import하는게 좋음 : `Assertions 커서 두고 +alt+enter+(on demand static~~)`
- 과거 history 보기 : `ctrl+e`
- Extract Method : `ctrl+alt+m`



---
---

## 목차(바로가기)

- [스프링 핵심 원리 - 기본편](#스프링-핵심-원리---기본편)
  - [객체 지향 설계와 스프링](#객체-지향-설계와-스프링)
    - [이야기 - 자바 진영의 추운 겨울과 스프링의 탄생](#이야기---자바-진영의-추운-겨울과-스프링의-탄생)
    - [스프링이란?](#스프링이란)
    - [좋은 객체 지향 프로그래밍?](#좋은-객체-지향-프로그래밍)
    - [좋은 객체 지형 설계의 5가지 원칙(SOLID)](#좋은-객체-지형-설계의-5가지-원칙solid)
    - [객체 지향 설계와 Spring](#객체-지향-설계와-spring)
  - [스프링 핵심 원리 이해1 - 예제 만들기](#스프링-핵심-원리-이해1---예제-만들기)
    - [프로젝트 생성](#프로젝트-생성)
    - [비즈니스 요구사항과 설계](#비즈니스-요구사항과-설계)
    - [회원 도메인 설계](#회원-도메인-설계)
    - [회원 도메인 개발](#회원-도메인-개발)
    - [회원 도메인 실행과 테스트](#회원-도메인-실행과-테스트)
    - [주문과 할인 도메인 설계](#주문과-할인-도메인-설계)
    - [주문과 할인 도메인 개발](#주문과-할인-도메인-개발)
    - [주문과 할인 도메인 실행과 테스트](#주문과-할인-도메인-실행과-테스트)
  - [스프링 핵심 원리 이해2 - 객체 지향 원리 적용](#스프링-핵심-원리-이해2---객체-지향-원리-적용)
    - [새로운 할인 정책 개발](#새로운-할인-정책-개발)
    - [새로운 할인 정책 적용과 문제점](#새로운-할인-정책-적용과-문제점)
    - [관심사의 분리](#관심사의-분리)
      - [정리](#정리)
    - [AppConfig 리팩터링](#appconfig-리팩터링)
  - [IntelliJ 단축키 모음집 & 참고](#intellij-단축키-모음집--참고)
  - [목차(바로가기)](#목차바로가기)

- [스프링 핵심 원리 - 기본편](#스프링-핵심-원리---기본편)
  - [객체 지향 설계와 스프링](#객체-지향-설계와-스프링)
    - [이야기 - 자바 진영의 추운 겨울과 스프링의 탄생](#이야기---자바-진영의-추운-겨울과-스프링의-탄생)
    - [스프링이란?](#스프링이란)
    - [좋은 객체 지향 프로그래밍?](#좋은-객체-지향-프로그래밍)
    - [좋은 객체 지형 설계의 5가지 원칙(SOLID)](#좋은-객체-지형-설계의-5가지-원칙solid)
    - [객체 지향 설계와 Spring](#객체-지향-설계와-spring)
  - [스프링 핵심 원리 이해1 - 예제 만들기](#스프링-핵심-원리-이해1---예제-만들기)
    - [프로젝트 생성](#프로젝트-생성)
    - [비즈니스 요구사항과 설계](#비즈니스-요구사항과-설계)
    - [회원 도메인 설계](#회원-도메인-설계)
    - [회원 도메인 개발](#회원-도메인-개발)
    - [회원 도메인 실행과 테스트](#회원-도메인-실행과-테스트)
    - [주문과 할인 도메인 설계](#주문과-할인-도메인-설계)
    - [주문과 할인 도메인 개발](#주문과-할인-도메인-개발)
    - [주문과 할인 도메인 실행과 테스트](#주문과-할인-도메인-실행과-테스트)
  - [스프링 핵심 원리 이해2 - 객체 지향 원리 적용](#스프링-핵심-원리-이해2---객체-지향-원리-적용)
    - [새로운 할인 정책 개발](#새로운-할인-정책-개발)
    - [새로운 할인 정책 적용과 문제점](#새로운-할인-정책-적용과-문제점)
    - [관심사의 분리](#관심사의-분리)
      - [정리](#정리)
    - [AppConfig 리팩터링](#appconfig-리팩터링)
  - [IntelliJ 단축키 모음집 & 참고](#intellij-단축키-모음집--참고)
  - [목차(바로가기)](#목차바로가기)