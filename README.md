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

### ���ɻ��� �и�

>�߿�

- ���ø����̼��� �ϳ��� �����̶�� �����غ���
  - ������ `�������̽�` == `�迪(��� ����)`
  - �� �迪�� �´� `��츦 ����`�ϴ� ���� `����`�ϴ°�?
  - �迪�� ���ϴ� ���� ������ ���ϴ°� �ƴ� `���� ��ȹ��`�� ���ϴ� �Ŵ�.
  - ���� �ڵ�� ��ġ `�ι̿� ����(�������̽�)`�� �ϴ� `���������� ��ī������(����ü,���)`�� `�ٸ��� ����(�������̽�)`�� �ϴ� `���� ���ΰ�(����ü, ���)`�� ���� �ʺ��ϴ� �Ͱ� ����.

  - `OrderServiceImpl`�� `OrderService�� ���õ� ������ `�ؾ��ϴµ�, discountPolicy�� �ڱⰡ ���� ���ñ��� ��.(���ɻ� �и� X)

`���ɻ縦 �и�����`(���� ��ȹ�ڸ� �����, ���� ���� ��ȹ���� å���� Ȯ���� �и�����.)

<strong>AppConfig ����</strong>

- ���ø����̼��� ��ü ���� ����� ����(or ����)(config)�ϱ� ����, <strong>���� ��ü�� ����</strong>�ϰ�, <strong>����</strong>�ϴ� å���� ������ ������ ���� Ŭ������ ������.
  - src/main/java/hello.core/AppConfig class ����

- MemberServiceImpl class�� ���� �ڵ带 �Ʒ��� ���� ����
  ```java
  //private final MemberRepository memberRepository = new MemoryMemberRepository();
  private final MemberRepository memberRepository;

  public MemberServiceImpl(MemberRepository memberRepository) {
    this.memberRepository = memberRepository;
  }
  ``` 
  - �����ڸ� ���ؼ� �� MemberRepositoryImpl�� ���� ������ ������.
- AppConfig class���� �Ʒ��� ���� �ڵ� �ۼ�.
  ```java
  public MemberService memberService(){
    return new MemberServiceImpl(new MemoryMemberRepository());
  }
  ``` 
  - ��𼱰� `AppConfig`�� ���ؼ� `memberService`�� �ҷ��� ����Ѵ�.
  - �׷���, `MemberService` ����ü ��ü�� ������ �Ǵµ�, �� �� `MemoryMemberRepository`�� ����.
- ���� ���� �ڵ带 ������ ���, `MemberServiceImpl`�� `MemoryMemberRepository`(�� ����ü)�� ���� �ڵ�� ��������!
  - ��, `�߻�ȭ���� �����Ѵ�`

-  ���� ���� ������ `������ ����`�̶�� �Ѵ�.
   -  �����ڸ� ���ؼ� ��ü�� ����

- ���������� OrderService�� �ٲ��ش�.
  - `OrderServiceImpl`�� ����ϴ� field�� 2���̴�.
    - `MemberRepository`,`DiscountPolicy`
  - `OrderServiceImpl` �ڵ� ����
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
  - `AppConfig` �ڵ� �߰�
    ```java
    public OrderService orderService(){
      return new OrderServiceImpl(new MemoryMemberRepository(), new FixDiscountPolicy());
    }
    ``` 
  - `AppConfig`�� ���ؼ� �������� OrderService�� ��ȸ�ϸ� `OrderServiceImpl`�� ��ȯ�� �Ǵµ� �ű⿡ `MemoryMemberRepository`�� `FixDiscountPolicy`�� ����.
  - �׷���, `OrderServiceImpl`�� �������̽����� �����ϰ� �ȴ�.

- `AppConfig`�� ���ø����̼��� ���� ���ۿ� �ʿ��� <strong>���� ��ü�� ����</strong>�Ѵ�.
  - `MemberServiceImpl`
  - `MemoryMemberRepository`
  - `OrderServiceImpl`
  - `FixDiscountPolicy`
- `AppConfig`�� ������ ��ü �ν��Ͻ��� ������ <strong>�����ڸ� ���ؼ� ����(����)</strong> ���ش�.
  - `MemberServiceImpl` -> `MemoryMemberRepository`
  - `OrderServiceImpl` -> `MemoryMemberRepository`, `FixDiscountPolicy`

����
- ���� �������� `MemberServiceImpl`�� `MemoryMemberRepository`�� �������� �ʴ´�!
- ���� `MemberRepository` interface���� ����.
- `MemberServiceImpl` ���忡�� `������`�� ���� � ���� ��ü�� ������(���Ե���)�� �� �� ����.
- `MemberServiceImpl�� ������`�� ���ؼ� � ���� ��ü�� ���������� ���� �ܺ� `AppConfig`���� ����.
- `MemberServiceImpl`�� �������� <strong>�������迡 ���� ����� �ܺ�</strong>�� �ñ�� <strong>���࿡�� ����</strong>�ϸ� �ȴ�.

Ŭ���� ���̾�׷�
![class_diagram2](./readme_img/class_diagram2.JPG)
- `MemberService`�� interface�̴�. 
- �� interface�� �����ϴ� ���� `MemberServiceImpl`�̴�.
- �� `MemberServiceImpl`�� `MemberRepository`��� interface�� �����Ѵ�.
- `AppConfig`�� `MemberServiceImpl`�� `MemoryMemberRepository`�� �����Ѵ�.
- �׷����Ͽ�, ��ü�� ������ ������ `AppConfig`�� ����Ѵ�.
- <strong>DIP �ϼ�</strong>
  - `MemberServiceImpl`�� `MemberRepository`�� �߻󿡸� �����ϸ� �ȴ�. ���� ����ü Ŭ������ ���� ��.
- <strong>���ɻ� �и�</strong>
  - ��ü�� �����ϰ� �����ϴ� ����(Config)�� �����ϴ� ����(Impl)�� ��Ȯ�� �и�.

ȸ�� ��ü �ν��Ͻ� ���̾�׷�
![instance_diagram](./readme_img/instacne_diagram.JPG)
- `AppConfig`�� `MemoryMemberRepository` ��ü�� ����.
- �� ����, `MemberServiceImpl`�� ������ ��, `MemoryMemberRepository`�� ���� ���� ���� �����ڿ� �Ѱ���.
- �׸��Ͽ�, `MemberServiceImpl`�� ������ `MemoryMemberRepository`�� ���� ���� ������ �ް� ��.

- <strong>DI(Dependency Injection)</strong>
  - Ŭ���̾�Ʈ�� `MemberServiceImpl`�� ���忡�� ���� �������踦 ��ġ �ܺο��� �������ִ� �� ���ٰ��Ͽ� `�������� ����` �Ǵ� `������ ����`�̶�� �Ѵ�.

`AppConfig` ����

- `MemberApp` �ڵ� ����
  ```java
  public static void main(String[] args) {
    AppConfig appConfig = new AppConfig();
    MemberService memberService = appConfig.memberService();
    //MemberService memberService = new MemberServiceImpl();
    ...
    ...
  }
  ``` 
  - �׷��� `AppConfig`�� �� `MemberServiceImpl`�� ����� ���� ���� `MemberServiceImpl`�� `MemoryMemberRepository` �� ����Ѵٴ� �ǹ̷� ��������.
    ```java
    public class AppConfig {

    public MemberService memberService(){
      return new MemberServiceImpl(new MemoryMemberRepository());
    }
    ```

- `OrderApp` �ڵ� ����
  ```java
  AppConfig appConfig = new AppConfig();
  MemberService memberService = appConfig.memberService();
  OrderService orderService = appConfig.orderService();
  ``` 
- MemberApp�� OrderApp test�� �����غ��� ���� �����ϴ� ����� �� �� �ִ�.

Test �ڵ� ����
- `MemberServiceTest`�� �Ʒ��� ���� ����
  ```java
  //MemberService memberService = new MemberServiceImpl();
  MemberService memberService;

  @BeforeEach
  public void beforeEach(){
    AppConfig appConfig = new AppConfig();
    memberService = appConfig.memberService();
  }
  ``` 
  - ������ �ϱ� ���� `AppConfig`�� �����, `memberService`�� �Ҵ����ش�. �� ��, test�� ���ư���. 
- ���������� `OrderServiceTest`�� ����
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

#### ����
- `AppConfig`�� ���ؼ� ���ɻ縦 �и�.
- �迪, ��츦 �����غ���.
- `AppConfig`�� ���� ��ȹ��
- `AppConfig`�� ����ü Ŭ������ ����.(��࿡ �´� ��� ��� ����). ���ø����̼��� ��� �����ؾ� ���� ��ü ������ å����.
- ���� �� ����ü����(�� ������) ��� ��ɵ��� �����ϴ� å�Ӹ� ���� ��.
- `OrderServiceImpl`�� ����� �����ϴ� å�Ӹ� ���� ��.

---

### AppConfig �����͸�

���� `AppConfig`�� ���� <strong>�ߺ�</strong>�� �ְ�, <strong>����</strong>�� ���� <strong>����</strong>�� �� �Ⱥ��δ�.(���� ���� �����ϱ�...)(���ҵ��� �巯���� �ϴ°� �߿���.)

- `AppConfig`�� �Ʒ��� ���� ����.
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
- `AppConfig`���� method �̸��� ���ؼ� ���ҵ��� ���� �巯��.
  - `MemberService`,`MemberRepository`,`OrderService`,`DiscountPolicy`
- `memberService`�� `MemberServiceImpl`�� ����ҰŴ�.
- `memberRepository`�� ���Ѱ��� `MemoryMemberRepository`�� ����ҰŴ�.
- 'orderService'�� ���� ��ü���� ���� ���� �� application���� `memberRepository`���� ���� ��������, ���� �� application���� `discountPolicy`���� ���� �����´�.
- `discountPolicy`�� ���� ���� `FixDiscountPolicy`�� ����ҰŴ�.

- ![config](./readme_img/config.JPG)
  - �׸��Ͽ� ���迡 ���� �׸��� Config�� �״�� �巯���� �ȴ�.(���� + ������ �� ���� ����)

- `new MemoryMemberRepository()` �� �κ��� �ߺ� ���ŵǾ���. ���� `MemoryMemberRepository`�� �ٸ� ����ü�� ������ �� �� �κи� �����ϸ� �ȴ�.
- `AppConfig`�� ���� ���Ұ� ���� Ŭ������ �Ѵ��� ���´�. ���ø����̼� ��ü ������ ��� �Ǿ��ִ��� ������ �ľ��� �� �ִ�.

---

### ���ο� ������ ���� ��å ����

���� ���� ��å(FixDiscountPolicy) -> ���� ���� ��å(RateDiscountPolicy)�� ����

- `AppConfig`�� ��������, ���ø����̼��� ũ�� `��� ����`�� `��ü�� �����ϰ� ����(Configuration) ����`���� �и�.
- ������ `AppConfig`�� �����ϸ� ��.
- ���, ������ �и� 
  - ![use_config](./readme_img/use_config.JPG)
- ���� ��å ����
  - ![change](./readme_img/change.JPG)

- `Appconfig`���� �Ʒ��� ���� �ڵ� ����
  ```java
  public DiscountPolicy discountPolicy(){
    //return new FixDiscountPolicy();
    return new RateDiscountPolicy();
  }
  ``` 
- ������ ���� ��å�� �����ص�, ���ø����̼��� ���� ������ ����ϴ� `Appconfig`�� �����ϸ� ��. Ŭ���̾�Ʈ �ڵ��� `OrderServiceImpl`�� �����ؼ� `��� ����`�� � �ڵ嵵 ������ �ʿ䰡 ����.

- `���� ����(AppConfig)`�� �翬�� ������ ��.

---

### ���� ��ü ���� ������ 5���� ��Ģ�� ����

���⼭�� SRP, DIP, OCP ����

SRP ���� å�� ��Ģ
>�� Ŭ������ �ϳ��� å�Ӹ� ������ �Ѵ�.
- SRP�� �����鼭 ���ɻ縦 �и�.
- ���� ��ü�� �����ϰ� �����ϴ� å���� `Appconfig`�� ���.
- `Ŭ���̾�Ʈ ��ü`�� �����ϴ� å�Ӹ� ���.

DIP �������� ���� ��Ģ
>���α׷��Ӵ� "�߻�ȭ�� �����ؾ���, ��üȭ�� �����ϸ� �ȵȴ�." ������ ����(DI)�� �� ��Ģ�� ������ ��� �� �ϳ���.
- `Ŭ���̾�Ʈ �ڵ�`�� `DiscountPolicy` �߻�ȭ �������̽����� �����ϵ��� �ڵ带 �����ؾ���.
- ������, Ŭ���̾�Ʈ �ڵ�� �������̽������δ� �ƹ��͵� ������ �� ����.(NullPointerException)
- `Appconfig`�� `FixDiscountPolicy` ��ü �ν��Ͻ��� `Ŭ���̾�Ʈ �ڵ�` ��� �����ؼ� `Ŭ���̾�Ʈ �ڵ�`�� �������踦 �����ߴ�.
- �̷����ؼ� DIP ��Ģ�� �����鼭 ���� �ذ�.

OCP
>����Ʈ���� ��Ҵ� Ȯ�忡�� ���� ������ ���濡�� ���� �־�� �Ѵ�.
- ������ ��� + `Ŭ���̾�Ʈ`�� DIP�� ��Ŵ ==> OCP�� ���� �� ���ɼ��� ����.
- `���ø����̼�` = `��� ����` + `���� ����`
- `Appconfig`�� �������踦 �����ؼ� `Ŭ���̾�Ʈ �ڵ�`�� �����ϹǷ� `Ŭ���̾�Ʈ �ڵ�`�� �������� �ʾƵ� ��.
- **����Ʈ���� ��Ҹ� ���Ӱ� Ȯ���ص� ��� ������ ������ ���� �ִ�**

---

### IoC, DI, �׸��� �����̳�

**������ ���� IoC(Inversion of Control)**
- ���� ȣ���ϴ� ���� �ƴ�, �����ӿ�ũ ���� �͵��� �� �ڵ带 ��� ȣ�����ִ� ��.(��ġ ������� �ڹٲ�� ����, ������ �����̶�� ��)
- `AppConfig`�� ������ ����, ���� ��ü�� �ڽ��� ������ �����ϴ� ���Ҹ� ����ϰ�, ���α׷��� ���� �帧�� ���� `AppConfig`�� ��������.
  - ex> `OrderServiceImpl`�� �ʿ��� �������̽����� ȣ�������� � ���� ��ü���� ������� �𸥴�.
- ���α׷��� ���� ���� �帧�� ���� ������ ��� `AppConfig`�� ������ �ִ�. ������ `OrderServiceImpl`�� `AppConfig`�� �����Ѵ�. �׸��� `AppConfig`�� `OrderServiceImpl`�� �ƴ� `Orderservice` �������̽��� �ٸ� ���� ��ü�� �����ϰ� ������ �� �� �ִ�. �׷� ��ǵ� ��ü `OrderServiceImpl`�� ������ �ڽ��� ������ ������ �� �̴�.
- �̷��� ���α׷��� ���� �帧�� ���� �����ϴ� ���� �ƴ϶� �ܺο��� �����ϴ� ���� `������ ����(IoC)`�̶� �Ѵ�.

**�����ӿ�ũ vs ���̺귯��**
- **�����ӿ�ũ**�� **���� �ۼ��� �ڵ带 ����**�ϰ�, **��� ����**�ϸ� �װ��� �����ӿ�ũ�� �´�.
  - ex> JUnit
- �ݸ鿡 **���� �ۼ��� �ڵ�**�� **���� ������ �帧�� ���**�Ѵٸ� �װ��� �����ӿ�ũ�� �ƴ϶� **���̺귯��**��.
  - ex> �ڹ� ��ü�� Json or xml �ٲܶ�, �� ���̺귯���� �ҷ��ٰ� ���� ȣ���ϴ� ��

**�������� ���� DI(Dependency Injection)**
- `OrderServiceImpl`�� `DiscountPolicy` �������̽��� �����Ѵ�. ���� � ���� ��ü�� �������� �𸥴�.
- ��������� **������ Ŭ���� ���� ����**�� **���� ������ �����Ǵ� ������ ��ü(�ν��Ͻ�) ���� ����** ���� �и��ؼ� �����ؾ� �Ѵ�.

  **������ Ŭ���� ��������**
  
  - Ŭ������ ����ϴ� import �ڵ常 ���� �������踦 ���� �Ǵ��� �� �ִ�.
  - ������ ��������� ���ø����̼��� �������� �ʾƵ� �м� ����.
  - IntelliJ������ `hello.core` ��Ŭ�� -> Diagrams -> show Diagram... -> Java Classes -> ���� ��Ŭ�� -> Show Dependencies Ŭ�� �ϸ� �������迡 ���� diagrams�� ����(����)
    ![show_dependencies](./readme_img/show_dependencies.JPG)
  - Ŭ���� ���̾�׷�
    - ![all_class_diagram](./readme_img/all_class_diagram.JPG)
  - �׷���, �̷��� Ŭ���� �������� �����δ� ���� � ��ü�� `OrderServiceImpl`�� ���� ���� �� �� ����.(���� ������Ѻ��� �� �� �ִ�.)

  **������ ��ü �ν��Ͻ� ���� ����**

  - ���ø����̼� ���� ������ ���� ������ ��ü �ν��Ͻ��� ������ ����� ���� ����.
  - ��ü ���̾�׷�
    - ![all_entity_diagram](./readme_img/all_entity_diagram.JPG)
  - ���ø����̼� **���� ����(��Ÿ��)** �� �ܺο��� ���� ���� ��ü�� �����ϰ� Ŭ���̾�Ʈ�� �����ؼ� Ŭ���̾�Ʈ�� ������ ���� �������谡 ���� �Ǵ� ���� **�������� ����**�̶�� �Ѵ�.
  - ��ü �ν��Ͻ��� �����ϰ�, �� �������� �����ؼ� ����.
  - �������� ������ ����ϸ� 
    - Ŭ���̾�Ʈ �ڵ带 �������� �ʰ�, Ŭ���̾�Ʈ�� ȣ���ϴ� ����� Ÿ�� �ν��Ͻ��� ������ �� �ִ�.
    - ������ Ŭ���� �������踦 �������� �ʰ�, ������ �ν��Ͻ� �������踦 ���� ������ �� �ִ�.
  
**IoC �����̳�, DI �����̳�**
- `AppConfig`ó�� ��ü�� �����ϰ� �����ϸ鼭 �������踦 ������ �ִ� ���� IoC �����̳� �Ǵ� **DI �����̳�** ��� ��.
- �Ǵ�, �����(application ��ü�� ���� ������ �Ѵٰ� �Ͽ�), ������Ʈ ���丮(object�� ����� ���ٰ� �Ͽ�) ������ �Ҹ��⵵ �Ѵ�.


---

### ���������� ��ȯ�ϱ�

���ݱ��� ������ �ڹ� �ڵ常���� DI�� ������.

`Appconfig` �ڵ� ����
- ���� �ڵ�
  ```java
  public class AppConfig {

    public MemberService memberService(){
      return new MemberServiceImpl(memberRepository());
    }

    public MemberRepository memberRepository() {
      return new MemoryMemberRepository();
    }

    public OrderService orderService(){
      return new OrderServiceImpl(memberRepository(), discountPolicy());
    }

    public DiscountPolicy discountPolicy(){

      //return new FixDiscountPolicy();
      return new RateDiscountPolicy();
    }
  }
  ``` 
- �ٲ� �ڵ�
  ```java
  @Configuration
  public class AppConfig {

    @Bean
    public MemberService memberService(){
      return new MemberServiceImpl(memberRepository());
    }
    @Bean
    public MemberRepository memberRepository() {
      return new MemoryMemberRepository();
    }

    @Bean
    public OrderService orderService(){
      return new OrderServiceImpl(memberRepository(), discountPolicy());
    }

    @Bean
    public DiscountPolicy discountPolicy(){
      //return new FixDiscountPolicy();
      return new RateDiscountPolicy();
    }
  }
  ``` 

`MemberApp` �ڵ� ����
- ���� �ڵ�
  ```java
  public static void main(String[] args) {

    AppConfig appConfig = new AppConfig();
    MemberService memberService = appConfig.memberService();
    //MemberService memberService = new MemberServiceImpl();
    Member member = new Member(1L, "memberA", Grade.VIP);
    memberService.join(member);

    Member findMember = memberService.findMember(1L);
    System.out.println("new member = " + member.getName());
    System.out.println("find Member = " + findMember.getName());
  }
  ``` 
- �ٲ� �ڵ�
  ```java
  public static void main(String[] args) {

    ApplicationContext applicationContext = new AnnotationConfigApplicationContext(AppConfig.class);
    MemberService memberService = applicationContext.getBean("memberService", MemberService.class);

    Member member = new Member(1L, "memberA", Grade.VIP);
    memberService.join(member);

    Member findMember = memberService.findMember(1L);
    System.out.println("new member = " + member.getName());
    System.out.println("find Member = " + findMember.getName());

  }
  ``` 

`OrderApp`�� ���� ���� �����ϰ� �ٲٸ� ��

**������ �����̳�**
- `ApplicationContext`�� `������ �����̳ʶ�� �Ѵ�.
- �������� �����ڰ� `AppConfig`�� ����ؼ� ���� ��ü�� �����ϰ� DI�� ������, �������ʹ� ������ �����̳ʸ� ���ؼ� ����Ѵ�.
- ������ �����̳ʴ� `@Configuration`�� ���� `AppConfig`�� ����(����) ������ ���.
- ���⼭ `@Bean`�̶� ���� �޼��带 ��� ȣ���ؼ� ��ȯ�� ��ü�� ������ �����̳ʿ� ���.
  - �̷��� ������ �����̳ʿ� ��ϵ� ��ü�� ������ ���̶� �Ѵ�.
- ������ ���� `@Bean`�� ���� method�� name�� ������ ���� �̸����� ���(`memberService`,`orderService`)
- �������� �����ڰ� �ʿ��� ��ü�� `AppConfig`�� ����ؼ� ���� ��ȸ������, �������ʹ� ������ �����̳ʸ� ���ؼ� �ʿ��� ������ ��(��ü)�� ã�ƾ� �Ѵ�. ������ ���� `applicationContext.getBean()` method�� ����ؼ� ã�� �� �ִ�.
- �������� �����ڰ� ���� �ڹ� �ڵ�� ��� ���� �ߴٸ�, �������ʹ� ������ �����̳ʿ� ��ü�� ������ ������ ����ϰ�, ������ �����̳ʿ��� ������ ���� ã�Ƽ� ����ϵ��� ������.

---
---

## ������ �����̳ʿ� ������ ��

---
---

### ������ �����̳� ����

������ �����̳� ���� ����

```java
//������ �����̳� ����
ApplicationContext applicationContext = new AnnotationConfigApplicationContext(AppConfig.class);
```

- `ApplicationContext` = ������ �����̳ʶ� �Ѵ�.
- `ApplicationContext` = �������̽�.
- ������ �����̳ʴ� XML ������� ���� ���� �ְ�, �ֳ����̼�(@) ����� �ڹ� ���� Ŭ������ ���� �� �ִ�.
- ������ `AppConfig`�� ����ߴ� ����� �ֳ����̼� ����� �ڹ� ���� Ŭ������ ������ �����̳ʸ� ���� ��.
- �ڹ� ���� Ŭ������ ������� ������ �����̳�(`ApplicationContext`)�� ������.
  - `new AnnotationsConfigApplicationContext(AppConfig.class);`
  - �� Ŭ������ `ApplicationContext` �������̽��� ����ü�̴�.

1. ������ �����̳� ����
![create_spring_container](./readme_img/create_spring_container.JPG)

   - `new AnnotationConfigApplicationContext(AppConfig.class)`
   - ������ �����̳ʸ� ������ ���� ���� ������ ����������ϸ� ���⼭�� `AppConfig.class`�� ���� ������ ����.

2. ������ �� ���
![spring_bin](./readme_img/spring_bin.JPG)

  - ������ �����̳ʴ� �Ķ���ͷ� �ѿ��� ���� Ŭ���� ������ ����ؼ� ������ ���� ���.
  
  **�� �̸�**
  - �� �̸��� method �̸��� ���.
  - �� �̸��� ���� �ο��� ���� �ִ�.
    - `@Bean(name="memberService2") `
  >**����: �� �̸��� �׻� �ٸ� �̸��� �ο�**�ؾ� �Ѵ�. ���� �̸��� �ο��ϸ�, �ٸ� ���� ���õǰų�, ���� ���� ��������ų� ������ ���� ������ �߻�.

3. ������ �� �������� ���� - �غ�
![spring_bin_depen](./readme_img/spring_bin_depen.JPG)
- ������ ��ü�� ������ ��, �� ���� ���� ���踦 �����������.

4. ������ �� �������� ���� - �Ϸ�
![spring_bin_fin](./readme_img/spring_bin_fin.JPG)
- `memberService`�� ��������� `memberRepository`�� �־����, �׷��� `MemoryMemberRepository`�� ������ ��.
- �� ����, `orderService`�� `memberRepository`�� `discountPolicy`�� �����Ѵ�. �׷��� `MemoryMemberRepository`�� `RateDiscountPolicy`�� ������ �ȴ�.
- ������ �����̳ʴ� ���� ������ �����ؼ� �������踦 ����(DI)�Ѵ�.
- �ܼ��� �ڹ� �ڵ带 ȣ���ϴ� �� ������, ���̰� �ִ�.(�̱��� �����̳ʿ��� ������).

**����**

  ������ = �� ���� + �������� ����, �ϴ� �ܰ�� �������� �ִ�.

  �׷��� �ڹ� �ڵ�� ������ ���� ����ϸ� �����ڸ� ȣ���ϸ鼭 �������� ���Ե� �ѹ��� ó���ȴ�.
  
  ���⼭�� ���ظ� ���� ���� ���������� ������ �����߰�, �ڼ��� ������ �������� �ڵ� ���Կ��� �ٽ� ����.

**����**

  ������ �����̳ʸ� �����ϰ�, ����(����) ������ �����ؼ� ������ �� ����ϰ�, �������赵 �����ߴ�.

  ������ ������ �����̳ʿ��� �����͸� ��ȸ�غ���.


---

### �����̳ʿ� ��ϵ� ��� �� ��ȸ

��� �� ����ϱ�
- �����ϸ� �������� ��ϵ� ��� �� ������ ����� �� �ִ�.
- `ac.getBeanDefinitionNames()` : �������� ��ϵ� ��� �� �̸� ��ȸ.
- `ac.getBean()` : �� �̸����� �� ��ü(�ν��Ͻ�)�� ��ȸ.

���������̼� �� ����ϱ�
- ������ ���ο��� ����ϴ� ���� `getRole()`�� ������ �� �ִ�.
  - `ROLE_APPLICATION` : �Ϲ������� ����ڰ� ������ ��
  - `ROLE_INFRASTRUCTURE` : �������� ���ο��� ����ϴ� ��
```java
@Test
@DisplayName("���ø����̼� �� ����ϱ�")
void findApplicationBean(){
    String[] beanDefinitionNames = ac.getBeanDefinitionNames();
    for (String beanDefinitionName : beanDefinitionNames) {
        BeanDefinition beanDefinition = ac.getBeanDefinition(beanDefinitionName);//bean �ϳ��ϳ��� ���� metadata ����
        // �������� ���ο��� ���� �ϱ� ���ؼ� ����� ���� �ƴ϶� ���� ���ø����̼��� �ַ� �����ϱ����ؼ�
        // ����� ��(�ƴϸ� �ܺ� ���̺귯��..)
        if (beanDefinition.getRole() == BeanDefinition.ROLE_APPLICATION){
            Object bean = ac.getBean(beanDefinitionName);
            System.out.println("name = " + beanDefinitionName + " object = " + bean);
        }
    }
}
```

---

### ������ �� ��ȸ - �⺻

`ac.getBean(���̸�, Ÿ��)`

`ac.getBean(Ÿ��)`

��ȸ ��� ������ ���� ������ ���� �߻�
  
  - `NoSuchBeanDefinitionException: No bean named 'xxxxx' available'`

��� �� ����ϱ�

```java
AnnotationConfigApplicationContext ac = new AnnotationConfigApplicationContext(AppConfig.class);

@Test
@DisplayName("��� �� ����ϱ�")
void findAllBean(){
    String[] beanDefinitionNames = ac.getBeanDefinitionNames();
    for (String beanDefinitionName : beanDefinitionNames) {
        Object bean = ac.getBean(beanDefinitionName);
        System.out.println("name = " + beanDefinitionName + " object = " + bean);
    }
}
```

���ø����̼� �� ����ϱ�

```java
@Test
@DisplayName("���ø����̼� �� ����ϱ�")
void findApplicationBean(){
    String[] beanDefinitionNames = ac.getBeanDefinitionNames();
    for (String beanDefinitionName : beanDefinitionNames) {
        BeanDefinition beanDefinition = ac.getBeanDefinition(beanDefinitionName);//bean �ϳ��ϳ��� ���� metadata ����
        // �������� ���ο��� ���� �ϱ� ���ؼ� ����� ���� �ƴ϶� ���� ���ø����̼��� �ַ� �����ϱ����ؼ�
        // ����� ��(�ƴϸ� �ܺ� ���̺귯��..)
        if (beanDefinition.getRole() == BeanDefinition.ROLE_APPLICATION){
            Object bean = ac.getBean(beanDefinitionName);
            System.out.println("name = " + beanDefinitionName + " object = " + bean);
        }
    }
}
```

�� �̸����� ��ȸ

```java
@Test
@DisplayName("�� �̸����� ��ȸ")
void findBeanByName(){
    MemberService memberService = ac.getBean("memberService",MemberService.class);
//        System.out.println("memberService = " + memberService);
//        System.out.println("memberService.getClass() = " + memberService.getClass());
    assertThat(memberService).isInstanceOf(MemberServiceImpl.class);
}

```

�̸� ���� Ÿ�����θ� ��ȸ

```java
@Test
@DisplayName("�̸� ���� Ÿ�����θ� ��ȸ")
void findBeanByType(){
    MemberService memberService = ac.getBean(MemberService.class);
    assertThat(memberService).isInstanceOf(MemberServiceImpl.class);
}
```

��ü Ÿ������ ��ȸ

```java
@Test
@DisplayName("��ü Ÿ������ ��ȸ")
void findBeanByName2(){
    MemberService memberService = ac.getBean("memberService",MemberServiceImpl.class);
    assertThat(memberService).isInstanceOf(MemberServiceImpl.class);
}
```
  - �������� ������


�� �̸����� ��ȸ

```java
@Test
@DisplayName("�� �̸����� ��ȸX")
void findByBeanNameX(){
//        ac.getBean("xxxxx", MemberService.class);
    //MemberService xxxxx = ac.getBean("xxxxx", MemberService.class);
    assertThrows(NoSuchBeanDefinitionException.class,
            () -> ac.getBean("xxxxx", MemberService.class));
}
```
  - assertThrows�� org.junit.jupiter.api.Assertions ����.
  ```java
  assertThrows(NoSuchBeanDefinitionException.class,
            () -> ac.getBean("xxxxx", MemberService.class)); 
  ``` 
    - ���� : () -> ~~~ : �� ������ ������ �ϸ� `NoSuchBeanDefinitionException`�� ��������(������ ����, �������� ����)


---

### ������ �� ��ȸ - ������ Ÿ���� �� �̻�

Ÿ������ ��ȸ�� ���� Ÿ���� ������ ���� �� �̻��̸� ������ �߻��Ѵ�. �̶��� �� �̸��� ��������.

`ac.getBeanOfType()` �� ����ϸ� �ش� Ÿ���� ��� ���� ��ȸ�� �� �ִ�.

Ÿ������ ��ȸ�� ���� Ÿ���� �� �̻� ������, �ߺ� ������ �߻��Ѵ�

```java
AnnotationConfigApplicationContext ac = new AnnotationConfigApplicationContext(SameBeanConfig.class);

//NoUniqueBeanDefinitionException�� ����
@Test
@DisplayName("Ÿ������ ��ȸ�� ���� Ÿ���� �� �̻� ������, �ߺ� ������ �߻��Ѵ�")
void findBeanByTypeDuplicate(){
    assertThrows(NoUniqueBeanDefinitionException.class,
            () -> ac.getBean(MemberRepository.class));
}
```

Ÿ������ ��ȸ�� ���� Ÿ���� �� �̻� ������, �� �̸��� �����ϸ� �ȴ�

```java
@Test
@DisplayName("Ÿ������ ��ȸ�� ���� Ÿ���� �� �̻� ������, �� �̸��� �����ϸ� �ȴ�")
void findBeanByName(){
    MemberRepository memberRepository = ac.getBean("memberRepository1",MemberRepository.class);
    assertThat(memberRepository).isInstanceOf(MemberRepository.class);
}
```

Ư�� Ÿ���� ��� ��ȸ�ϱ�
```java
@Test
@DisplayName("Ư�� Ÿ���� ��� ��ȸ�ϱ�")
void findAllBeanByType(){
    //key : String, value : MemberRepository
    Map<String, MemberRepository> beansOfType = ac.getBeansOfType(MemberRepository.class);
    for (String key : beansOfType.keySet()) {
        System.out.println("key = " + key + " value = " + beansOfType.get(key));
    }
    System.out.println("beansOfType = " + beansOfType);
    assertThat(beansOfType.size()).isEqualTo(2);

}
```

Test���� ���� Config ����
```java
// �ߺ��� �˻��ؾ��ϴµ� Appconfig�� �ǵ�� �Ⱦ ���� ����
//static�� ���� : scope�� �� �ȿ����� ����ϰڴٴ� �ǹ�
@Configuration
static class SameBeanConfig {

    @Bean
    public MemberRepository memberRepository1() {
        return new MemoryMemberRepository();
    }

    @Bean
    public MemberRepository memberRepository2() {
        return new MemoryMemberRepository();
    }
}
```

---

### ������ �� ��ȸ - ��� ����

- �θ� Ÿ������ ��ȸ�ϸ�, �ڽ� Ÿ�Ե� �Բ� ��ȸ�Ѵ�.
- �׷��� ��� �ڹ� ��ü�� �ְ� �θ��� `Object` Ÿ������ ��ȸ�ϸ�, ��� ������ ���� ��ȸ�� �� �ִ�.

TestConfig ����

```java
@Configuration
static class TestConfig{
    @Bean
    public DiscountPolicy rateDiscountPolicy(){
        return new RateDiscountPolicy();
    }

    @Bean
    public DiscountPolicy fixDiscountPolicy(){
        return new FixDiscountPolicy();
    }
}
```

�θ� Ÿ������ ��ȸ ��, �ڽ��� �� �̻� ������ �ߺ� ������ �߻��Ѵ�

```java
@Test
  @DisplayName("�θ� Ÿ������ ��ȸ ��, �ڽ��� �� �̻� ������ �ߺ� ������ �߻��Ѵ�")
  void findBeanByParentTypeDuplicate(){
      DiscountPolicy bean = ac.getBean(DiscountPolicy.class);
      Assertions.assertThrows(NoUniqueBeanDefinitionException.class,
              () -> ac.getBean(DiscountPolicy.class));
  }
```

�θ� Ÿ������ ��ȸ ��, �ڽ��� �� �̻� ������, �� �̸��� �����ϸ� �ȴ�

```java
@Test
@DisplayName("�θ� Ÿ������ ��ȸ ��, �ڽ��� �� �̻� ������, �� �̸��� �����ϸ� �ȴ�")
void findBeanByParentTypeBeanName(){
    DiscountPolicy rateDiscountPolicy = ac.getBean("rateDiscountPolicy",DiscountPolicy.class);
    org.assertj.core.api.Assertions.assertThat(rateDiscountPolicy).isInstanceOf(RateDiscountPolicy.class);
}
```

Ư�� ���� Ÿ������ ��ȸ

```java
//not good
@Test
@DisplayName("Ư�� ���� Ÿ������ ��ȸ")
void findBeanBySubTypes(){
    RateDiscountPolicy bean = ac.getBean(RateDiscountPolicy.class);
    org.assertj.core.api.Assertions.assertThat(bean).isInstanceOf(RateDiscountPolicy.class);
}
```

�θ� Ÿ������ ��� ��ȸ�ϱ�

```java
@Test
@DisplayName("�θ� Ÿ������ ��� ��ȸ�ϱ�")
void findAllBeanByParentType(){
    Map<String, DiscountPolicy> beansOfType = ac.getBeansOfType(DiscountPolicy.class);
    org.assertj.core.api.Assertions.assertThat(beansOfType.size()).isEqualTo(2);
    for (String key : beansOfType.keySet()) {
        System.out.println("key = " + key + " value = " + beansOfType.get(key));
    }
}
```

�θ� Ÿ������ ��� ��ȸ�ϱ� - Object

```java
//java ��ü�� ������ object type�̱� �����̴�
//�׷��� spring bin�� ��ϵ� ��� ��ü�� �� Ƣ��´�.
@Test
@DisplayName("�θ� Ÿ������ ��� ��ȸ�ϱ� - Object")
void findAllBeanByObjectType(){
    Map<String, Object> beansOfType = ac.getBeansOfType(Object.class);
    for (String key : beansOfType.keySet()) {
        System.out.println("key = " + key + " value = " + beansOfType.get(key));
    }
}
```
---

### BeanFactory�� ApplicationContext
 
![beanfactory](./readme_img/beanfactory.JPG)

  - �׸��� ���� ApplicationContext�� BeanFactory���ٰ� �ΰ������ ���ѰŶ�� ���صȴ�.

**BeanFactory**
- ������ �����̳��� �ֻ��� �������̽�.
- ������ ���� ����, ��ȸ�ϴ� ���� ���
- `getBean()`�� ����
- ���ݱ��� ����� ��κ� ����� BeanFactory�� �����ϴ� ���.

**ApplicationContext**
- BeanFactory�� ����� ��� ��ӹ޾Ƽ� ����.
- ���� �����ϰ� �˻��ϴ� ����� BeanFactory�� �������ִµ�, ��������?
  - ���ø����̼��� ������ ���� ���� �����ϰ� ��ȸ�ϴ� ����� �����̰�, �� ���� **�ΰ����**�� �ʿ��ϴ�.

**ApplicationContext�� �����ϴ� �ΰ����**
![application](./readme_img/application.JPG)
   
  - **�޽����ҽ��� Ȱ���� ����ȭ ���**
    - ex> �ѱ����� ������ �ѱ����, ����ǿ��� ������ ����� ���
  - **ȯ�溯��**
    - ����,����,����� �����ؼ� ó��
    - �����Ҷ��� ũ�� 3���� ȯ���� ����
      - ����(�� PC), TEST ����(���� ȯ��), � ȯ��(���� ����) + ����(�������� ȯ��)(��� ���� ������ ȯ��)
  - **���ø����̼� �̺�Ʈ**
    - �̺�Ʈ�� �����ϰ� �����ϴ� ���� ���ϰ� ����
  - **���� ���ҽ� ��ȸ**
    - ����, Ŭ�����н�, �ܺ� ��� ���ҽ��� ���ϰ� ��ȸ.

����
- ApplicationContext�� BeanFactory�� ����� ��ӹ޴´�.
- ApplicationContext�� �� ������� + ���� �ΰ� ����� ����.
- BeanFactory�� ���� ����� ���� ���� ����. �ΰ������ ���Ե� ApplicationContext�� ����Ѵ�.
- BeanFactory�� ApplicationContext�� ������ �����̳ʶ� �Ѵ�.

---

### �پ��� ���� ���� ���� - �ڹ� �ڵ� ,XML

- ������ �����̳ʴ� �پ��� ������ ���� ������ �޾Ƶ帱 �� �ְ� �����ϰ� ����Ǿ� �ִ�.
  - �ڹ� �ڵ�, XML, Groovy ��...

![xml](./readme_img/xml.JPG)

�ֳ����̼� ��� �ڹ� �ڵ� ���� ���
- ���ݱ��� �ߴ� �͵�
- `new AnnotationConfigApplicationContext(AppConfig.class)`
- `AnnotationConfigApplicationContext` Ŭ������ ����ϸ鼭 �ڹ� �ڵ�ε� ���� ������ �ѱ�� �ȴ�.


XML ���� ���
- �ֱٿ��� ������ ��Ʈ�� ���� ����ϸ鼭 XML ��� ������ �� ���X.
- `GenericXmlApplicationContext`�� ����ϸ鼭 `xml` ���� ������ �ѱ�� �ȴ�.

- xml ����� `appConfig.xml` ������ ���� ������ �ڹ� �ڵ�� �� `AppConfig.java` ���� ������ ���غ��� ���� ����ϴٴ� ���� �� �� �ִ�.
- xml ������� �����ϴ� ���� �ֱٿ� �� ���X
  - �ʿ��� ��� ���� ���۷��� �������� Ȯ��.
  - https://spring.io/projects/spring-framework

---

### ������ �� ���� ��Ÿ ���� - BeanDefinition

- xml, �ڹ� �ڵ� �� �������� �̷� �پ��� ���� ������ �����ϴ� ���� �߽ɿ��� `BeanDefinition` �̶�� �߻�ȭ�� �ִ�.
- ��, **���Ұ� ������ ���������� ���� ��**�̴�.
  - XML�� �о BeanDefinition�� ����� �ȴ�.
  - �ڹ� �ڵ带 �о BeanDefinition�� ����� �ȴ�.
  - ������ �����̳ʴ� �ڹ� �ڵ�����, XML���� ���� �ȴ�. ���� BeanDefintion�� �˸� �ȴ�.
- `BeanDefinition`�� �� ���� ��Ÿ������ �Ѵ�.
  - `@Bean`, `<bean>`�� ���� �ϳ��� ��Ÿ ������ �����ȴ�.
- ������ �����̳ʴ� �� ��Ÿ������ ������� ������ ���� �����Ѵ�.
  ![beandefinition](./readme_img/beandefinition.JPG)

  - �׸� �� `������ �����̳�` ��ü�� `BeanDefinition`���� �����Ѵ�. class�� �����Ȱ���, xml�� �����Ȱ���, ���Ƿ� �Ȱ��� �������
  - ������ü�� �߻�ȭ(`BeanDefinition`)���� �����ϵ��� �����Ѱ���.

  �ڵ� ������ ���� �� ���� �ְ� ������,
  ![bean_code](./readme_img/bean_code.JPG)

  - `AnnotationConfigApplicationContext`�� `AnnotatedBeanDefinitionReader`�� ����ؼ� `AppConfig.class`�� �а� `BeanDefinition`�� ����.
  - `GenericXmlApplicationContext`�� `XmlBeanDefinitionReader`�� ����ؼ� `appConfig.xml` ���� ������ �а� `BeanDefinition`�� ����.
  - ���ο� ������ ���� ������ �߰��Ǹ�, XxxBeanDefinitionReader�� ���� `BeanDefinition`�� �����ϸ� �ȴ�.


BeanDefinition ���캸��

```java
AnnotationConfigApplicationContext ac = new AnnotationConfigApplicationContext(AppConfig.class);

@Test
@DisplayName("�� ���� ��Ÿ���� Ȯ��")
void findApplicationBean(){
    String[] beanDefinitionNames = ac.getBeanDefinitionNames();
    for (String beanDefinitionName : beanDefinitionNames) {
        BeanDefinition beanDefinition = ac.getBeanDefinition(beanDefinitionName);

        if (beanDefinition.getRole() == BeanDefinition.ROLE_APPLICATION){
            System.out.println("beanDefinitionName = " + beanDefinitionName +
            " beanDefinition = " + beanDefinition);
        }
    }
}
```
  
  - **BeanDefinition ����**
    - BeanClassName : ������ ���� Ŭ���� ��(�ڹ� ���� ó�� ���丮 ������ ���� ����ϸ� ����)
    - factoryBeanName : ���丮 ������ ���� ����� ��� �̸�
      - ex> appConfig
    - factoryMethodName : ���� ������ ���丮 �޼��� ����
      - ex> memberService
    - Scope : �̱���(�⺻��)
    - lazyInit : ������ �����̳ʸ� ������ �� ���� �����ϴ� ���� �ƴ϶�, ���� ���� ����� �� ���� �ִ��� ������ ����ó�� �ϴ��� ����
    - InitMethodName : ���� �����ϰ�, �������踦 ������ �� ȣ��Ǵ� �ʱ�ȭ �޼��� ��
    - DestroyMethodName : ���� �����ֱⰡ ������ �����ϱ� ������ ȣ��Ǵ� �޼��� ��
    - Constructor arguments, Properties : �������� ���Կ��� ����Ѵ�.(�ڹ� ���� ó�� ���丮 ������ ���� ����ϸ� ����)

  �Ʒ��� ���� �׽�Ʈ�� ������ ����.
    ![beandefinition2](./readme_img/beandefinition2.JPG)


**����**
- BeanDefinition�� ���� �����ؼ� ������ �����̳ʿ� ����� ���� �ִ�. �׷���, �ǹ����� BeanDefinition�� ���� �����ϰų� ����� ���� ���� ����.
- BeanDefinition�� ���ؼ��� �������� �پ��� ������ ���� ������ BeanDefinition���� �߻�ȭ�ؼ� ����ϴ� �� ������ �����ϱ�
- ���� ������ �ڵ峪 ������ ���� ���� �ҽ��� �ڵ带 �� ��, BeanDefinitino�̶�� ���� ���� ���� �ִµ�, �̶� �̷��� ��Ŀ������ ���ø��� �ȴ�.

Spring�� bean�� ����ϴ� ��(ũ�� 2����)
1. ���� spring bean ���(xml,...)
2. ��ȸ�ؼ��ϱ�(factorymethod���,�ڹ� �ڵ带 ������ @Bean ����ϴ� ���)

---
---

## �̱��� �����̳�

---
---

### �� ���ø����̼ǰ� �̱���

- �̱��� ���� : ��ü�� ���� JVM�ȿ� �ϳ��� �־���ϴ� �׷��� ����
- �������� �»��� ����� �¶��� ���� ����� �����ϱ� ���� ź��.
- ��κ��� ������ ���ø����̼��� �� ���ø����̼��̴�. ���� ���� �ƴ� ���ø����̼� ����(batch, demon...)�� �󸶵��� ������ �� �ִ�.
- �� ���ø����̼��� ���� ���� ���� ���ÿ� ��û�� �Ѵ�.

![single](./readme_img/single.JPG)
  - Ŭ���̾�Ʈ A,B,C�� spring���� ���ÿ� ��û�� ��.
  - �츮�� ���� ���� DI �����̳�(AppConfig)���� ��ü�� ��ȯ��.
  - ��, ���� 3�� ��û�ϸ� ��ü�� 3�� ������ ��.
  - ��� ��û�� �ö����� ��ü�� �������ϴµ�, �̷��� ���� �������̴�.

```java
@Test
@DisplayName("������ ���� ������ DI �����̳�")
void pureContainer(){
    AppConfig appConfig = new AppConfig();
    //1. ��ȸ: ȣ���� �� ���� ��ü�� ����
    MemberService memberService1 = appConfig.memberService();

    //2. ��ȸ: ȣ���� �� ���� ��ü�� ����
    MemberService memberService2 = appConfig.memberService();

    //�������� �ٸ� ���� Ȯ��
    System.out.println("memberService1 = " + memberService1);
    System.out.println("memberService2 = " + memberService2);

    //memberService1 != memberService2
    assertThat(memberService1).isNotSameAs(memberService2);
}
```
  - ������
    ![result](./readme_img/result.JPG)
  - ��ü�� ���� �ٸ���.
  - ��, JVM �޸𸮿� ��� ��ü�� �����ؼ� �ö󰡰� �ȴ�.
  - �� ���ø����̼��� Ư¡�� �� ��û�� ��û ������ �̷������� ��� ��ü�� �����ϴ� ���� ȿ�������� �ʴ�.
  - �츮�� ���ſ� ������� ������ ���� ������ DI �����̳��� AppConfig�� ��û�� �� �� ���� ��ü�� ���� �����Ѵ�.
  - �� Ʈ������ �ʴ� 100�� ������ �ʴ� 100�� ��ü�� �����ǰ� �Ҹ�ȴ� == **�޸� ���� ���ϴ�**
  - �ذ����� �ش� ��ü�� �� **1���� ����**�ǰ�, **����**�ϵ��� �����ϸ� �ȴ� -> **�̱��� ����**


---

### �̱��� ����

- Ŭ������ �ν��Ͻ��� �� 1���� �����Ǵ� ���� �����ϴ� ������ �����̴�.
  - �� JVM, �� java ���� �ȿ����� ��ü�� �ν��Ͻ��� �� 1���� �����ǵ��� �ϴ� ������ ����.
- �׷��� ��ü �ν��Ͻ��� 2�� �̻� �������� ���ϵ��� ���ƾ� �Ѵ�.
  - private �����ڸ� ����ؼ� �ܺο��� ���Ƿ� new Ű���带 ������� ���ϵ��� ���ƾ� �Ѵ�.

```java
public class SingletonService {

    private static final SingletonService instace = new SingletonService();
    
  
    ....
}
```
  - �ڱ� �ڽ��� ���ο� private static���� ������ �ִ�.
    - �̷��� �ϸ�, class level�� �ö󰡱⶧���� �� 1���� �����ϰ� �ȴ�.
  - JVM, �ڹٰ� �� ��, SingletonService�� static�̶�� �Ǿ��ְ� �� �����ʿ� new��� �Ǿ��ִ°� ���� new SingletonService()�� ���������� ������� �� ��ü(�ڱ��ڽ�)�� �����ؼ� `instance`�� ������ �־��. �׷���, �ڱ� �ڽ��� ��ü �ν��Ͻ��� �����ؼ� ���� �ȿ��� ���ִ°���.

```java
public static SingletonService getInstace(){
    return instace;
}
```
  - ��ȸ�Ҷ���, getInstance()�� ����ϸ� ��.

```java
private SingletonService(){
        
}
```
  - �ٸ� ������ new�� ���� ��ü�� �����ϴ� ���� �����ϱ� ���� private���� ����.

```java
public void logic(){
    System.out.println("�̱��� ��ü ���� ȣ��");
}
```
  - �׳� ������

���� �ڵ���� ���� `�̱���`�� ��.
1. static ������ ��ü instance�� �̸� �ϳ� �����ؼ� �÷��д�.
2. �� ��ü �ν��Ͻ��� �ʿ��ϸ� ���� `getInstance()` �޼��带 ���ؼ��� ��ȸ�� �� �ִ�. �� �޼��带 ȣ���ϸ� �׻� ���� �ν��Ͻ��� ��ȯ�Ѵ�.
3. �� 1���� ��ü �ν��Ͻ��� �����ؾ� �ϹǷ�, �����ڸ� private���� ���Ƽ� Ȥ�ö� �ܺο��� new Ű����� ��ü �ν��Ͻ��� �����Ǵ� ���� ���´�.


singleton test
```java
@Test
@DisplayName("�̱��� ������ ������ ��ü ���")
void singletonServiceTest(){
    SingletonService singletonService1 = SingletonService.getInstace();
    SingletonService singletonService2 = SingletonService.getInstace();

    System.out.println("singletonService1 = " + singletonService1);
    System.out.println("singletonService2 = " + singletonService2);
    
}
```
   - �������ϸ�, ���� ��ü�ΰ��� Ȯ���� �� �ִ�.

- �׷��ٸ�, AppConfig�� ��� �� �̱��� �������� �ٲ���ϳ�?
  - �׷��ʿ�� ����.
  - spring container�� ����ϸ� spring container�� �⺻������ ��ü�� �̱������� ���� ���� ����.
- �̱��� ������ �����̵Ǹ�, ���� �� ��û�� �ʴ� 100���� �ͼ� ó���ؾߵǾ ��ü�� �������ʰ� �ִ� ��ü�� �״�� ��Ȱ���� == ������ ������.


- �̱��� ������ �����ϴ� ����� ���������� �ִ�.
  - ���� �����, ��ü�� �̸� �����صδ� ���� �ܼ��ϰ� ������ ���.
  - ��Ÿ���

**�̱��� ���� ������**
- �̱��� ������ �����ϴ� �ڵ� ��ü�� ���� ����.
- ��������� Ŭ���̾�Ʈ�� ��ü Ŭ������ �����Ѵ� -> DIP�� ����.
- Ŭ���̾�Ʈ�� ��ü Ŭ������ �����ؼ� OCP ��Ģ ������ ���ɼ��� ����.
- �׽�Ʈ�ϱ� ��ƴ�.
- ���� �Ӽ��� �����ϰų� �ʱ�ȭ �ϱ� ��ƴ�.
- private �����ڷ� �ڽ� Ŭ������ ����� ��ƴ�.
- ��������� �������� ��������.
- ��Ƽ�������� �Ҹ��⵵ �Ѵ�.

---

### �̱��� �����̳�

������ �����̳ʴ� �̱��� ������ �������� �ذ��ϸ鼭, ��ü �ν��Ͻ��� �̱���(1���� ����)���� �����Ѵ�. ���ݱ��� �н��� ������ ���� �ٷ� �̱������� �����Ǵ� ���̴�.

**�̱��� �����̳�**
- ������ �����̳ʴ� �̱��� ������ �������� �ʾƵ�, ��ü �ν��Ͻ��� �̱������� ����.
  - �����̳ʴ� ��ü�� �ϳ��� �����ؼ� ����.
- ������ �����̳ʴ� �̱��� �����̳� ������ �Ѵ�. �̷��� �̱��� ��ü�� �����ϰ� �����ϴ� ����� �̱��� ������Ʈ���� �Ѵ�.
- ������ �����̳��� �̷� ��� ���п� �̱��� ������ ��� ������ �ذ��ϸ鼭 ��ü�� �̱������� ����.
  - �̱��� ������ ���� �������� �ڵ尡 ���� �ʾƵ� ��.
  - DIP, OCP, �׽�Ʈ, private �����ڷ� ���� �����Ӱ� �̱����� ����� �� �ִ�.

**�̱��� �����̳� ���� ��**
```java
@Test
@DisplayName("������ �����̳ʿ� �̱���")
void springContainer(){

    ApplicationContext ac = new AnnotationConfigApplicationContext(AppConfig.class);

    MemberService memberService1 = ac.getBean("memberService",MemberService.class);
    MemberService memberService2 = ac.getBean("memberService",MemberService.class);


    //�������� �ٸ� ���� Ȯ��
    System.out.println("memberService1 = " + memberService1);
    System.out.println("memberService2 = " + memberService2);

    //memberService1 != memberService2
    assertThat(memberService1).isSameAs(memberService2);
}
```

  ![after_singleton](./readme_img/after_singleton.JPG)
  - ������ �����̳� ���п� ���� ��û�� �� �� ���� ��ü�� �����ϴ� ���� �ƴ϶�, �̹� ������� ��ü�� �����ؼ� ȿ�������� ������ �� �ִ�.

���� : �������� �⺻ �� ��� ����� �̱���������, �̱��� ��ĸ� �����ϴ� ���� �ƴϴ�. ��û�� �� ���� ���ο� ��ü�� �����ؼ� ��ȯ�ϴ� ��ɵ� ������.

---

### �̱��� ����� ������

- �̱��� �����̵�, ������ ���� �̱��� �����̳ʸ� ����ϵ�, ��ü �ν��Ͻ��� �ϳ��� �����ؼ� �����ϴ� �̱��� ����� ���� Ŭ���̾�Ʈ�� �ϳ��� ���� ��ü �ν��Ͻ��� �����ϱ� ������ **�̱��� ��ü�� ���¸� ����(stateful)�ϰ� �����ϸ� �ȵȴ�.**
- **������(stateless)�� ����**�ؾ� �Ѵ�.
  - Ư�� Ŭ���̾�Ʈ�� �������� �ʵ尡 ������ �ȵȴ�.
  - Ư�� Ŭ���̾�Ʈ�� ���� ������ �� �ִ� �ʵ尡 ������ �ȵ�.
  - ������ �б⸸ ����.(�������̸� ���� �����ϸ� �ȵ�.)
  - �ʵ� ��ſ� �ڹٿ��� �������� �ʴ�, ��������, �Ķ����, ThreadLocal ���� ����ؾ� �Ѵ�.
- ������ ���� �ʵ忡 ���� ���� �����ϸ� ���� ū ��ְ� �߻��� �� �ִ�. 

```java
@Test
void statefulServiceSingleton(){
    ApplicationContext ac = new AnnotationConfigApplicationContext(TestConfig.class);
    StatefulService statefulService1 = ac.getBean(StatefulService.class);
    StatefulService statefulService2 = ac.getBean(StatefulService.class);

    //ThreadA : A ����ڰ� 10000�� �ֹ�
    statefulService1.order("userA",10000);
    //ThreadB : B ����ڰ� 20000�� �ֹ�
    statefulService2.order("userB",20000);

    //ThreadA : ����� A�� �ֹ� �ݾ��� ��ȸ
    int price = statefulService1.getPrice();
    System.out.println("price = " + price);
}
```
  - �츮�� ����� ���� 10000���̴�.(�ֳ��ϸ� statefulService1�� ���� ��ȸ�߱� ������)
  - ������ �����ϸ� 20000���� ���´�.(�ֳ�, ���� ��ü�� �����ϴµ� �߰��� ����� B�� price�� �ٲ���ȱ� ����)

  - �ִ��� �ܼ��� �����ϱ� ����, ���� ������� ������� �ʾҴ�.
  - ThreadA�� �����A �ڵ带 ȣ���ϰ�, ThreadB�� �����B �ڵ带 ȣ���Ѵٰ� ����.
  - `StatefulService`�� `price` �ʵ�� �����Ǵ� �ʵ��ε�, Ư�� Ŭ���̾�Ʈ�� ���� ����.
  - �����A�� �ֹ��ݾ��� 10000���� �Ǿ�� �ϴµ�, 20000���̶�� ����� ����.
  - �ǹ����� �̷� ��츦 ���� ���µ�, �̷����� ���� �ذ��ϱ� ����� ū �������� ������.
  - �����ʵ�� ����!. ������ ���� �׻� ������(stateless)�� �����ؾ���.

---

### @Configuration�� �̱���

- @Bean memberService ȣ���ϸ� ��������� new MemoryMemberRepository()�� �ѹ� ȣ����.

- @Bean orderService ȣ���ϸ� ��������� new MemoryMemberRepository()�� ȣ��

- ������ MemoryMemberRepository()�� �� �� ȣ���� �� ==> �̱����� ������ ���ΰ�??

���� ���� �׽�Ʈ �غ���
```java
@Test
void configurationTest(){
    ApplicationContext ac = new AnnotationConfigApplicationContext(AppConfig.class);

    MemberServiceImpl memberService = ac.getBean("memberService", MemberServiceImpl.class);
    OrderServiceImpl orderService = ac.getBean("orderService", OrderServiceImpl.class);
    MemberRepository memberRepository = ac.getBean("memberRepository", MemberRepository.class);

    MemberRepository memberRepository1 = memberService.getMemberRepository();
    MemberRepository memberRepository2 = orderService.getMemberRepository();


    System.out.println("memberService -> memberRepository1 = " + memberRepository1);
    System.out.println("orderService -> memberRepository2 = " + memberRepository2);
    System.out.println("memberRepository = " + memberRepository);

    assertThat(memberService.getMemberRepository()).isSameAs(memberRepository);
    assertThat(orderService.getMemberRepository()).isSameAs(memberRepository);
}
```
- Ȯ���غ��� memberRepository �ν��Ͻ��� ��� ���� �ν��Ͻ��� �����Ǿ� ���ȴ�.
- AppConfig�� �ڹ� �ڵ带 ���� �и��� ���� 2�� `new MemoryMemberRepository` ȣ���ؼ� �ٸ� �ν��Ͻ��� �����Ǿ�� �Ұ� ������ `Appconfig`���� ��ü ���� �κп� soutm �ؼ� Ȯ���غ��� �ѹ����� ȣ��Ǵ� ����� �� �� �ִ�.


---

### @Configuration�� ����Ʈ�ڵ� ������ ����

������ �����̳ʴ� �̱��� ������Ʈ����.
  - ���� ������ ���� �̱����� �ǵ��� �������־�� �Ѵ�.
  - �׷��� �������� �ڹ� �ڵ���� ��� �ϱ�� ��ƴ�.
  - ������ �� �ڹ� �ڵ带 ���� �и� 3�� ȣ��Ǿ�� �Ѵ�.

�׷��� �������� Ŭ������ ����Ʈ�ڵ带 �����ϴ� ���̺귯���� ����Ѵ�

```java
@Test
void configurationDeep(){
    ApplicationContext ac = new AnnotationConfigApplicationContext(AppConfig.class);
    AppConfig bean = ac.getBean(AppConfig.class);
    System.out.println("bean.getClass() = " + bean.getClass());
}
```
  - ���� ������ Ŭ�������ٸ� ������ ���� ��µǾ�� �Ѵ�. `class hello.core.AppConfig`
  - �׷��� `bean.getClass() = class hello.core.AppConfig$$EnhancerBySpringCGLIB$$da84958b` �̷��� ��� ����� ���´�.
  - �̰��� ���� ���� Ŭ������ �ƴ϶� �������� CGLIB��� ����Ʈ�ڵ� ���� ���̺귯���� ����ؼ� `AppConfig` Ŭ������ ��ӹ��� ������ �ٸ� Ŭ������ �����, �� �ٸ� Ŭ������ ������ ������ ����� ���̴�.
  - ![configuration](./readme_img/configuration.JPG)
  - AppConfig�� �ִµ� CGLIB��� ����Ʈ�ڵ� ���� ���̺귯���� ������ AppConfig�� ��ӹ޾Ƽ� �ٸ� Ŭ����(`AppConfig@CGLIB`)�� �����. �׸��� `AppConfig@CGLIB`�� ������ ������ ����ع���, ������ �����̳ʿ��� �̸��� appConfig�̳� instance ��ü�� AppConfig@CGLIB�� ���ִ�.

�� ������ �ٸ� Ŭ������ �ٷ� �̱����� ����ǵ��� ���ش�. 

- @Bean�� ���� �޼��帶�� �̹� ������ ���� �����ϸ� �����ϴ� ���� ��ȯ�ϰ�, ������ ���� ������ �����ؼ� ������ ������ ����ϰ� ��ȯ�ϴ� �ڵ尡 �������� ���������.
- ���п� �̱����� ����Ǵ� ���̴�.

@Configuration�� �����ϰ� @Bean�� ���� ��� �� �ڵ���� �����ϸ� MemberRepository�� 3�� ȣ�� �Ǵ� ���� �� �� �ִ�.
  - 1���� @Bean�� ���� ������ �����̳ʿ� ����ϱ� ���ؼ�, 2���� ���� `memberRepository()`�� ȣ���ϸ鼭 �߻��� �ڵ�.

**����**
- @Bean�� ����ص� ������ ������ ��ϵ�����, �̱����� �������� �ʴ´�.
  - `memberRepository()` ó�� �������� ������ �ʿ��ؼ� �޼��带 ���� ȣ���� �� �̱����� �������� �ʴ´�.

- ũ�� ����� ���� ����. ������ ���� ������ �׻� `@Configuration`�� �������.

---
---

## ������Ʈ ��ĵ

---
---

### ������Ʈ ��ĵ�� �������� �ڵ� ���� �����ϱ�

- ���ݱ��� ������ ���� ����� ���� �ڹ� �ڵ��� @Bean�̳� XML�� `<bean>`���� ���ؼ� ���� ������ ���� ����� ������ ���� �����ߴ�.
- ���������� ��� �ȵǾ�����, ������ ���� ���� ���鰡�Ǹ� ������ ����ϱ� ������, ���� ������ Ŀ����, �ݺ��ϰ�, �����ϴ� ������ �߻�.
- �׷��� **�������� ���� ������ ��� �ڵ����� ������ ���� ����ϴ� ������Ʈ ��ĵ�̶�� ���**�� ����.
- �� **�������赵 �ڵ����� �����ϴ� `@Autowired`��� ��ɵ� ����**

```java
@ComponentScan(
    excludeFilters = @ComponentScan.Filter(type= FilterType.ANNOTATION)
)
```
- @Component�� ���� Ŭ������ ã�Ƽ� �ڵ����� ������ ������ �������
- ���߿��� �ڵ����� �� �͵鵵 �ִ�.(Configuration �ֳ����̼��� ���� ���̵�)

```java
@Configuration
@ComponentScan(
    excludeFilters = @ComponentScan.Filter(type= FilterType.ANNOTATION, classes = Configuration.class)
)
public class AutoAppConfig {
}
```
- ������Ʈ ��ĵ�� ����Ϸ��� ���� `@ComponetScan`�� ���� ������ �ٿ��ָ� �ȴ�.
- ������ `AppConfig`�ʹ� �ٸ��� `@Bean`���� ����� Ŭ������ �ϳ��� ����.

>���� : ������Ʈ ��ĵ�� ����ϸ� `@Configuration` �� ���� ���� ������ �ڵ����� ��ϵǱ� ������, AppConfig, TestConfig �� �ռ� �����ξ��� ���� ������ �Բ� ��ϵǰ� ����Ǿ� ������. �׷��� `excludeFilters`�� �̿��ؼ� ���������� ������Ʈ ��ĵ ��󿡼� �����ߴ�. ���� ���� ������ ������Ʈ ��ĵ ��󿡼� ���������� ������, ���� ���� �ڵ带 �ִ��� ����� �����ϰ� �;� �� ����� �����ߴ�.

������Ʈ ��ĵ�� �̸� �״�� `@Component` �ֳ����̼��� ���� Ŭ������ ��ĵ�ؼ� ������ ������ ����Ѵ�. `@Component`�� �ٿ�����.(+@Autowired)

- ������ AppConfig������ `@Bean`���� ���� ���� ������ �ۼ��߰�, �������赵 ���� ����ߴ�. ������ �̷� ���� ���� ��ü�� ���� ������, �������� ���Ե� �� Ŭ���� �ȿ��� �ذ��ؾ� �Ѵ�.
- `@Autowired`�� �������踦 �ڵ����� �������ش�. �ڼ��� ���� ���� �ڿ� �����ϰڴ�.




1. **ComponentScan**
  - ![component_scan](./readme_img/component_scan.JPG)
   - `@ComponentScan`�� `@Component`�� ���� ��� Ŭ������ ������ ������ ����Ѵ�.
   - �̶� ������ ���� �⺻ �̸��� `Ŭ������`�� ����ϵ� �� �ձ��ڸ� �ҹ��ڸ� ����Ѵ�
   - **�� �̸� �⺻ ����** : MemberServiceImpl Ŭ���� -> memberServiceImpl
   - **�� �̸� ���� ����** : ���� ������ ���� �̸��� ���� �����ϰ� ������ `@Component("memberServiceImpl")` �̷������� �̸��� �ο��ϸ� �ȴ�.
  
2. **@Autowired �������� �ڵ� ����**
  - ![autowired](./readme_img/autowired.JPG)
  - �����ڿ� `@Autowired`�� �����ϸ�, ������ �����̳ʰ� �ڵ����� �ش� ������ ���� ã�Ƽ� �����Ѵ�.
  - �̶� �⺻ ��ȸ ������ ������ ���� ���� ã�Ƽ� �����Ѵ�.
    - `getBean(MemberRepository.clasS)` �� �����ϴٰ� �����ϸ� �ȴ�.
    - �� �ڼ��� ������ �ڿ��� ����.
  - �����ڿ� �Ķ���Ͱ� ���Ƶ� �� ã�Ƽ� �ڵ����� �����Ѵ�.

ȥ�� ����
- AutoAppConfig�� `@ComponentScan`
- �ڵ����� class path�� �������鼭 �� spring bin�� ���
  - ���� ����ϴ� ���� �ƴϰ� `@Component`�� ���� class�� ������ �� ���.
- �׷���, `@Component`�� ���� class�� ������ ������ ����ϸ� �������踦 ������ �� �ִ� ����� ����.
  - ������ �������� �� ������ ������������ �� ������.
  - ������ AutoAppConfig�� ���������� �Ȼ���ϱ� ������ �׷��� `@Autowired`�� ���� �������� �ڵ� ������ ����Ѵ�.
- `@Autowired`�� �⺻������ `Ÿ��`�� ������ ����� ���ش�.

---

### Ž�� ��ġ�� �⺻ ��ĵ ���

Ž���� ��Ű���� ���� ��ġ ����
- ��� �ڹ� Ŭ������ �� ������Ʈ ��ĵ�ϸ� �ð��� ���� �ɸ���. �׷��� �� �ʿ��� ��ġ���� Ž���ϵ��� ���� ��ġ�� ������ �� �ִ�.
- 
  ```java
  @ComponentScan(
    basePackages = "hello.core",
  )
  ```
- `basePackages` : Ž���� ��Ű���� ���� ��ġ�� ����. �� ��Ű���� �����ؼ� ���� ��Ű���� ��� Ž��.
  - `basePackages = {"hello.core","hello.service"}` �̷��� ���� ���� ��ġ�� ������ ���� �ִ�.
- `basePackageClasses` : ������ Ŭ������ ��Ű���� Ž�� ���� ���� �����Ѵ�.
- ���� �������� ������, `@ComponentScan`�� ���� ���� ���� Ŭ������ ��Ű���� ���� ��ġ�� �ȴ�.

  > �����ϴ� ��� : ��Ű�� ��ġ�� �������� �ʰ�, ���� ���� Ŭ������ ��ġ�� ������Ʈ �ֻ�ܿ� �δ� ���̴�. �ֱ� ������ ��Ʈ�� �� ����� �⺻���� �����Ѵ�.

  ���� ��� ������Ʈ�� ������ ��Ƽ ������ �Ǿ� ������
  - `com.hello`
  - `com.hello.service`
  - `com.hello.repository`

  `com.hello`�� ������Ʈ ���� ��Ʈ, ���⿡ AppConfig ���� ���� ���� ������ �ΰ�, `@ComponentScan` �ֳ����̼��� ���̰�, `basePackages` ������ �����Ѵ�. 

  �̷��� �ϸ� `com.hello`�� ������ ������ ��� �ڵ����� ������Ʈ ��ĵ�� ����� �ȴ�. �׸��� ������Ʈ ���� ���� ������ ������Ʈ�� ��ǥ�ϴ� �����̱� ������ ������Ʈ ���� ��Ʈ ��ġ�� �δ� ���� ���� �����Ѵ�.
  
  ����� ������ ��Ʈ�� ����ϸ� ������ ��Ʈ�� ��ǥ ���� ������ `@SpringBootApplication`�� �� ������Ʈ ���� ��Ʈ ��ġ�� �δ� ���� �����̴�. (�׸��� �� �����ȿ� �ٷ� `@ComponentScan`�� ����ִ�!)

������Ʈ ��ĵ �⺻ ���
- �����ʹ� ��ĵ�� `@Component`�Ӹ� �ƴ϶� ������ ���� ���뵵 �߰��� ��� �����Ѵ�.
  - `@Component` : ������Ʈ ��ĵ���� ���
  - `@Controller` : ������ MVC ��Ʈ�ѷ����� ���
  - `@Service` : ������ ����Ͻ� �������� ���
  - `@Repository` : ������ ������ ���� �������� ���
  - `@Configuration` : ������ ���� �������� ���

  > ���� : ��� �ֳ����̼ǿ��� ��Ӱ����� ���� ����. �׷��� �̷��� �ֳ����̼��� Ư�� �ֳ����̼��� ��� �ִ� ���� �ν��� �� �ִ� ���� �ڹ� �� �����ϴ� ����� �ƴϰ�, �������� �����ϴ� ����̴�.  

- ������Ʈ ��ĵ�� �뵵 �Ӹ� �ƴ϶� ���� �ֳ����̼��� ������ �������� �ΰ� ����� �����Ѵ�.
  - `@Controller` : ������ MVC ��Ʈ�ѷ��� �ν�
  - `@Repository` : ������ ������ ���� �������� �ν��ϰ�, ������ ������ ���ܸ� ������ ���ܷ� ��ȯ���ش�.
  - `@Configuration` : �ռ� ���ҵ��� ������ ���� ������ �ν��ϰ�, ������ ���� �̱����� �����ϵ��� �߰� ó���� �Ѵ�.
  - `@Service` : ��� `@Service`�� Ư���� ó���� ���� �ʴ´�. ��� �����ڵ��� �ٽ� ����Ͻ� ������ ���⿡ �ְڱ��� ��� ����Ͻ� ������ �ν��ϴµ� ������ �ȴ�.

  > ���� : `useDefaultFilters` �ɼ��� �⺻���� �����ִµ�, �� �ɼ��� ���� �⺻ ��ĵ ������ ���ܵȴ�. 

---

### ����

- `includeFilters` : ������Ʈ ��ĵ ����� �߰��� ����.
- `excludeFilters` : ������Ʈ ��ĵ���� ������ ����� ����.

```java
@Configuration
@ComponentScan(
    includeFilters = @Filter(type = FilterType.ANNOTATION, classes = MyIncludeComponent.class),
    excludeFilters = @Filter(type = FilterType.ANNOTATION, classes = MyExcludeComponent.class)
)
```
- `includeFilters`�� `MyIncludeComponent` �ֳ����̼��� �߰��ؼ� BeanA�� ������ �� ��ϵȴ�.
- `excludeFilters`�� `MyExcludeComponent` �ֳ����̼��� �߰��ؼ� BeanB�� ������ �� ��ϵ��� �ʴ´�.

FilterType �ɼ��� 5���� �ɼ��� �ִ�.
- ANNOTATION : �⺻��, �ֳ����̼��� �ν��ؼ� �����Ѵ�.
  - ex> `org.example.SomeAnnotation`
- ASSIGNABLE_TYPE : ������ Ÿ�԰� �ڽ� Ÿ���� �ν��ؼ� �����Ѵ�.
  - ex> `org.example.SomeClass`
- ASPECTJ: AspectJ ���� ���
  - ex> `org.example..*Service+`
- REGEX : ���� ǥ����
  - ex> `org\.example\.Default.*`
- CUSTOM : `TypeFilter`�̶�� �������̽��� �����ؼ� ó��
  - ex> `org.example.MyTypeFilter`


������ `BeanA`�� ���� ������ �Ʒ��� ���� �ڵ� �ۼ�.
```java
@ComponentScan(
  includeFilters = {
    @Filter(type = FilterType.ANNOTATION, classes = MyIncludeComponent.class),
  },
  excludeFilters = {
    @Filter(type = FilterType.ANNOTATION, classes = MyExcludeComponent.class),
    @Filter(type = FilterType.ASSIGNABLE_TYPE, classes = BeanA.class)
  }
)
```
>���� : `@Component` �� ����ϱ� ������, `includeFilters`�� ����� ���� ���� ����. `excludeFilters`�� �������� ������ ��Ȥ ����� ���� ������ ������ �ʴ�.<br>
Ư�� �ֱ� ������ ��Ʈ�� ������Ʈ ��ĵ�� �⺻���� �����ϴµ�, ���������δ� �ɼ��� �����ϸ鼭 ����ϱ� ���ٴ� �������� �⺻ ������ �ִ��� ���߾� ����ϴ� ���� �����ϰ�, ��ȣ�ϴ� ���̴�.

---

### �ߺ� ��ϰ� �浹

������Ʈ ��ĵ���� ���� �� �̸��� ����ϸ� ������ ���� �ΰ��� ��Ȳ�� �ִ�.

1. �ڵ� �� ��� vs �ڵ� �� ���
2. ���� �� ��� vs �ڵ� �� ���


�ڵ� �� ��� vs �ڵ� �� ���
- ������Ʈ ��ĵ�� ���� �ڵ����� ������ ���� ��ϵǴµ�, �� �̸��� ���� ��� �������� ������ �߻���Ų��.
  - `ConflictingBeanDefinitionException` ���� �߻�

���� �� ��� vs �ڵ� �� ���


```java
@Component
public class MemoryMemberRepository implements MemberRepository{
```

```java
@Configuration
@ComponentScan(
        basePackages = "hello.core.member",
        excludeFilters = @ComponentScan.Filter(type= FilterType.ANNOTATION, classes = Configuration.class)
)
public class AutoAppConfig {

    @Bean(name = "memoryMemberRepository")
    MemberRepository memberRepository(){
        return new MemoryMemberRepository();
    }
}
```

�� ��� ���� �� ����� �켱���� ������.(���� ���� �ڵ� ���� �������̵� �ع�����.)

**���� �� ��Ͻ� ���� �α�**
```text
Overriding bean definition for bean 'memoryMemberRepository' with a different definition: replacing ....
```
�����ڰ� �ǵ��ߴٸ� ����������, ������ �����ڰ� �ǵ������� �����ؼ� �̷� ����� ��������� ���ٴ� ���� �������� ������ �̷� ����� ��������� ��찡 ��κ��̴�.<br>
**�׷��� ���� ��� ����� ���װ� ���������. �׻� ��� ����� ���״� �ָ��� ���״�**<br>
�׷��� �ֱ� ������ ��Ʈ������ ���� �� ��ϰ� �ڵ� �� ����� �浹���� ������ �߻��ϵ��� �⺻ ���� �ٲپ���.

---
---

## �������� �ڵ� ����

---
---

### �پ��� �������� ���� ���

�������� ������ ũ�� 4���� ����� �ִ�.
- ������ ����
- ������ ����(setter ����)
- �ʵ� ����
- �Ϲ� �޼��� ����

������ ����
- �̸� �״�� �����ڸ� ���ؼ� ���� ���踦 ���� �޴� ���.
- ���ݱ��� �츮�� �����ߴ� ����� �ٷ� ������ ����.
- Ư¡
  - ������ ȣ������� �� 1���� ȣ��Ǵ� ���� ����.
  - **�Һ�, �ʼ�** �������迡 ���
  - 
  ```java
  @Component
  public class OrderServiceImpl implements OrderService{
    private final MemberRepository memberRepository;
    private final DiscountPolicy discountPolicy;

    @Autowired
    public OrderServiceImpl(MemberRepository memberRepository, DiscountPolicy discountPolicy) {
        this.memberRepository = memberRepository;
        this.discountPolicy = discountPolicy;
    }
  }
  ```
    - ������ : ���� �ѹ� �Ҵ�ǰŴ� �ٲ�� �ȵ�.
    - private final : �ʼ������� ���� ������
    
  **�߿�! �����ڰ� �� 1���� ������ @Autowired�� �����ص� �ڵ� ���� �ȴ�.** ���� ������ �󿡸� �ش��Ѵ�.

������ ����(setter ����)
- setter�� �Ҹ��� �ʵ��� ���� �����ϴ� ������ �޼��带 ���ؼ� �������踦 �����ϴ� ���.
- Ư¡
  - **����, ����** ���ɼ��� �ִ� �������迡 ���
  - �ڹٺ� ������Ƽ �Ծ��� ������ �޼��� ����� ����ϴ� ����̴�.
  - 
  ```java
  @Component
  public class OrderServiceImpl implements OrderService{
      private MemberRepository memberRepository;
      private DiscountPolicy discountPolicy;

      @Autowired
      public void setMemberRepository(MemberRepository memberRepository) {
          this.memberRepository = memberRepository;
      }

      @Autowired
      public void setDiscountPolicy(DiscountPolicy discountPolicy) {
          this.discountPolicy = discountPolicy;
      }
  }
  ```
    - ���࿡ MemberRepository�� ������ �� ����� �ȵǾ�������쿡�� ����� �� �ִ�.
  > ���� : `@Autowired`�� �⺻ ������ ������ ����� ������ ������ �߻��Ѵ�. ������ ����� ��� �����ϰ� �Ϸ��� `@Autowired(required = false)` �� �����ϸ� �ȴ�.  

  > ���� : �ڹٺ� ������Ƽ, �ڹٿ����� ���ź��� �ʵ��� ���� ���� �������� �ʰ�, setXxx, getXxx��� �޼��带 ���ؼ� ���� �аų� �����ϴ� ��Ģ�� ������µ�, �װ��� �ڹٺ� ������Ƽ �Ծ��̴�.

    - ex >
      ```java
      Class Data{
        private int age;
        public void setAge(int age){
          this.age = age;
        }

        public int getAge(){
          return age;
        }
      }
      ```

�ʵ� ����
- �̸� �״�� �ʵ忡 �ٷ� �����ϴ� ���.
- Ư¡
  - �ڵ尡 ������������ �ܺο��� ������ �Ұ����ؼ� �׽�Ʈ �ϱ� �����.
  - DI �����ӿ�ũ�� ������ �ƹ��͵� �� �� ����.
  - ������� ����!!
  - ����ص� �Ǵ� ��
    - ���ø����̼��� ���� �ڵ�� ���� ���� �׽�Ʈ �ڵ�
    - ������ ������ �������� �ϴ� `@Configuration` ���� �������� Ư���� �뵵�� ���
  ```java
  @Componet
  public class OrderServiceImpl implements OrderService{
    @Autowired
    private MemberRepository memberRepository;
    @Autowired
    private DiscountPolicy discountPolicy;
  }
  ``` 

�Ϲ� �޼��� ����
- �Ϲ� �޼��带 ���ؼ� ���� ���� �� �ִ�.
- Ư¡
  - �ѹ��� ���� �ʵ带 ���� ���� �� �ִ�.
  - �Ϲ������� �� ������� �ʴ´�.
  - 
    ```java
    @Component
    public class OrderServiceImpl implements OrderService{
      private MemberRepository memberRepository;
      private DiscountPolicy discountPolicy;

      @Autowired
      public void init(MemberRepository memberRepository, DiscountPolicy discountPolicy){
        this.memberRepository = memberRepository;
        this.discountPolicy = discountPolicy;
      }
    }
    ```
  > ���� : �������� �ڵ� ������ ������ �����̳ʰ� �����ϴ� ������ ���̾�� �����Ѵ�. ������ ���� �ƴ� `Member`�� ���� Ŭ�������� `@Autowired` �ڵ带 �����ص� �ƹ� ��ɵ� �������� �ʴ´�.

---

### �ɼ� ó��

������ ������ ���� ��� �����ؾ� �� ���� �ִ�.
�׷��� `@Autowired`�� ����ϸ� `required`�ɼ��� �⺻���� `true`�� �Ǿ� �־ �ڵ� ���� ����� ������ ������ �߻��Ѵ�.

�ڵ� ���� ����� �ɼ����� ó���ϴ� ����� ������ ����.
- `@Autowired(required=false)` : �ڵ� ������ ����� ������ ������ �޼��� ��ü�� ȣ�� �ȵ�.
- `org.springframework.lang.@Nullable` : �ڵ� ������ ����� ������ null�� �Էµȴ�.
- `Optional<>` : �ڵ� ������ ����� ������ `Optional.empty`�� �Էµȴ�.

```java
static class TestBean{

    @Autowired(required = false)
    public void setNoBean1(Member noBean1){
        System.out.println("noBean1 = " + noBean1);
    }

    @Autowired
    public void setNoBean2(@Nullable Member noBean2){
        System.out.println("noBean2 = " + noBean2);
    }

    @Autowired
    public void setNoBean3(Optional<Member> noBean3){
        System.out.println("noBean3 = " + noBean3);
    }
}
```
- **Member�� ������ ���� �ƴϴ�**
- `setNoBean1()`�� `@Autowired(required=false)` �̹Ƿ� ȣ�� ��ü�� �ȵȴ�.

��°��
>setNoBean2 = null<br>
setNoBean3 = Optional.empty

>���� : @Nullable, Optional�� ������ ���ݿ� ���ļ� �����ȴ�. ���� �� ������ �ڵ� ���Կ��� Ư�� �ʵ忡�� ����ص� �ȴ�.

---

### ������ ������ �����ض�!

���ſ��� ������ ���԰� �ʵ� ������ ���� ���������, �ֱٿ��� �������� ������ DI �����ӿ�ũ ��κ��� **������ ������ ����**�Ѵ�. �� ������ ������ ����.

**�Һ�**
- ��κ��� �������� ������ �ѹ� �Ͼ�� ���ø����̼� ����������� �������踦 ������ ���� ����. ������ ��κ��� ��������� ���ø����̼� ���� ������ ���ϸ� �ȵȴ�.(�Һ��ؾ� �Ѵ�)
- ������ ������ ����ϸ�, setXxx �޼��带 public���� ����ξ�� �Ѵ�.
- ������ �Ǽ��� ������ �� �� �ְ�, �����ϸ� �ȵǴ� �޼��带 ����δ� ���� ���� ���� ����� �ƴϴ�.
- ������ ������ ��ü�� ������ �� �� 1���� ȣ��ǹǷ� ���Ŀ� ȣ��Ǵ� ���� ����. ���� �Һ��ϰ� ������ �� �ִ�.

**���� ����**
�����ӿ�ũ ���� ������ �ڹ� �ڵ带 ���� �׽�Ʈ �ϴ� ��쿡 ������ ���� ������ ���������� ���
```java
public class OrderServiceImpl implements OrderService{
  private MemberRepository memberRepository;
  private DiscountPolicy discountpolicy;

  @Autowired
  public void setMemberRepository(MemberRepository memberRepository){
    this.memberRepository = memberRepository;
  }
  @Autowired
  public void setDiscountPolicy(DiscountPolicy discountPolicy){
    this.discountPolicy = discountPolicy;
  }
} 
```
- `Autowired`�� �����ӿ�ũ �ȿ��� ������ ���� �������谡 ������ ������ �߻�������, ������ �����ӿ�ũ ���� ������ �ڹ� �ڵ�θ� ���� �׽�Ʈ�� �����ϰ� �ִ�.

�̷��� �׽�Ʈ�� �����ϸ� ������ �ȴ�.
```java
@Test
void createOrder(){
  OrderServiceImpl orderService = new OrderServiceImpl();
  orderService.createOrder(1L,"itemA",10000);
}
```
�׷��� ���� ���� ����� NPE(Null Pointer Exception)�� �߻��ϴµ�, memberRepository, discountPolicy ��� �������� ������ �����Ǿ��� �����̴�.

������ ������ ����ϸ� ����ó�� ���� �����͸� ���� ���� �� **������ ����**�� �߻��Ѵ�.<br>
�׸��� IDE���� �ٷ� � ���� �ʼ��� �����ؾ� �ϴ��� �� �� �ִ�.

```java
@Test
void create(){
  OrderServiceImpl orderService = new OrderServiceImpl();
  orderService.createOrder(1L,"itemA",10000);
}
```
 
**final Ű����**
������ ������ ����ϸ� �ʵ忡 `final` Ű���带 ����� �� �ִ�. �׷��� �����ڿ��� Ȥ�ö� ���� �������� �ʴ� ������ ������ ������ �����ش�. ���� �ڵ带 ����.
```java
@Component
public class OrderServiceImpl implements OrderService{
  private final MemberRepository memberRepository;
  private final DiscountPolicy discountPolicy;

  @Autowired
  public OrderServiceImpl(MemberRepository memberRepository, DiscountPolicy discountPolicy){
    this.memberRepository = memberRepository;
  }
}
```
- �� ���� �ʼ� �ʵ��� `discountPolicy`�� ���� �����ؾ� �ϴµ�, �� �κ��� �����Ǿ���. �ڹٴ� ������ ������ ���� ������ �߻���Ų��.
- `java: variable discountPolicy might not have been initialized`
- **������ ������ ���󿡼� ���� ������, ���� ������!**

> ���� : ������ ������ ������ ������ ���� ����� ��� ������ ���Ŀ� ȣ��ǹǷ�, �ʵ忡 `final` Ű���带 ����� �� ����. ���� ������ ���� ��ĸ� `final` Ű���带 ����� �� �ִ�.


**����**
- ������ ���� ����� �����ϴ� ������ ���������� ������, �����ӿ�ũ�� �������� �ʰ�, ������ �ڹ� ����� Ư¡�� �� �츮�� ����̱⵵ �ϴ�.
- �⺻���� ������ ������ ����ϰ�, �ʼ� ���� �ƴ� ��쿡�� ������ ���� ����� �ɼ����� �ο��ϸ� �ȴ�. ������ ���԰� ������ ������ ���ÿ� ����� �� ����.
- �׻� ������ ������ �����ض�! �׸��� ���� �ɼ��� �ʿ��ϸ� ������ ������ �����ض�. �ʵ� ������ ������� �ʴ°� ����.

---

### �Һ��� �ֽ� Ʈ����

���� ������ �غ���, ��κ��� �� �Һ��̰�, �׷��� ������ ���� �����ڿ� final Ű���带 ����ϰ� �ȴ�. <br>
�׷��� �����ڵ� ������ �ϰ�, ���� ���� ���� �����ϴ� �ڵ嵵 ������ �ϰ�... <br>
�ʵ� ����ó�� �� ���ϰ� ����ϴ� ����� ������? 

1. `build.gradle`�� ���̺귯�� �� ȯ�� �߰�
2. File->Settings -> plugin -> lombok �˻� ��ġ ����
3. File->Settings -> Annotation Processors �˻� -> Enable annotation processing üũ
4. ������ �׽�Ʈ Ŭ������ ����� @Getter, @Setter Ȯ��

`@RequiredArgsConstructor`
- `final`�� ���� �ʵ带 ��Ƽ� �����ڸ� �ڵ����� ������ش�.
- �ڵ尡 ���� ����������.
- �Һ��� �ڹ��� �ֳ����̼� ���μ������ ����� �̿��ؼ� ������ ������ ������ �ڵ带 �ڵ����� �������ش�. ���� `class`�� ����� ���� �ڵ尡 �߰��Ǿ� �ִ� ���� Ȯ���� �� �ִ�.

**����**
�ֱٿ��� �����ڸ� �� 1�� �ΰ�, `@Autowired`�� �����ϴ� ����� �ַ� ����Ѵ�. ���⿡ Lombok ���̺귯���� `@RequiredArgsConstructor` �Բ� ����ϸ� ����� �� �����ϸ鼭, �ڵ�� ����ϰ� ����� �� �ִ�.

---

### ��ȸ ���� 2�� �̻� - ����

`@Autowired`��  Ÿ��(Type)���� ��ȸ�Ѵ�.
```java
@Autowired
private DiscountPolicy discountPolicy
```
Ÿ������ ��ȸ�ϱ� ������, ��ġ ���� �ڵ�� �����ϰ� ����.
`ac.getBean(DiscountPolicy.class)`

������ �� ��ȸ�ؼ� �н��ߵ��� Ÿ������ ��ȸ�ϸ� ���õ� ���� 2�� �̻��� �� ������ �߻��Ѵ�.<br>
`DiscountPolicy`�� ���� Ÿ���� `FixDiscountPolicy`, `RateDiscountPolicy` �Ѵ� ������ ������ �����غ���.

```java
@Component
public class FixDiscountPolicy implements DiscountPolicy()
```
```java
@Component
public class RateDiscountPolicy implements DiscountPolicy()
```

`NoUniqueBeanDefinitionException` ���� �߻�.

�����޽��������� `fixDiscountPolicy`,`rateDiscountPolicy` 2���� �߰ߵǾ��ٰ� ���Ѵ�.

�̶� ���� Ÿ������ ������ ���� ������, ���� Ÿ������ �����ϴ� ���� DIP�� �����ϰ� �������� ��������. �׸��� �̸��� �ٸ���, ������ �Ȱ��� Ÿ���� ������ ���� 2�� ���� �� �ذ��� �ȵȴ�.

������ ���� ���� ����ؼ� ������ �ذ��ص� ������, ���� ���� �ڵ� ���Կ��� �ذ��ϴ� ���� ����� �ִ�.

---

### @Autowired �ʵ� ��, @Qualifier, @Primary

��ȸ ��� ���� 2�� �̻��� �� �ذ� ���
- @Autowired �ʵ� �� ��Ī
- @Quilifer -> @Quilifier�� �Ӹ�Ī -> �� �̸� ��Ī
- @Primary ���

@Autowired �ʵ� �� ��Ī

- `@Autowired`�� Ÿ�� ��Ī�� �õ��ϰ�, �̶� ���� ���� ������ �ʵ� �̸�, �Ķ���� �̸����� �� �̸��� �߰� ��Ī�Ѵ�.

- �����ڵ�
```java
@Autowired
private DiscountPolicy discountPolicy
```

- �ʵ� ���� �� �̸����� ����
```java
Autowired
private DiscountPolicy rateDiscountPolicy
```

�ʵ� ���� `rateDiscountPolicy`�̹Ƿ� ���� ���Եȴ�.<br>
**�ʵ� �� ��Ī�� ���� Ÿ�� ��Ī�� �õ� �ϰ� �� ����� ���� ���� ���� �� �߰��� �����ϴ� ����̴�.**

**Autowired ��Ī ����**
1. Ÿ�� ��Ī
2. Ÿ�� ��Ī�� ����� 2�� �̻��� �� �ʵ� ��, �Ķ���� ������ �� �̸� ��Ī

@Quilifier ���
`Quilifier`�� �߰� �����ڸ� �ٿ��ִ� ����̴�. ���Խ� �߰����� ����� �����ϴ� ������ �� �̸��� �����ϴ� ���� �ƴϴ�.

**�� ��Ͻ� @Qualifier�� �ٿ� �ش�**
```java
@Component
@Qualifier("mainDiscountPolicy")
public class RateDiscountPolicy implements DiscountPolicy{}
```
```java
@Component
@Qualifier("fixDiscountPolicy")
public class FixDiscountPolicy implements DiscountPolicy{}
```

**���Խÿ� @Qualifier�� �ٿ��ְ� ����� �̸��� �����ش�.**

**������ �ڵ� ���� ����**
```java
@Autowired
public OrderServiceImpl(MemberRepository memberRepository, @Qualifier("mainDiscountPolicy") DiscountPolicy discountPolicy){
  this.memberRepository = memberRepository;
  this.discountPolicy = discountPolicy;
}
```

**������ �ڵ� ���� ����**
```java
@Autowired
public DiscountPolicy setDiscountPolicy(@Qualifier("mainDiscountPolicy") DicounstPolicy discountPolicy){
  return discountPolicy;
}
```

`@Qualifier`�� ������ �� `@Qulifier("mainDiscountPolicy")`�� ��ã���� ��� �ɱ�? �׷��� mainDiscountPolicy��� �̸��� ������ ���� �߰��� ã�´�. ������ ����� `@Qualifier`�� `@Qulifier`�� ã�� �뵵�θ� ����ϴ°� ��Ȯ�ϰ� ����.

������ ���� ���� �� ��Ͻÿ��� @Qualifier�� �����ϰ� ����� �� �ִ�.
```java
@Bean
@Qualifier("mainDiscountPolicy")
public DiscountPolicy discountPolicy(){
  return new...
}
```

**@Qualifier ����**
1. @Qualifier���� ��Ī
2. �� �̸� ��Ī
3. `NosuchBeanDefinitionException` ���� �߻�

**@Primary ���**
`@Primary`�� �켱������ ���ϴ� ����̴�. @Autowired �ÿ� ���� �� ��Ī�Ǹ� `@Primary`�� �켱���� ������.

main DB(90%)�� ���� DB(10%)�� �ִٰ� �����ϰ�, main DB�� �������� Ŀ�ؼ��� �Ҷ����� Qualifier�� ���ְ�, ���� DB�� �����ö��� Qualifier�ϱ⿡�� ������. �׷��� main DB �������� �ڵ忡�� `@Primary`�� �ɾ��ش�. 

`@Qualifier`�� ������ ���� ���� �� ��� �ڵ忡 `@Qualifier`�� �ٿ��־�� �Ѵٴ� ���̴�.

�ݸ鿡 `@Primary`�� `@Qualifer`�� ���� �ʿ䰡 ����.

**@Primary, @Qualifier Ȱ��**
�ڵ忡�� ���� ����ϴ� ���� db�� Ŀ�ؼ��� ȹ���ϴ� ������ ���� �ְ�, �ڵ忡�� Ư���� ������� ���� ����ϴ� ���� db�� Ŀ�ؼ��� ȹ���ϴ� ������ ���� �ִٰ� �����غ���. ���� db�� Ŀ�ؼ��� ȹ���ϴ� ������ ���� `@Primary`�� �����ؼ� ��ȸ�ϴ� ������ `@Qualifier` ���� ���� ���ϰ� ��ȸ�ϰ�, ���� db Ŀ�ؼ� ���� ȹ�� �� ���� `@Qualifer`�� �����ؼ� ��������� ȹ�� �ϴ� ������� ����ϸ� �ڵ带 ����ϰ� ������ �� �ִ�. ���� �̶� ���� db�� ������ ���� ����� ��, `Qualifier`�� �������ִ� ���� �������.

**�켱����**
`@Primary`�� �⺻�� ó�� �����ϴ� ���̰�, `@Qualifier`�� �ſ� ���ϰ� �����Ѵ�. �̷� ��� � ���� �켱���� ��������? �������� �ڵ����ٴ� ������, ���� ������ ���ñ� ���ٴ� ���� ������ ���ñ��� �켱 ������ ����. ���� ���⼭�� `@Qualifier`�� �켱���� ����.

---

### �ֳ����̼� ���� �����

`@Qualifier("mainDiscountPolicy")` �̷��� ���ڸ� ������ �����Ͻ� Ÿ�� üũ�� �ȵȴ�. ������ ���� �ֳ����̼��� ���� ������ �ذ��� �� �ִ�.
```java
@Compoent
@MainDiscountPolicy
public class RateDiscountPolicy implements DiscountPolicy{}
```

�ֳ����̼ǿ��� ����̶�� ������ ����. �̷��� ���� �ֳ����̼��� ��Ƽ� ����ϴ� ����� �������� �������ִ� ����̴�. @Qulifier �Ӹ� �ƴ϶� �ٸ� �ֳ����̼ǵ鵵 �Բ� �����ؼ� ����� �� �ִ�. �������� @Autowired�� ������ �� �� �ִ�. ���� �������� �����ϴ� ����� �ѷ��� ���� ���� ���к��ϰ� ������ �ϴ� ���� ���������� �� ȥ���� ������ �� �ִ�.


---
---

## IntelliJ ����Ű ������ & ����
- �⺻������ `Preferences -> keymap` ���� �� �� ������ ����ϰ����ϴ� ����Ű �̸��� �Է��ϸ� ȯ�濡 �°�(window,mac..) ����Ű�� ����
- Preferences(or Settings) �ٷΰ��� : `ctrl+alt+s`
- Generate(������,Getter,Setter ��...) : `alt+insert` (������ ��� alt+function+delete)
- `Compact middle Package`
- �ڵ��ϼ�(�����ݷб��� �����ؼ�) : `ctrl+shift+enter`
- public static void main(String[] args) ���� : `psvm + enter`
- �� �����ؼ� ������ �ֱ� : `ctrl+alt+v`
- Print a value to System.out : `soutv+enter`
- main������ �Լ����� test �ٷ� �����ϱ�: `ctrl+shift+t`
- test�� �Ҷ� Assertions�� static import�ϴ°� ���� : `Assertions Ŀ�� �ΰ� +alt+enter+(on demand static~~)`
- ���� history ���� : `ctrl+e`
- Extract Method : `ctrl+alt+m`
- ����Ʈ�� �迭�� ������ for �ڵ� ����,iterator() : `iter+tab`
- �˻� : `ctrl+n`


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
    - [���ɻ��� �и�](#���ɻ���-�и�)
      - [����](#����)
    - [AppConfig �����͸�](#appconfig-�����͸�)
    - [���ο� ������ ���� ��å ����](#���ο�-������-����-��å-����)
    - [���� ��ü ���� ������ 5���� ��Ģ�� ����](#����-��ü-����-������-5����-��Ģ��-����)
    - [IoC, DI, �׸��� �����̳�](#ioc-di-�׸���-�����̳�)
    - [���������� ��ȯ�ϱ�](#����������-��ȯ�ϱ�)
  - [������ �����̳ʿ� ������ ��](#������-�����̳ʿ�-������-��)
    - [������ �����̳� ����](#������-�����̳�-����)
    - [�����̳ʿ� ��ϵ� ��� �� ��ȸ](#�����̳ʿ�-��ϵ�-���-��-��ȸ)
    - [������ �� ��ȸ - �⺻](#������-��-��ȸ---�⺻)
    - [������ �� ��ȸ - ������ Ÿ���� �� �̻�](#������-��-��ȸ---������-Ÿ����-��-�̻�)
    - [������ �� ��ȸ - ��� ����](#������-��-��ȸ---���-����)
    - [BeanFactory�� ApplicationContext](#beanfactory��-applicationcontext)
    - [�پ��� ���� ���� ���� - �ڹ� �ڵ� ,XML](#�پ���-����-����-����---�ڹ�-�ڵ�-xml)
    - [������ �� ���� ��Ÿ ���� - BeanDefinition](#������-��-����-��Ÿ-����---beandefinition)
  - [�̱��� �����̳�](#�̱���-�����̳�)
    - [�� ���ø����̼ǰ� �̱���](#��-���ø����̼ǰ�-�̱���)
    - [�̱��� ����](#�̱���-����)
    - [�̱��� �����̳�](#�̱���-�����̳�-1)
    - [�̱��� ����� ������](#�̱���-�����-������)
    - [@Configuration�� �̱���](#configuration��-�̱���)
    - [@Configuration�� ����Ʈ�ڵ� ������ ����](#configuration��-����Ʈ�ڵ�-������-����)
  - [������Ʈ ��ĵ](#������Ʈ-��ĵ)
    - [������Ʈ ��ĵ�� �������� �ڵ� ���� �����ϱ�](#������Ʈ-��ĵ��-��������-�ڵ�-����-�����ϱ�)
    - [Ž�� ��ġ�� �⺻ ��ĵ ���](#Ž��-��ġ��-�⺻-��ĵ-���)
    - [����](#����)
    - [�ߺ� ��ϰ� �浹](#�ߺ�-��ϰ�-�浹)
  - [�������� �ڵ� ����](#��������-�ڵ�-����)
    - [�پ��� �������� ���� ���](#�پ���-��������-����-���)
    - [�ɼ� ó��](#�ɼ�-ó��)
    - [������ ������ �����ض�!](#������-������-�����ض�)
    - [�Һ��� �ֽ� Ʈ����](#�Һ���-�ֽ�-Ʈ����)
    - [��ȸ ���� 2�� �̻� - ����](#��ȸ-����-2��-�̻�---����)
    - [@Autowired �ʵ� ��, @Qualifier, @Primary](#autowired-�ʵ�-��-qualifier-primary)
    - [�ֳ����̼� ���� �����](#�ֳ����̼�-����-�����)
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
    - [���ɻ��� �и�](#���ɻ���-�и�)
      - [����](#����)
    - [AppConfig �����͸�](#appconfig-�����͸�)
    - [���ο� ������ ���� ��å ����](#���ο�-������-����-��å-����)
    - [���� ��ü ���� ������ 5���� ��Ģ�� ����](#����-��ü-����-������-5����-��Ģ��-����)
    - [IoC, DI, �׸��� �����̳�](#ioc-di-�׸���-�����̳�)
    - [���������� ��ȯ�ϱ�](#����������-��ȯ�ϱ�)
  - [������ �����̳ʿ� ������ ��](#������-�����̳ʿ�-������-��)
    - [������ �����̳� ����](#������-�����̳�-����)
    - [�����̳ʿ� ��ϵ� ��� �� ��ȸ](#�����̳ʿ�-��ϵ�-���-��-��ȸ)
    - [������ �� ��ȸ - �⺻](#������-��-��ȸ---�⺻)
    - [������ �� ��ȸ - ������ Ÿ���� �� �̻�](#������-��-��ȸ---������-Ÿ����-��-�̻�)
    - [������ �� ��ȸ - ��� ����](#������-��-��ȸ---���-����)
    - [BeanFactory�� ApplicationContext](#beanfactory��-applicationcontext)
    - [�پ��� ���� ���� ���� - �ڹ� �ڵ� ,XML](#�پ���-����-����-����---�ڹ�-�ڵ�-xml)
    - [������ �� ���� ��Ÿ ���� - BeanDefinition](#������-��-����-��Ÿ-����---beandefinition)
  - [�̱��� �����̳�](#�̱���-�����̳�)
    - [�� ���ø����̼ǰ� �̱���](#��-���ø����̼ǰ�-�̱���)
    - [�̱��� ����](#�̱���-����)
    - [�̱��� �����̳�](#�̱���-�����̳�-1)
    - [�̱��� ����� ������](#�̱���-�����-������)
    - [@Configuration�� �̱���](#configuration��-�̱���)
    - [@Configuration�� ����Ʈ�ڵ� ������ ����](#configuration��-����Ʈ�ڵ�-������-����)
  - [������Ʈ ��ĵ](#������Ʈ-��ĵ)
    - [������Ʈ ��ĵ�� �������� �ڵ� ���� �����ϱ�](#������Ʈ-��ĵ��-��������-�ڵ�-����-�����ϱ�)
    - [Ž�� ��ġ�� �⺻ ��ĵ ���](#Ž��-��ġ��-�⺻-��ĵ-���)
    - [����](#����)
    - [�ߺ� ��ϰ� �浹](#�ߺ�-��ϰ�-�浹)
  - [�������� �ڵ� ����](#��������-�ڵ�-����)
    - [�پ��� �������� ���� ���](#�پ���-��������-����-���)
    - [�ɼ� ó��](#�ɼ�-ó��)
    - [������ ������ �����ض�!](#������-������-�����ض�)
    - [�Һ��� �ֽ� Ʈ����](#�Һ���-�ֽ�-Ʈ����)
    - [��ȸ ���� 2�� �̻� - ����](#��ȸ-����-2��-�̻�---����)
    - [@Autowired �ʵ� ��, @Qualifier, @Primary](#autowired-�ʵ�-��-qualifier-primary)
    - [�ֳ����̼� ���� �����](#�ֳ����̼�-����-�����)
  - [IntelliJ ����Ű ������ & ����](#intellij-����Ű-������--����)
  - [����(�ٷΰ���)](#�����ٷΰ���)