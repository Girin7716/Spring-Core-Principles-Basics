# ������ �ٽ� ���� - �⺻��
������ ���� '������ �ٽ� ����-�⺻��'(�迵��)�� �����ϸ� ������ ������Դϴ�.<br>
https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-%ED%95%B5%EC%8B%AC-%EC%9B%90%EB%A6%AC-%EA%B8%B0%EB%B3%B8%ED%8E%B8

---
---

## ��ü ���� ����� ������

---

### �̾߱� - �ڹ� ������ �߿� �ܿ�� �������� ź��
<BR>

������ ����
- 2002�� �ε� ���� å �Ⱓ
- EJB�� ������ ����
- BeanFactory, ApllicationContext, POJO, ������ ����, �������� ����

---

### �������̶�?

- �ʼ�
  - ������ �����ӿ�ũ
  - ������ ��Ʈ

- ����
  - ������ ������ : �⺻���� CRUD�� � �����ͺ��̽��� ����ѵ�, �̷��� ���ϰ� ����� �� �ֵ��� �����ִ� ���� '������ ������'��� ����̴�. �� �� ���� ����ϴ� ���� '������ ������ JPA'�� ���� �����.
  - ������ ���� : ���� ����� ���ϰ� ����� �� �ֵ��� ������.
  - ������ ��ť��Ƽ : ���Ȱ� ����
  - ������ Rest Docs : API������ test�� ���ϰ� ��� API����ȭ�� ���ϰ� ����.
  - ������ ��ġ : ��ġó��(1000���� ������Ʈ�� �ѹ��� �ϴ°� �ƴ� ����� ������Ʈ�ϴ� ����)�� Ưȭ�� ���
  - ������ Ŭ���� : Ŭ���忡 Ưȭ�� ���

- ������ �����ӿ�ũ
  - �ٽ� ��� : ������ DI �����̳�, AOP, �̺�Ʈ, ��Ÿ
  - �� ��� : ������ MVC, ������ WebFlux
  - ������ ���� ��� : Ʈ�����, JDBC, ORM ����, XML ����
  - ��� ���� : ĳ��, �̸���, ��������, �����층
  - �׽�Ʈ : ������ ��� �׽�Ʈ ����
  - ��� : ��Ʋ��, �ڹ�
  - �ֱٿ��� ������ ��Ʈ�� ���ؼ� ������ �����ӿ�ũ�� ������� ���ϰ� ���.

- ������ ��Ʈ
  - <strong>�������� ���ϰ� ����� �� �ֵ��� ����, �ֱٿ��� �⺻���� ���</strong>
  - �ܵ����� ������ �� �ִ� ������ ���ø����̼��� ���� ����
  - Tomcat ���� �� ������ �����ؼ� ������ �� ������ ��ġ���� �ʾƵ� ��.
  - �ս��� ���� ������ ���� starter ���Ӽ� ����
  - �������� 3rd parth(�ܺ�) ���̺귯�� �ڵ� ����
    - ���ſ��� ���� ������ ���������. ������ �ܺ� ���̺귯�� ������ ���ؼ��� ���X
  - ��Ʈ��, ���� Ȯ��, �ܺ� ���� ���� ���δ��� �غ� ��� ����
    - �ȯ�濡�� ����͸��� �߿�. �̷� �κ��� ��������Ʈ�� �⺻������ ��������.
  - ���ʿ� ���� ������ ����
    - �������� ������ �����ӿ�ũ ������ ���������, ��������Ʈ�� �̸� ���ϰ� ����.

- ������ �ܾ�?
  - �������̶�� �ܾ�� ���ƿ� ���� �ٸ��� ���ȴ�.
    - ������ DI �����̳� ���
    - ������ �����ӿ�ũ
    - ������ ��Ʈ, ������ �����ӿ�ũ ���� ��� ������ ������ ���°�

- �������� �ٽ� ����, ����
  - �������� �ڹ� ��� ����� �����ӿ�ũ
  - �ڹ� ����� ���� ū Ư¡ - <strong>��ü ���� ���</strong>
  - �������� ��ü ���� �� ���� ������ Ư¡�� ������� �����ӿ�ũ
  - �������� <strong>���� ��ü ����</strong> ���ø����̼��� ������ �� �ְ� �����ִ� �����ӿ�ũ

---

### ���� ��ü ���� ���α׷���?

- ��ü ���� Ư¡
  - �߻�ȭ
  - ĸ��ȭ
  - ���
  - <strong>������</strong>

- ��ü ���� ���α׷���
  - ��ü ���� ���α׷����� ���α׷��� ��ɾ��� ������� ���� �ð����� ��� ���� ���� ������ ����, �� <strong>"��ü"</strong>���� <strong>����</strong>���� �ľ��ϰ��� �ϴ� ���̴�. ������ <strong>��ü</strong>�� �޽����� �ְ�ް�, �����͸� ó���� �� �ִ�.<strong>(����)</strong>
  - ��ü ���� ���α׷����� ���α׷��� <strong>����</strong>�ϰ� <strong>����</strong>�� �����ϰ� ����� ������ ��Ը� ����Ʈ���� ���߿� ���� ���ȴ�.

- �����ϰ�, ������ ����?
  - ���� �� �����ϵ���
  - Ű����, ���콺 ���� �������
  - ��ǻ�� ��ǰ ���� �������
  - ������Ʈ�� ���� �����ϰ� �����ϸ鼭 ������ �� �ִ� ���
  > ������(Polymorphism)

- �������� �Ǽ��� ����
  - �Ǽ���� ��ü ������ 1:1�� ��Ī�� �� �ȵ�.
  - �׷��� �����ϸ� �����ϱ� ����
  - <strong>����</strong>�� <strong>����</strong>���� ������ ����
    - ���� : �������̽�
    - ���� : �������̽��� ������ ��ü

- ������ - �ڵ��� ����
  - ![car](./readme_img/car.JPG)
  - �ڵ��� ������ 3���� �ٸ� �ڵ����� ����
  - ���� �����ڰ� K3�� Ÿ�ٰ� �ٸ� �ڵ����� �ƹݶ��� ���� �ٲ㵵 �翬�� ������ �� �� ����.
    - �ֳ��ϸ� �ڵ��� ���ҿ� ���� ������ �ٲ���� ���̱� �����̴�.
  - <strong>�׷��� �ڵ����� �ٲ� ���������� ������ ���� �ʴ´�.</strong>
    > �����ϰ� ������ �����ϴ�.
  - �����ڴ� �ڵ��� ���ҿ� ���ؼ��� �����ϰ� �ִ�.
  - �̷��� �ڵ��� ���Ҹ� ����� �ڵ��� ������ �и��� ������ '������'(client)�� ���ؼ� �̷��� ��.
    - client�� �ڵ����� ���� ������ ���� ��.
    - �ڵ��� ������ �ٲ� client���Դ� ������ ����.
  - client�� ������ �����ʰ� ���ο� ����� ������ �� �ִ�.
  - ��, ���ο� �ڵ����� ���͵� client�� ���ο� ���� �ȹ���� ��.

- ���� ���� ����
  - ![show](./readme_img/show.JPG)
  - ���� ��ü�� �����ϴ�.
  - ���Ұ� �������� ���� = ���氡���� ��ü ���ɼ��� ����
    - �����ϰ� ������ �����ϴٶ�� ��

- �������� �Ǽ��� ���� ����
  - ������ - �ڵ���
  - ���� ����
  - Ű����, ���콺, ������ ǥ�� �������̽���
  - ���� �˰���(���ĸ� �Ǹ� �� ���� ����� �˰������� ��ü)
  - ���� ��å ����

- <strong>���Ұ� ������ �и�</strong>
  - <strong>����</strong>�� �������� �����ϸ� ������ <strong>�ܼ�</strong>������, <strong>����</strong>������ <strong>����</strong>�� ��
  - ����
    - <strong>Ŭ���̾�Ʈ</strong>�� ����� ����(�������̽�)�� �˸� �ȴ�.
    - <strong>Ŭ���̾�Ʈ��</strong> ���� ����� <strong>���� ������ ����</strong> �ȴ�.
      - ex> ������ - �ڵ���
    - <strong>Ŭ���̾�Ʈ</strong>�� ���� ����� <strong>���� ������ ����</strong>�Ǿ ������ ���� �ʴ´�.
      - �⸧������ �������� �ٲ� �����ڴ� ���� ����
    - <strong>Ŭ���̾�Ʈ</strong>�� ���� <strong>��� ��ü�� ����</strong>�ص� ������ ���� �ʴ´�.
      - K3���� �׽���� �ٲ㵵 �����ڴ� ������ ���� ����.

- ���Ұ� ������ �и�_�ڹ� ���
  - �ڹ� ����� �������� Ȱ��
    - ���� = �������̽�
    - ���� = �������̽��� ������ Ŭ����, ���� ��ü
  - ��ü�� ������ �� <strong>����</strong>�� <strong>����</strong>�� ��Ȯ�� �и�
  - ��ü ����� ����(�������̽�)�� ���� �ο��ϰ�, �� ������ �����ϴ� ���� ��ü �����

- ��ü�� �����̶�� ������� ����
  - ȥ�� �ִ� ��ü�� ����
  - Ŭ���̾�Ʈ : <strong>��û</strong>, ���� : <strong>����</strong>
  - �� ���� ��ü Ŭ���̾�Ʈ�� ��ü ������ ���� ���� ���踦 ������.
  - ![client_server](./readme_img/client_server.JPG)

- �ڹ� ����� ������
  - ![overriding](./readme_img/overriding.JPG)
    - MemberService�� save()�� ȣ���ϸ�, interface�� MemberRepository�� save()�� ȣ���ϸ�, �����δ� ���� ����ü���� save()�� ȣ���̵ȴ�.(���� ��� ���� MemoryMemberRepository�� �������� �ش� save()�� ȣ��)
  - <strong>�������̵�</strong>�� ���÷�����
  - �������̵��� �ڹ� �⺻ ����
  - �������̵� �� �޼��尡 ����
  - ���������� �������̽��� ������ ��ü�� ���� ������ �����ϰ� ������ �� �ִ�.
  - ���� Ŭ���� ��� ���赵 ������, �������̵� ���밡��
  - ![client](./readme_img/client.JPG)
    - client(MemberService)�� MemberRepository�� �����Ѵ�.
      - �����Ѵ� == ���� ���� �˰� �ִ�.
  - ![overriding](./readme_img/overriding.JPG)
    - MemberRepository�� ����ü(MemoryMemberRepository, JdbcMemberRepository)���� �Ҵ��� �� �ִ�.
      - ![interface](./readme_img/interface.JPG)

    - �ڵ� ����
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

    - � ����ü�� �ֳĿ� ���� �ٸ�
      - ![who](./readme_img/who.JPG)


- <strong>�������� ����</strong>
  - �������̽��� ������ ��ü �ν��Ͻ��� <strong>���� ����</strong>�� �����ϰ� <strong>����</strong>�� �� �ִ�.
  - �������� ������ �����Ϸ��� <strong>����</strong>�̶�� ��ü������ ���迡�� �����ؾ���.
  - <strong>Ŭ���̾�Ʈ�� �������� �ʰ�, ������ ���� ����� �����ϰ� ������ �� �ִ�.</strong>

- ���Ұ� ������ �и�_����
  - �Ǽ����� ���Ұ� �����̶�� ���� ������ �������� ���� ��ü �������� ������ �� ����
  - �����ϰ�, ������ ����
  - Ȯ�� ������ ����
  - Ŭ���̾�Ʈ�� ������ ���� �ʴ� ������ ����
  - �������̽��� ���������� �� �����ϴ� ���� �߿�

- ���Ұ� ������ �и�_�Ѱ�
  - ����(�������̽�) ��ü�� ���ϸ�, Ŭ���̾�Ʈ, ���� ��ο� ū ������ �߻��Ѵ�.
    - �ڵ����� ������ �����ؾ� �Ѵٸ�?
    - �뺻 ��ü�� ����ȴٸ�?
    - USB �������̽��� ����ȴٸ�?
  - �������̽��� ���������� �� �����ϴ� ���� �߿�


- �������� ��ü ����
  - �������� ���� �߿�!
  - �������� �������� �ش�ȭ�ؼ� �̿��� �� �ְ� �����ش�.
  - ���������� �̾߱��ϴ� ������ ����(IoC), �������� ����(DI)�� �������� Ȱ���ؼ� ���Ұ� ������ ���ϰ� �ٷ� �� �ֵ��� �����Ѵ�.
  - �������� ����ϸ� ��ġ ���� �� �����ϵ���! ���� ������ ��츦 �����ϵ���! ������ ���ϰ� ������ �� �ִ�.

---

### ���� ��ü ���� ������ 5���� ��Ģ(SOLID)

- SOLID
    > Ŭ���ڵ�� ������ �ι�Ʈ ��ƾ�� ���� ��ü ���� ������ 5���� ��Ģ�� ����
  - SRP : ���� å�� ��Ģ(Single Responsibility Principle)
  - OCP : ����-��� ��Ģ(Open/Closed Principle)
  - LSP : �������� ġȯ ��Ģ(Liskov Substitution Principle)
  - ISP : �������̽� �и� ��Ģ(Interface Segregation Principle)
  - DIP : �������� ���� ��Ģ(Dependency Inversion Principle)

- SRP ���� å�� ��Ģ
  - �� Ŭ������ �ϳ��� å�Ӹ� ������ �Ѵ�.
  - �ϳ��� å���̶�� ���� ��ȣ�ϴ�.
    - Ŭ �� �ְ�, ���� �� �ִ�.
    - ���ư� ��Ȳ�� ���� �ٸ���.
  - <strong>�߿��� ������ ����</strong>�̴�. ������ ���� �� �ı� ȿ���� ������ ���� å�� ��Ģ�� �� ���� ��
  - EX> UI ����, ��ü�� ������ ����� �и�

- OCP ����-��� ��Ģ(�߿�)
  - ����Ʈ���� ��Ҵ� <strong>Ȯ�忡�� ����</strong> ������ <strong>���濡�� ����</strong> �־�� �Ѵ�.
    - �ڵ��� ������� ����� �߰��� �� �ִ�??
- <strong>������</strong>�� Ȱ���غ���
- �������̽��� ������ ���ο� Ŭ������ �ϳ� ���� ���ο� ����� ����
- ���ݱ��� ��� ���Ұ� ������ �и��� �����غ���.
    - �ڵ� ����
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

    - MemberService�� ����,
      - 1���ڵ�) field�� MemberRepository �������̽��� �˰� �ְ� new �ؼ� MemoryMemberRepository�� ����.
      - 2���ڵ�) field�� MemberRepository �������̽��� �˰� �ְ� new �ؼ� JdbcMemberRepository�� ����.
    - �� �ڵ带 ���� JDBC�� �ٲܷ��� �ᱹ �ڵ带 �����ؾ��Ѵ�.

- OCP ����-��� ��Ģ_������
  - MemberService Ŭ���̾�Ʈ�� ���� Ŭ������ ���� ����
    - 
    ```java
    MemberRepository m = new MemoryMemberRepository();//�����ڵ�
    ```
    - 
    ```java
    MemberRepository m = new JdbcMemberRepository();//���� �ڵ�
    ```
  - <strong>���� ��ü�� �����Ϸ��� Ŭ���̾�Ʈ �ڵ带 �����ؾ� �Ѵ�.</strong>
  - <strong>�и� �������� ��������� OCP ��Ģ�� ��ų �� ����.</strong>
  - �� ������ ��� �ذ��ؾ� �ϳ�?
  - ��ü�� �����ϰ�, �������踦 �ξ��ִ� ������ ����, �����ڰ� �ʿ��ϴ�.
    - ������ �����̳ʰ� ����.

- LSP �������� ġȯ ��Ģ
  - ���α׷��� ��ü�� ���α׷��� ��Ȯ���� ���߸��� �����鼭 ���� Ÿ���� �ν��Ͻ��� �ٲ� �� �־�� �Ѵ�.
    - EX> �ڵ��� �������̽��� ������ ������ ����� ����̴�. �׷���, �ڷ� ���� �����ϸ� LSP ����, �������� ������ ������.(�׷��� ������ ������ ���� �ʰ� ������ ������ �ȵ�. ��������� ������ �������.)
  - ���������� ���� Ŭ������ �������̽� �Ծ��� �� ���Ѿ� �Ѵٴ� ��, �������� �����ϱ� ���� ��Ģ, �������̽��� ������ ����ü�� �ϰ� ����Ϸ���, �� ��Ģ�� �ʿ��ϴ�.
  - �ܼ��� �����Ͽ� �����ϴ� ���� �Ѿ�� �̾߱�
  
- ISP �������̽� �и� ��Ģ
  - Ư�� Ŭ���̾�Ʈ�� ���� �������̽� ���� ���� ���� �������̽� �ϳ����� ����.
  - �ڵ��� �������̽� -> ���� �������̽�, ���� �������̽��� �и�.(�ڵ��� �������̽��� �ʹ� ũ�ϱ� �и�, �̴� ����� Ŭ���̾�Ʈ�� ������ Ŭ���̾�Ʈ�� ����� Ŭ���̾�Ʈ�� �и��� �� �ִ�.)
  - ����� Ŭ���̾�Ʈ -> ������ Ŭ���̾�Ʈ, ����� Ŭ���̾�Ʈ�� �и�.
  - �и��ϸ� ���� �������̽� ��ü�� ���ص� ������ Ŭ���̾�Ʈ�� ������ ���� ����.
  - �������̽��� ��Ȯ������, ��ü ���ɼ��� ��������.


- <strong>DIP �������� ���� ��Ģ(�߿�)</strong>
  - ���α׷��Ӵ� "�߻�ȭ�� �����ؾ���, ��üȭ�� �����ϸ� �ȵȴ�." ������ ������ �� ��Ģ�� ������ ��� �� �ϳ���.
  - ���� �̾߱��ؼ� ���� Ŭ������ �������� ����, �������̽��� �����϶�� ��.(��, Ŭ���̾�Ʈ �ڵ尡 ���� Ŭ������ �ٶ��� ���� �������̽��� �ٶ󺸰� �ϱ�, MemberService�� MemberRepository interface�� �ٶ󺸰��ϰ�, MemoryMemberRepository�� JdbcMemberRepository�� ���ؼ��� ������Ѵ�.)
  - �տ��� �̾߱��� <strong>����(Role)�� �����ϰ� �ؾ� �Ѵٴ� �Ͱ� ����.</strong> ��ü ���� Ŭ���̾�Ʈ�� �������̽��� �����ؾ� �����ϰ� ����ü�� ������ �� �ִ�! ����ü�� �����ϰ� �Ǹ� ������ ���� ���������.
  - �׷��� OCP���� ������ MemberService�� �������̽��� ����������, ���� Ŭ������ ���ÿ� �����Ѵ�.
  - MemberService Ŭ���̾�Ʈ�� ���� Ŭ������ ���� ����
    ```java
    MemberRepository m = new MemoryMemberRepository();
    ```
  - <strong>DIP ����</strong>

- ����
  - ��ü ������ �ٽ��� ������
  - ������ �����δ� ���� ��ǰ�� ���� ������� ������ �� ����.
  - ������ �����δ� ���� ��ü�� ������ �i Ŭ���̾�Ʈ �ڵ嵵 �Բ� ����ȴ�.
  - <strong>������ �����δ� OCP, DIP�� ��ų �� ����.</strong>
  - ���� �� �ʿ���.


---

### ��ü ���� ����� Spring

- ������ �̾߱⿡ �� ��ü ���� �̾߱Ⱑ �����°�?
  - <strong>�������� ���� ����� ������ + OCP, DIP�� �����ϰ� ����</strong>
    - DI(Dependency Injection): ��������, ������ ����
    - DI �����̳� ����
      - �ڹ� ��ü���� � �����̳ʾȿ� �־�ΰ� �� �ȿ��� ���� �������踦 �������ְ� �������ִ� ��ɵ��� ��������.
  - <strong>Ŭ���̾�Ʈ �ڵ��� ���� ���� ��� Ȯ��</strong>
  - ���� ��ǰ�� ��ü�ϵ��� ����.

- �������� ���� ����
  - ���� � �����ڰ� ���� ��ü ���� ������ �Ϸ��� OCP, DIP ��Ģ�� ��Ű�鼭 ������ �غ���, �ʹ� ������ ���Ҵ�. �躸�� ����� ũ��. �׷��� �����ӿ�ũ�� ��������.
  - �����ϰ� �ڹٷ� OCP, DIP ��Ģ���� ��Ű�鼭 ������ �غ���, �ᱹ ������ �����ӿ�ũ�� ����� �ȴ�,(�� ��Ȯ���� DI �����̳�)
  - DI ������ ���� �����ص� ���ذ� �� �ȵ� -> �ڵ�� ¥���� �ʿ伺�� �˰Եȴ�!

- ����
  - ��� ���迡 <strong>����</strong>�� <strong>����</strong>�� �и�����.
  - �ڵ���, ������ ���� ���÷�����.
  - ���ø����̼� ���赵 ������ ���� �ϵ��� �迪�� ������ְ�, ���� �������� <strong>����</strong>�ϰ� <strong>����</strong>�� �� �ֵ��� ����� ���� ���� ��ü ���� �����.
  - �̻������δ� ��� ���迡 �������̽��� �ο�����.

- ����_�ǹ� ���
  - ������ �������̽��� �����ϸ� �߻�ȭ��� ����� �߻��Ѵ�.
    - �ܼ��ϰԴ�, �������̽� Ŭ������ ���� Ŭ������ ������ ��.
    - �߻�ȭ�� �ǹ����� �����ڰ� �ڵ带 �ѹ� �� ���������.(�������̽��� ����, ����ü�� ����)
  - ����� Ȯ���� ���ɼ��� ���ٸ�, ����ü Ŭ������ ���� ����ϰ�, ���� �� �ʿ��� �� �����͸��ؼ� �������̽��� �����ϴ� �͵� ����̴�.

- å��õ
  - ��ü���� å ��õ : ��ü������ ��ǰ� ����
  - ������ å ��õ : ����� ������(�ʼ�)
  - JPA å ��õ : �ڹ� ORM ǥ�� JPA ���α׷���

---
---

## ������ �ٽ� ���� ����1 - ���� �����

�� �ܿ������� ������ Java�θ� �ۼ��غ�����.(������Ʈ ȯ�漳���� ���ϰ� �Ϸ��� ������ ��Ʈ�� ����ϱ� ��. �׿ܿ��� ������ �ڹٷθ� ����)

---
---

### ������Ʈ ����

- ȯ��
  - Java11
  - IntelliJ
- start.spring.io���� �Ʒ��� ���� ������Ʈ ����
  - Gradle Project
  - Java
  - 2.4.2
  - Project Metadata
    - Group : hello
    - Artifact(�����) : core
    - Packaging : Jar
    - Java : 11
  - Dependencies : �ƹ��͵� ���þ��Ұ���(only �ڹٷ� �ۼ��ҰŶ�)

- �� ���� �� �ٿ� �ޱ� -> ���� Ǯ�� -> IntelliJ���� open -> ���� Ǭ ��ηΰ��� build.gradle ���� -> Open as Project

- build.gradle
  ```java
  dependencies {
    implementation 'org.springframework.boot:spring-boot-starter'
    testImplementation 'org.springframework.boot:spring-boot-starter-test'
  }
  ``` 
  - �������谡 spring-boot-starter�� test���õ� ���̺귯�� �̷��� �ΰ����� ���ִ�.

- ������
  - src/main/java/hello.core/CoreApplication�� �����ϸ� ��.
    - �����ϸ� �ٷ� ��������(�ֳ� spring web project�� ������ �ƴϱ⶧����)

- Preferences -> gradle �Է� -> Build and run using : IntelliJ IDEA, Run tests using : IntelliJ IDEA�� ����
  - �̷����ϸ� IntelliJ ���� Java�� �ٷ� �����ϱ⶧���� ü���� �� ������.

---

### ����Ͻ� �䱸���װ� ����

- ȸ��
  - ȸ�� ����, ȸ�� ��ȸ
  - ȸ������ �Ϲݰ� VIP ����� �ִ�.
  - ȸ�� �����ʹ� ��ü DB�� ������ ���� �ְ�, �ܺ� �ý��۰� ������ �� �ִ�.(��Ȯ��)
- �ֹ��� ���� ��å
  - ȸ���� ��ǰ �ֹ� ����
  - ȸ�� ��޿����� ���� ��å ����
  - ���� ��å
    - ��� VIP�� 1,000�� �������ִ� ���� �ݾ� ���� ����(���߿� ����� ���� ����)
  - ���� ��å�� ���� ���ɼ��� ����.
    - ȸ���� �⺻ �׸� ��å�� ���� ������ ����, ���� �������� ����� �̷�� �ʹ�. �־��� ��� ������ �������� ���� �� �ִ�(��Ȯ��)

- ��Ȯ���� �κж����� ������ ������ ��ٸ� ���� ����.
- <strong>�������̽��� ����� ����ü�� �������� ���Ƴ��� �� �ֵ��� �����ϸ� �ȴ�.</strong>
  
---

### ȸ�� ������ ����

- ȸ�� ������ ���� ����
  - ��ȹ�ڵ鵵 �� �� �ִ� �׸�
  - ![member_domain](./readme_img/member_domain.JPG)
  - Ŭ���̾�Ʈ(����)�� ȸ�� ���� ȣ��
  - ȸ�� ����(����)�� �ΰ��� ����� ������,
    - ȸ������
    - ȸ����ȸ
  - ȸ�� �����(����)��� �������̽��� ������ ����
    - �ֳ��ϸ� ȸ�� db�� ��ü ������ ���� �ְ�, �ܺ� �ý��۰� ������ �� �ֱ� ����.
    - ȸ�� �����Ϳ� �����ϴ� ������ ���� ����.
  - ȸ�� ������� ����
    - �޸� ȸ�� �����(����)
    - DB ȸ�� �����(����)
    - �ܺ� �ý��� ���� ȸ�� �����(����)
    - �� �� ���ϳ��� ȸ�� ����� �������̽��� ������ �ȴ�.
    - �ϴ���, �޸� ȸ�� �����(������)�� ���� ������ �����ϱ�� ��.(��, �޸��̱⶧���� ������ ����õǸ� �����Ͱ� ���󰡴ϱ� �����Ҷ��� ���)

- ȸ�� Ŭ���� ���̾�׷�
  - ������ ���� ���踦 �������� �����ڵ��� ��üȭ�Ͽ� Ŭ���� ���̾�׷��� ����
  - interface�� ����ü���� ����
  - ���� ���� level
  - ������ �������� �ʰ� Ŭ�����鸸 �м��ؼ� �� �� �ִ� �׸�
  - ![class_diagram](./readme_img/class_diagram.JPG)
  - MemberService(����)(interface)
    - ȸ�� ����
    - MemberServiceImpl(����ü)
  - MemberRepository(����)(interface)
    - ȸ�� �����
    - MemoryMemberRepository(����ü)
    - DbMemberRepository(����ü)

- ȸ�� ��ü ���̾�׷�
  - ����ü���� ������ �㶧 �������� ������ ��. �̸� ǥ���ϰ��� ��.
  - ���� ������ �ö���� ��ü����(�޸� ����) �������� ��� �Ǵ��� �׸�����.
  - ![entity_diagram](./readme_img/entity_diagram.JPG)
  - Ŭ���̾�Ʈ�� ȸ�� ���񽺸� �ٶ� ��.
  - ȸ�� ����(��Ȯ���� ȸ�� ���� ����ü)�� �޸� ȸ�� ����Ҹ� �ٶ�.

- ���� ����
  - ������ -> Ŭ���� ���̾�׷� -> ��ü ���̾�׷�

---

### ȸ�� ������ ����

- ������ �ۼ��� ȸ�� Ŭ���� ���̾�׷��� �������� �����ϱ�.
- member package ����
  - Grade(enum)
    - ȸ�� ����� ��Ÿ����
    - BASIC, VIP
  - Member(Class, Entity)
    - 3���� �Ӽ��� ����
      - id, name, grade
      ```java
      private Long id;
      private String name;
      private Grade grade;
      ``` 
    - ������ �����
      ```java
      public Member(Long id, String name, Grade grade) {
        this.id = id;
        this.name = name;
        this.grade = grade;
      }
      ``` 
    - Getter & Setter ����
      - �����͸� �������� �ž��ִ� ����
      - Getter �� Setter�� ���� private�� ������ �������� �� �ִ�.  
  - MemberRepository(interface)
    ```java
    public interface MemberRepository {

      void save(Member member);

      Member findById(Long memberId);
    }
    ```
    - save()
      - ȸ�� ����
    - findById()
      - ȸ���� id�� ȸ���� ã�� ���
  - MemoryMemberRepository(����ü)
    - ������ ���� package���� ����ü���� ����γ� ������ �����ϱ� ���� member package�� �־��
    - ����ü�ϱ� �Ʒ��� ���� �ؾ���
      ```java
      public class MemoryMemberRepository implements MemberRepository
      ```
    - ����Ҵϱ� Map���� ����Ұ� �־����
      ```java
      private static Map<Long, Member> store = new HashMap<>();
      ```
      - HashMap<>()�� ���ü� �̽��� ���� �� �־ ����� ConcurrentHashMap�� ����Ѵ�.
    - save(Member member)
    - findById(Long memberId)
      - store���� get()�ؼ� �Ѿ�� memberId�� ������ ã�±��.
    - �̷��� �����ϰ� �޸𸮷� ����ϴ� db�� ������� ������ ������ �� �ִ�. ���� �޸𸮷θ� �����ϱ� ������ test�뵵�θ� ����Ѵ�.

  - MemberService(interface)
    - 2���� ����� ����.
    - join()
      - ȸ�� ����
    - findMember()
      - ȸ�� ��ȸ
  - MemberServiceImpl(����ü)
    - �������ϰ� ��ȸ�� �ҷ��� �ʿ��� ���� MemberRepository�̴�. �׷���, MemberRepository�� interface�̹Ƿ� ���� ��ü�� �����ؼ� �־������.
      ```java
      private final MemberRepository memberRepository = new MemoryMemberRepository();
      ``` 
    - ȸ�� ����
      ```java
      @Override
      public void join(Member member) {
        memberRepository.save(member);
      }
      ``` 
      - join()���� save()�� ȣ���ϸ� �������� ���ؼ� MemoryMemberRepository�� �ִ� save()�� ȣ���� �ȴ�.
    - ȸ�� ��ȸ
      ```java
      @Override
      public Member findMember(Long memberId) {
        return memberRepository.findById(memberId);
      }
      ``` 

---

### ȸ�� ������ ����� �׽�Ʈ

- ȸ�� ��ü ���̾�׷��� �׸��� �������.
- ��Ÿ�ӿ� ���� -> Ŭ���̾�Ʈ�� MemberServiceImpl�� ����ϰ� �� -> ȸ�� ���񽺴� �޸� ȸ�� ����Ҹ� ������.
- src/main/java/hello.core�� MemberApp ����
  - ���⼭ �ߵǴ��� test�� ����
  - MemberService�� ���� ����ü�� new MemberServiceImpl()�ؼ� ��������.
  - join() test
    - member�� �����ڸ� ���� ��ü ����
    - join(member)
    - memberService.findMember()�� ���� ������ ����� ã�� ����� �Ȱ����� ���ϴµ��� test�� �Ȱ���
  - �� ��Ĵ�� test�� ���� ������ �ڹ��ڵ�� �����Ѱ���(spring ����X)
  - �׷���, ���ø����̼� �������� main method�� test�ϴ°��� �Ѱ谡 ����.(���� ����� �ƴ�)
  - <strong>�׷���, Junit�̶�� test framework�� ����Ѵ�.</strong>

- test(junit)
  - src/test/java/hello.core/ �� member package ����
  - src/test/java/hello.core/member/ �� MemberServiceTest class ����
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
      - ~~�Ѱ͵��� �־�������
    - when
      - �̷��� ������
    - then
      - �䷸�� �ȴ�.
    - ����
      - Assertions(org.assertj.core.api)�� ���� �����ϸ� ��
  - join test�� �����ϸ� ������ ����� �� �� �ִ�.
  - ������ ���� �ڹ��ڵ�� �����ϸ� ������ ����(��µ� ����� ���鼭) �����߾�����, junit���� �����ϸ� ��µ� ����� ���� ���鼭 �����ϴ� ���� �ƴ϶� ����, ������ ������ �ٷ� Ȯ�� �����ϴ�.
  - test code �ۼ��� �ʼ����̴�.

- ȸ�� ������ ������ ������
  - �ٸ� ����ҷ� ������ �� OCP ��Ģ�� �ؼ����� ����.
  - DIP ��Ģ�� �ؼ����� ����.
  - ��, <strong>�������谡 �������̽� �Ӹ� �ƴ϶� �������� ��� �����ϴ� �������� ����</strong>
    - �ڵ忡���� �Ʒ� �κ��� ����ü�� �����ϴ� �κ��̴�.
    ```java
    public class MemberServiceImpl implements MemberService{
      private final MemberRepository memberRepository = new MemoryMemberRepository();
      ...
      ...
      ...
    ``` 
      - ���� MemberRepository��� interface�� ������ ������, �ڿ� ���� �Ҵ��ϴ� �κ��� new MemoryMemberRepository()�κп��� ����ü�� �����Ѵ�.
      - �׷��� MemberServiceImpl�� MemberRepository(�߻�ȭ) �Ӹ� �ƴ϶� MemoryMemberRepository(��üȭ)�� �����Ѵ�.

---

### �ֹ��� ���� ������ ����

- �ֹ��� ���� ��å(only ���ҿ� ���� �׸�)
  - [����Ͻ� �䱸���װ� ����](#����Ͻ�-�䱸���װ�-����) ���� �ֹ��� ���� ��å Ȯ���ϰ� ����.
- �ֹ� ������ ����, ����, å��
  - ![order_domain](./readme_img/order_domain.JPG)
  - `Ŭ���̾�Ʈ`�� �ֹ� ������ �� �� ����.
    - Ŭ���̾�Ʈ�� Spring MVC���� Controller�� �� ��.
  - `�ֹ� ���� ����`�� �ֹ� ������ ������ ��.
    - ȸ�� ����� �ʿ��ϱ� ������ `ȸ�� ����� ����`���� ȸ�� ��ȸ�ؼ�,
    - �� ȸ���� ����� ������ `���� ��å ����`���ٰ� �����, ������ ����� �ֹ� ���� ���ҿ��ٰ� �������ְ�,
  - `�ֹ� ���� ����`�� ���������� ������ ����� ����� `Ŭ���̾�Ʈ`���� ��ȯ�Ѵ�.
  - ����: �����δ� �ֹ� �����͸� DB�� �����ϰ�����, ������ �ʹ� ������ �� �� �־ �����ϰ�, �ܼ��� �ֹ� ����� ��ȯ.

- �ֹ� ������ ��ü(���� + ������ ���� �׸�)
  - ![all_order_domain](./readme_img/all_order_domain.JPG)
  - �� �׸��� �� ���� `����` ���� �����, `����`�� �� ������ ����.
    - `����`�� `����`�� �и��߱� ������, �����Ӱ� `���� ��ü`�� ������ �� �ְ� ���谡 �ȰŴ�.(�����ϰ� ���� ����)

- �ֹ� ������ Ŭ���� ���̾�׷�
  - ������ ���� �׸��� ������ �Ʒ��� ���� Ŭ���� ���̾�׷� ����.
  - ![order_domain_class](./readme_img/order_domain_class.JPG)

- �ֹ� ������ ��ü ���̾�׷�1
  - Ŭ���� ���̾�׷��� �ٸ��� ���� ���� ���ø����̼��� ������ �������� ��ü���� �������谡 �ξ����� �׸�
  - ![order_domain_entity1](./readme_img/order_domain_entity1.JPG)
  - `Ŭ���̾�Ʈ`�� `�ֹ� ���� ����ü`�� ȣ���ϸ�, `�޸� ȸ�� �����`�� ȣ�� + `���� ���� ��å`�� ȣ���Ѵ�.
  - ��, ȸ���� �޸𸮿��� ��ȸ�ϰ�, ���� ���� ��å(���� �ݾ�)�� �����ص� �ֹ� ���񽺸� �������� �ʾƵ� �ȴ�. ���ҵ��� ���� ���踦 �״�� ���� �� �� �ִ�.

- �ֹ� ������ ��ü ���̾�׷�2
  - ![order_domain_entity2](./readme_img/order_domain_entity2.JPG)
  - ���߿� �ٲ�� ����ü�� ���Ͱ��� �ٲ㼭 ����� ��.
  - ȸ���� �޸𸮰� �ƴ� ���� DB���� ��ȸ�ϰ�, ���� ���� ��å(�޹� �ݾ׿� ���� % ����)�� �����ص� �ֹ� ���񽺸� �������� �ʾƵ� �ȴ�.
  - ����, <strong>���� ���踦 �״�� ���� �� �� �ִ�.</strong>

---

### �ֹ��� ���� ������ ����

- discount ���� ����
  - src/main/java/hello.core/discount package ����
  - DiscountPolicy interface ����
    - ���� ��� �ݾ��� ��ȯ����
  - FixDiscountPolicy Class ����(����������å ����ü)
    ```java
    private int discountFixAmount = 1000; // 1000�� ����

    @Override
    public int discount(Member member, int price) {
      if (member.getGrade() == Grade.VIP){
          return discountFixAmount;
      }else{
          return 0;
      }
    }
    ``` 
    - VIP�� 1000�� ����, �� �ܴ� 0�� ����
- order ���� ����
  - src/main/java/hello.core/order package ����
  - Order class ����
    - �ֹ����� ������ �� ������ ��������� ��ü
    - field�� memberId, itemName, itemPrice,discountPrice(���� �ݾ�)
    - �� ��, ������ ����
    - �׸���, getter, setter ����
    - calculatePrice()(��� ����)
      ```java
      public int calculatePrice(){
        return itemPrice - discountPrice;
      }
      ``` 
    - toString()
      - Generate->toString()�ؼ� ����
      - ���ϰ� ��ü�� �����͸� ���� ���ؼ� ����
      - ��ü�� ����ϸ� toString()�� ����� ����

  - OrderService interface ����
    - createOrder()
      - OrderService���� �ֹ��� �����Ҷ� ȸ�� id, ��ǰ��, ��ǰ ������ �Ķ���ͷ� �Ѱܾ���. �׷���, return���� �ֹ� ����� ��ȯ�Ѵ�.

  - OrderServiceImpl class ����
    - OrderService�� MemberRepository���� ȸ���� ã�ƾ��ϰ�, DiscountPolicy�� �ʿ���.
      ```java
      private final MemberRepository memberRepository = new MemoryMemberRepository();
      private final DiscountPolicy discountPolicy = new FixDiscountPolicy();
      ```
       
    - createOrder����
      ```java
      @Override
      public Order createOrder(Long memberId, String itemName, int itemPrice) {
        Member member = memberRepository.findById(memberId);
        int discountPrice = discountPolicy.discount(member, itemPrice);

        return new Order(memberId, itemName, itemPrice, discountPrice);
      }
      ```
      - OrderService ���忡���� ���ο� ���ؼ��� �� ������ ���ο� ���� �κ��� discountPolicy�� �˾Ƽ� ���ְ� �׿� ���� ����� ����.
        - ���� ü�� ��Ģ�� �� ��Ŵ
        - ����, ���ο� ���� ������ �ʿ��ϸ� ���� �κи� ��ġ�� ��.(�ֹ������� �Ȱǵ鿩�� ��.)

---

### �ֹ��� ���� ������ ����� �׽�Ʈ

�ֹ��� ���ϴ´�� �����ϴ��� main method �����غ�.(���� ���� ����� �ƴ�.)
- src/main/java/hello.core/order/OrderApp class ����
  - ������ VIP member�� �����ϰ� �̸� �޸�DB�� �־���(�׷��� �ֹ����� ã�� �� �� �����ϱ�)
    ```java
    Long memberId = 1L;
    Member member = new Member(memberId, "memberA", Grade.VIP);
    memberService.join(member);
    ``` 
  - createOrder�� ���� 10000��¥�� itemA�� memberId�� order�� ������.
    ```java
    Order order = orderService.createOrder(memberId,"itemA",10000);
    ```
  - order�� ����ϸ� Order Class�� toString���� ���� �Ʒ��� ���� ��¹��� ���´�.
    - ![print_order](./readme_img/print_order.JPG)
    <br/>


junit�� ���� test�ϱ�
- ���� ���� ����ϰ� ����� ��.
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
  - @Test �������.
  - sysout ��� Assertions���� Ȯ��.

- ���� test�� �� ����� ���� �߿���.
  - ���� test�� spring�̳� �����̳��� ���� ���� �����ϰ� �ڹ��ڵ�� test�� �ϴ� ��.


---
---

## ������ �ٽ� ���� ����2 - ��ü ���� ���� ����

---
---

### ���ο� ���� ��å ����

>���� ��å�� �������αݾ�(VIP�� 1000�� ����)���ٴ� �ֹ� �ݾ״� ����% �������� �ٲٰ��� �Ѵ�.

- ������ ����Ʈ���� ���� ����
  >������ �������� `���ΰ� ��ȣ�ۿ�`��<br> 
  �������� �������� `�۵��ϴ� ����Ʈ����`��<br> 
  �Ծ� ���󺸴� `������ ����`��<br> 
  ��ȹ�� �����⺸�� `��ȭ�� �����ϱ�`��<br> 
  ��ġ �ְ� �����.

- RateDiscountPolicy ����
  - ![ratediscount](./readme_img/ratediscount.JPG)
  - �Ʒ��� ���� �ϴ� �ۼ�
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

- RateDiscountPolicyTest ����
  - �Ʒ��� ���� �ڵ� �ۼ�(���� test)
  ```java
  @Test
  @DisplayName("VIP�� 10% ������ ����Ǿ�� �Ѵ�")
  void vip_o(){
    //given
    Member member = new Member(1L, "memberVIP", Grade.VIP);
    //when
    int discount = discountPolicy.discount(member, 10000);
    //then
    Assertions.assertThat(discount).isEqualTo(1000);
  }
  ``` 
  - @DisplayName() : junit5���� ���� �����ϸ� test ���� ����� vip_o ��� ��ȣ�ȿ� ���� ���ڷ� ����.
  - test�� �Ҷ����� `���� test`�� �߿��ϳ� `���� test`�� �߿��ϴ�.
  - �Ʒ��� ���� �ڵ� �ۼ�(���� test)
  ```java
  @Test
  @DisplayName("VIP�� �ƴϸ� ������ ������� �ʾƾ� �Ѵ�")
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

### ���ο� ���� ��å ����� ������

- ������ ���� ���ο� ���� ��å�� ������ �ҷ��� OrderServiceImpl�� �� �Ʒ��� ���� �ڵ带 ���ľ��Ѵ�.
  ```java
  //private final DiscountPolicy discountPolicy = new FixDiscountPolicy();
  private final DiscountPolicy discountPolicy = new RateDiscountPolicy();
  ...
  ...
  ```
  - ���� ��å�� �����ҷ��� Ŭ���̾�Ʈ�� `OrderServiceImpl` �ڵ带 ���ľ� �Ѵ�.

- ������ `������`�� �߰���!!
  - ���Ұ� ���� �и� O
  - ������ Ȱ��, �������̽��� ���� ��ü �и� O
  - OCP, DIP�� ���� ��ü���� ���� ��Ģ �ؼ�? X
    - �׷��� �������� �ƴ�!
  - DIP: �ֹ����� Ŭ���̾�Ʈ `OrderServiceImpl`�� �������̽�(�߻�)�Ӹ� �ƴ϶� `����ü Ŭ�������� ����`�ϰ� �ִ�.
    - interface ���� : `DiscountPolicy`
    - ����ü ���� : `FixDiscountPolicy`, `RateDiscountPolicy`
    - ���� ���� ����
      ![real](./readme_img/real.JPG)
  - OCP : �������� �ʰ� Ȯ���ؾ���
    - ���� �ڵ�� `����� Ȯ���ؼ� ����`�ϸ�, `Ŭ���̾�Ʈ �ڵ忡 ������ ��`.
    - ��å ����
      ![change_policy](./readme_img/change_policy.JPG)

<br/>
<strong> ���� ���� ������ ��� �ذ��� �� ������?</strong><br/>

- `�������̽����� �����ϵ��� ���踦 ��������`
  - ![only_interface](./readme_img/only_interface.JPG)
  - �Ʒ��� ���� �ڵ� ����
  ```java
  //private final DiscountPolicy discountPolicy = new FixDiscountPolicy();
  //private final DiscountPolicy discountPolicy = new RateDiscountPolicy();
  private DiscountPolicy discountPolicy;
  ``` 
  - DiscountPolicy�� interface�̴�. ��, OrderServiceImpl�� �߻�ȭ�� DiscountPolicy���� �����Ѵ�.

- ���� ���� �ڵ带 ������ ��, OrderServiceTest�� ������ `NullPointerException`�� �߻�
  - ����ü ���� �������̽��� ������ ���ȱ� ����.

<strong>�ذ� ���</strong>

- ������ Ŭ���̾�Ʈ�� `OrderServiceImpl`�� `DiscountPolicy`�� ���� ��ü�� ��� �����ϰ� �������־�� �Ѵ�.

---


---
---

## IntelliJ ����Ű ������ & ����
- �⺻������ Preferences -> keymap ���� �� �� ������ ����ϰ����ϴ� ����Ű �̸��� �Է��ϸ� ȯ�濡 �°�(window,mac..) ����Ű�� ����
- Preferences(or Settings) �ٷΰ��� : ctrl+alt+s
- Generate(������,Getter,Setter ��...) : alt+insert (������ ��� alt+function+delete)
- Compact middle Package
- �ڵ��ϼ�(�����ݷб��� �����ؼ�) : ctrl+shift+enter
- public static void main(String[] args) ���� : psvm + enter
- �� �����ؼ� ������ �ֱ� : ctrl+alt+v
- Print a value to System.out : soutv+enter
- main������ �Լ����� test �ٷ� �����ϱ�: ctrl+shift+t
- test�� �Ҷ� Assertions�� static import�ϴ°� ���� : Assertions Ŀ�� �ΰ� +alt+enter+(on demand static~~)

---
---

## ����(�ٷΰ���)

- [������ �ٽ� ���� - �⺻��](#������-�ٽ�-����---�⺻��)
  - [��ü ���� ����� ������](#��ü-����-�����-������)
    - [�̾߱� - �ڹ� ������ �߿� �ܿ�� �������� ź��](#�̾߱�---�ڹ�-������-�߿�-�ܿ��-��������-ź��)
    - [�������̶�?](#�������̶�)
    - [���� ��ü ���� ���α׷���?](#����-��ü-����-���α׷���)
    - [���� ��ü ���� ������ 5���� ��Ģ(SOLID)](#����-��ü-����-������-5����-��Ģsolid)
    - [��ü ���� ����� Spring](#��ü-����-�����-spring)
  - [������ �ٽ� ���� ����1 - ���� �����](#������-�ٽ�-����-����1---����-�����)
    - [������Ʈ ����](#������Ʈ-����)
    - [����Ͻ� �䱸���װ� ����](#����Ͻ�-�䱸���װ�-����)
    - [ȸ�� ������ ����](#ȸ��-������-����)
    - [ȸ�� ������ ����](#ȸ��-������-����)
    - [ȸ�� ������ ����� �׽�Ʈ](#ȸ��-������-�����-�׽�Ʈ)
    - [�ֹ��� ���� ������ ����](#�ֹ���-����-������-����)
    - [�ֹ��� ���� ������ ����](#�ֹ���-����-������-����)
    - [�ֹ��� ���� ������ ����� �׽�Ʈ](#�ֹ���-����-������-�����-�׽�Ʈ)
  - [������ �ٽ� ���� ����2 - ��ü ���� ���� ����](#������-�ٽ�-����-����2---��ü-����-����-����)
    - [���ο� ���� ��å ����](#���ο�-����-��å-����)
    - [���ο� ���� ��å ����� ������](#���ο�-����-��å-�����-������)
  - [IntelliJ ����Ű ������ & ����](#intellij-����Ű-������--����)
  - [����(�ٷΰ���)](#�����ٷΰ���)

- [������ �ٽ� ���� - �⺻��](#������-�ٽ�-����---�⺻��)
  - [��ü ���� ����� ������](#��ü-����-�����-������)
    - [�̾߱� - �ڹ� ������ �߿� �ܿ�� �������� ź��](#�̾߱�---�ڹ�-������-�߿�-�ܿ��-��������-ź��)
    - [�������̶�?](#�������̶�)
    - [���� ��ü ���� ���α׷���?](#����-��ü-����-���α׷���)
    - [���� ��ü ���� ������ 5���� ��Ģ(SOLID)](#����-��ü-����-������-5����-��Ģsolid)
    - [��ü ���� ����� Spring](#��ü-����-�����-spring)
  - [������ �ٽ� ���� ����1 - ���� �����](#������-�ٽ�-����-����1---����-�����)
    - [������Ʈ ����](#������Ʈ-����)
    - [����Ͻ� �䱸���װ� ����](#����Ͻ�-�䱸���װ�-����)
    - [ȸ�� ������ ����](#ȸ��-������-����)
    - [ȸ�� ������ ����](#ȸ��-������-����)
    - [ȸ�� ������ ����� �׽�Ʈ](#ȸ��-������-�����-�׽�Ʈ)
    - [�ֹ��� ���� ������ ����](#�ֹ���-����-������-����)
    - [�ֹ��� ���� ������ ����](#�ֹ���-����-������-����)
    - [�ֹ��� ���� ������ ����� �׽�Ʈ](#�ֹ���-����-������-�����-�׽�Ʈ)
  - [������ �ٽ� ���� ����2 - ��ü ���� ���� ����](#������-�ٽ�-����-����2---��ü-����-����-����)
    - [���ο� ���� ��å ����](#���ο�-����-��å-����)
    - [���ο� ���� ��å ����� ������](#���ο�-����-��å-�����-������)
  - [IntelliJ ����Ű ������ & ����](#intellij-����Ű-������--����)
  - [����(�ٷΰ���)](#�����ٷΰ���)