# ������ MVC 1�� - �鿣�� �� ���� �ٽ� ���

---
---

## ����

- [������ MVC 1�� - �鿣�� �� ���� �ٽ� ���](#������-mvc-1��---�鿣��-��-����-�ٽ�-���)
  - [����](#����)
  - [�� ���ø����̼� ����](#��-���ø����̼�-����)
    - [�� ����, �� ���ø����̼� ����](#��-����-��-���ø����̼�-����)
    - [����](#����)
    - [���� ��û - ��Ƽ ������](#����-��û---��Ƽ-������)
    - [HTML, HTTP API, CSR, SSR](#html-http-api-csr-ssr)
    - [�ڹ� �鿣�� �� ��� ����](#�ڹ�-�鿣��-��-���-����)
  - [����](#����-1)
    - [������Ʈ ����](#������Ʈ-����)
    - [Hello ����](#hello-����)
    - [HttpServletRequest - ����](#httpservletrequest---����)
    - [HTttpServletRequest - �⺻ ����](#htttpservletrequest---�⺻-����)
    - [HTTP ��û ������ - ����](#http-��û-������---����)
    - [HTTP ��û ������ - GET ���� �Ķ����](#http-��û-������---get-����-�Ķ����)
    - [HTTP ��û ������ - POST HTML Form](#http-��û-������---post-html-form)
    - [HTTP ��û ������ - API �޽��� �ٵ� - �ܼ� �ؽ�Ʈ](#http-��û-������---api-�޽���-�ٵ�---�ܼ�-�ؽ�Ʈ)
    - [HTTP ��û ������ - API �޽��� �ٵ� - JSON](#http-��û-������---api-�޽���-�ٵ�---json)
    - [HttpServletResponse - �⺻ ����](#httpservletresponse---�⺻-����)
    - [HTTP ���� ������ - �ܼ� �ؽ�Ʈ, HTML](#http-����-������---�ܼ�-�ؽ�Ʈ-html)
    - [HTTP ���� ������ - API JSON](#http-����-������---api-json)
  - [����, JSP, MVC ����](#����-jsp-mvc-����)
    - [ȸ�� ���� �� ���ø����̼� �䱸����](#ȸ��-����-��-���ø����̼�-�䱸����)
    - [�������� ȸ�� ���� �� ���ø����̼� �����](#��������-ȸ��-����-��-���ø����̼�-�����)
    - [JSP�� ȸ�� ���� �� ���ø����̼� �����](#jsp��-ȸ��-����-��-���ø����̼�-�����)
    - [MVC ���� - ����](#mvc-����---����)
    - [MVC ���� - ����](#mvc-����---����)


---
---

## �� ���ø����̼� ����

---
---

### �� ����, �� ���ø����̼� ����

�� - HTTP ��� ����̴�.

- �� ���������� URL�� ġ�� ���ͳ��� ���ؼ� server�� �����ϰ� server������ HTML�� ���� client�� �����ְ� �� �������� ���� HTML�� ������ �츮���� �����ش�.

- client���� server�� �����͸� �����Ҷ�, server���� client�� �����͸� ������ ��, �̶� HTTP protocol ������� ������.

��� ���� �������� HTTP������� �����͸� �ְ� ����
- HTML,TXT
- IMAGE,����,����,����
- JSON,XML(API)
- ���� ��� ������ ������ ���� ����
- server�� �����͸� �ְ� ���� ���� ��κ� HTTP ���

�� ����(Web Server)

- HTTP ��� ���� ����
- ���� ���ҽ� ����, ��Ÿ �ΰ���� ����
- ����(����) HTML, CSS, JS, �̹���, ����
- ex> NGINX, APACHE

![webserver](./readme_img/webserver.JPG)

�� ���ø����̼� ����(WAS - Web Application Server)

- HTTP ��� ����
- �� ���� ��� + (���� ���ҽ� ���� ����)
- **���α׷� �ڵ带 �����ؼ� ���ø����̼� ���� ����**
  - ���� HTML, HTTP API(JSON)
  - ����, JSP, ������ MVC
- ex> ��Ĺ(Tomcat) Jetty, Undertow

![WAS](./readme_img/was.JPG)

�� ����, �� ���ø����̼� ����(WAS) ����

- �� ������ ���� ���ҽ�(����), WAS�� ���ø����̼� ����
- ��� ���� �� ��赵 ��ȣ
  - �� ������ ���α׷��� �����ϴ� ����� �����ϱ⵵ ��
  - �� ���ø����̼� ������ �� ������ ����� ������
- �ڹٴ� ���� �����̳� ����� �����ϸ� was
  - ���� ���� �ڹ��ڵ带 �����ϴ� ���� �����ӿ�ũ�� ����
- **WAS�� ���ø����̼� �ڵ带 �����ϴµ� �� Ưȭ**

�� �ý��� ���� - WAS, DB
- WAS, DB ������ �ý��� ���� ����
- WAS�� ���� ���ҽ�, ���ø����̼� ���� ��� ���� ����

- ![websystem](./readme_img/websystem.JPG)

- WAS�� �ʹ� ���� ������ ���, ���� ������ ���
- ���� ��� ���ø����̼� ������ ���� ���ҽ� ������ ������ ����� �� ����
- WAS ��ֽ� ���� ȭ�鵵 ���� �Ұ���

�� �ý��� ���� - WEB, WAS, DB
- ���� ���ҽ��� �� ������ ó��
- �� ������ ���ø����̼� �������� ������ ó���� �ʿ��ϸ� WAS�� ��û�� ����
- WAS�� �߿��� ���ø����̼� ���� ó�� ����
- ![web_was_db](./readme_img/web_was_db.JPG)
  - ���� �д��� ��

- ȿ������ ���ҽ� ����
  - ���� ���ҽ��� ���� ���Ǹ� Web ���� ����
  - ���ø����̼� ���ҽ��� ���� ���Ǹ� WAS ����

- ���� ���ҽ��� �����ϴ� �� ������ �� ���� ����
- ���ø����̼� ������ �����ϴ� WAS ������ �� ����
- WAS, DB ��ֽ� WEB ������ ���� ȭ�� ���� ����
- ![die_was](./readme_img/die_was.JPG)

---

### ����

HTML Form ������ ����
- POST ���� - ����
- ![post](./readme_img/post.JPG)
  - action="/save" -> URL�� �߰�
  - method="post" -> post������� ������ ����
  - �� �� ���� �ְ� ������ ������ �� �������� ������ ��û HTTP �޽����� �������

�������� ó���ؾ� �ϴ� ����
- �� ���ø����̼� ���� ���� �����ؾ� �Ѵٸ�?
  - ���� TCP/IP ���� ���, ���� ����
  - HTTP ��û �޽����� �Ľ��ؼ� �б�
  - POST ���, /save URL ����
  - Content-Type Ȯ��
  - HTTP �޽��� �ٵ� ���� ����
  - ���� ���μ��� ����
  - **����Ͻ� ���� ����(���Ⱑ �ǹ��ִ� ����Ͻ� ����)**
    - **���̶����̽��� ���� ��û**
  - HTTP ���� �޽��� ���� ����
    - HTTP ���� ���� ����
    - Header ����
    - �޽��� �ٵ� HHTML �����ؼ� �Է�
  - TCP/IP�� ���� ����, ���� ����

- ������ �����ϴ� WAS ���
  - ���� �������� ����Ͻ� ���� ���� �κи� ������ ��� ���� �� ��������.

Ư¡
```java
@WebServlet(name = "helloServlet", urlPatterns = "/hello")
public class HelloServlet extends HttpServlet{
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response){
        //���ø����̼� ����
    }
}
```
  - urlPatterns(/hello)�� URL�� ȣ��Ǹ� ���� �ڵ尡 ����
  - HTTP ��û ������ ���ϰ� ����� �� �ִ� HttpServletRequest
  - HTTP ���� ������ ���ϰ� ������ �� �ִ� HttpServletResponse
  - �����ڴ� HTTP ������ �ſ� ���ϰ� ���

![logic](./readme_img/logic.JPG)
- �� ���������� `localhost:8080/hello` ��û
- �׷���, WAS���� HTTP ��û �޽��� ������� request, response ��ü�� ���� ����
- �� ����, helloServlet ����
- helloServlet�� ���ᰡ �Ǹ� response ��ü ������ HTTP ���� ����
- �׸��� �� �������� ���� �޽��� ����

HTTP ��û, ���� �帧
- HTTP ��û��
  - WAS�� Request, Response ��ü�� ���� ���� ���� ��ü ȣ��
  - �����ڴ� Request ��ü���� HTTP ��û ������ ���ϰ� ������ ���
  - �����ڴ� Response ��ü�� HTTP ���� ������ ���ϰ� �Է�
  - WAS�� Response ��ü�� ����ִ� �������� HTTP ���� ������ ����

���� �����̳�
![servlet_container](./readme_img/servlet_container.JPG)
- ������ �����ϴ� WAS�ȿ��� ���� �����̳ʰ� �ִ�.
- ���� �����̳� �ȿ��� ���� ��ü�� ���� �����̳ʰ� �ڵ����� ����, ȣ������.
- �����ֱ� ���� : WAS�� ����ɶ� �� ������ ���� ��������

- ��Ĺó�� ������ �����ϴ� WAS�� `���� �����̳�`��� ��.
- ���� �����̳ʴ� ���� ��ü�� ����, �ʱ�ȭ, ȣ��, �����ϴ� �����ֱ� ����
- ���� ��ü�� **�̱������� ����**
  - ���� ��û�� �� �� ���� ��� ��ü�� �����ϴ� ���� ��ȿ��
  - ���� �ε� ������ ���� ��ü�� �̸� �����ΰ� ��Ȱ��
  - ��� �� ��û�� ������ ���� ��ü �ν��Ͻ��� ����
  - **���� ���� ��� ����**
  - ���� �����̳� ����� �Բ� ����
- JSP�� �������� ��ȯ �Ǿ ���
- **���� ��û�� ���� ��Ƽ ������ ó�� ����**

---

### ���� ��û - ��Ƽ ������

![who_call_servlet](./readme_img/who_servlet.JPG)
- �����尡 ȣ������

������
- ���ø����̼� �ڵ带 �ϳ��ϳ� ���������� �����ϴ� ���� ������
- �ڹ� ���� �޼��带 ó�� �����ϸ� main�̶�� �̸��� �����尡 ����
- �����尡 ���ٸ� �ڹ� ���ø����̼� ������ �Ұ���
- ������� �ѹ��� �ϳ��� �ڵ� ���θ� ����
- ���� ó���� �ʿ��ϸ� �����带 �߰��� ����

���� ��û - ������ �ϳ� ���
- ��û�� �ϳ��� �´�.
- �׷��� ������ �Ҵ�����
- �� �����带 ������ servlet �ڵ带 ��������
- �׸��� �����带 ������ ������ ����
- ������ �ǰ��� �����尡 �޽��� ��.

���� ��û - ������ �ϳ� ���
- ��û1�� ����.
  - �����带 ����ؼ� servlet�� ��û������ ó���� �����ǰ� �ִ�.
- �̶�, ��û2�� ����.
  - �����峭 �ϳ��ۿ� ���µ� ��û1������ ����ϰ� �־ �����带 ��ٷ�����.
- �̷���, 1�� 2�� �� �� �׾����.

��û ���� ������ ����
- ��û1�� ����
  - ������ ����������, ó�� ����
- ��û2�� ����
  - ������ ���� �����ؼ� ó���ϰ� ��û�� ������ ������ �޽�.
- ����
  - ���� ��û�� ó���� �� �ִ�.
  - ���ҽ�(CP, �޸�)�� ����� �� ���� ó������
  - �ϳ��� �����尡 ���� �Ǿ, ������ ������� ���� ����.
- ����
  - ������� ���� ����� ��� ��δ�.
    - ���� ��û�� �� ������ �����带 �����ϸ�, ���� �ӵ��� �ʾ�����.
  - ������� context switching ����� �߻��Ѵ�.
  - ������ ������ ������ ����.
    - �� ��û�� �ʹ� ���� ����, CPU, �޸� �Ӱ����� �Ѿ ������ ���� �� �ִ�.

������ Ǯ
![thread_pool](./readme_img/thread_pool.JPG)
- ������ Ǯ�ȿ� �̸� �������� ��������� ����ִ�.(200����� ����)
- ��û�� �� ������ ������ Ǯ���� �����ٰ� ����, �����带 �� ����ϸ� �����带 ���̴°��� �ƴ� ������ Ǯ�� �ݳ��� �Ѵ�.

![zero](./readme_img/zero_threadpool.JPG)
- ������ Ǯ�� ���̻� �����尡 ���� �� ��û�� ������ ����ϰų� ������ �� �ִ�.

- ��û ���� ������ ������ ���� ����
  - Ư¡
    - �ʿ��� �����带 ������ Ǯ�� �����ϰ� ����.
    - ������ Ǯ�� ���� ������ �������� �ִ�ġ�� ����. ������ �ִ� 200�� �⺻ ����(���� ����)
  - ���
    - �����尡 �ʿ��ϸ�, �̹� �����Ǿ� �ִ� �����带 ������ Ǯ���� ������ ����Ѵ�.
    - ����� �����ϸ� ������ Ǯ�� �ش� �����带 �ݳ��Ѵ�.
    - �ִ� �����尡 ��� ������̾ ������ Ǯ�� �����尡 ���ٸ�?
      - ��ٸ��� ��û�� �����ϰų� Ư�� ���ڸ�ŭ�� ����ϵ��� ������ �� �ִ�.
  - ����
    - �����尡 �̸� �����Ǿ� �����Ƿ�, �����带 �����ϰ� �����ϴ� ���(CPU)�� ����ǰ�, ���� �ð��� ������.
    - ���� ������ �������� �ִ�ġ�� �����Ƿ� �ʹ� ���� ��û�� ���͵� ���� ��û�� �����ϰ� ó���� �� �ִ�.

- �ǹ� ��
  - WAS�� �ֿ� Ʃ�� ����Ʈ�� �ִ� ������(max thread) ���̴�.
  - �� ���� �ʹ� ���� �����ϸ�?
    - ���� ��û�� ������, ���� ���ҽ��� ����������, Ŭ���̾�Ʈ�� �ݹ� ���� ����.
  - �� ���� �ʹ� ���� �����ϸ�?
    - ���� ��û�� ������, CPU, �޸� ���ҽ� �Ӱ��� �ʰ��� ���� �ٿ�
  - ��� �߻���?
    - Ŭ����� �ϴ� �������� �ø���, ���Ŀ� Ʃ��
    - Ŭ���尡 �ƴϸ� ������ Ʃ��

- ������ Ǯ�� ���� ����
  - ���� ���ڴ� ��� ã�°�...?
  - ���ø����̼� ������ ���⵵, CPU, �޸�, IO ���ҽ� ��Ȳ�� ���� ��� �ٸ�
  - ���� �׽�Ʈ
    - �ִ��� ���� ���񽺿� �����ϰ� ���� �׽�Ʈ �õ�
    - ��: ����ġ ab, ���̹���, nGrinder

WAS�� ��Ƽ ������ ����
- �ٽ�
  - ��Ƽ �����忡 ���� �κ��� WAS�� ó��
  - **�����ڰ� ��Ƽ ������ ���� �ڵ带 �Ű澲�� �ʾƵ� ��**
  - �����ڴ� ��ġ **�̱� ������ ���α׷����� �ϵ��� ���ϰ� �ҽ� �ڵ带 ����**
  - ��Ƽ ������ ȯ���̹Ƿ� �̱��� ��ü(����, ������ ��)�� �����ؼ� ���.

---

### HTML, HTTP API, CSR, SSR

���� ���ҽ�
- ������ HTML ����, CSS, JS, �̹���, ���� ���� ����
- �ַ� �� ������
- ![static](./readme_img/static.JPG)

HTML ������
- �������� �ʿ��� html ������ �����ؼ� ����
- �� ������: HTML �ؼ�
- ![html_page](./readme_img/html_page.JPG)
  - �ֹ� ������ ������!
  - WAS(���ø����̼� ������ ������ �� ����)�� DB�� ���ؼ� �ֹ� ���� ��ȸ.
  - �̰��� �������� HTML ����(JSP,Ÿ�Ӹ���...)
  - �������� ������ HTML�� ���������� ������.

HTTP API
- HTML�� �ƴ϶� �����͸� ����
- �ַ� JSON ���� ���
- �پ��� �ý��ۿ��� ȣ��
- ![http_api](./readme_img/http_api.JPG)
- �����͸� �ְ� ����, UI ȭ���� �ʿ��ϸ�, Ŭ���̾�Ʈ�� ���� ó��
- ��, �� Ŭ���̾�Ʈ, ���� to ����
1. �� Ŭ���̾�Ʈ to ����
2. �� Ŭ���̾�Ʈ to ����
3. ���� to ���� 

- �پ��� �ý��� ����
  - �ַ� JSON ���·� ������ ���
  - UI Ŭ���̾�Ʈ ����
    - �� Ŭ���̾�Ʈ(������, �ȵ���̵�, PC ��)
    - �� ���������� �ڹٽ�ũ��Ʈ�� ���� HTTP API ȣ��
    - React, Vue.js ���� �� Ŭ���̾�Ʈ
  - ���� to ����
    - �ֹ� ���� -> ���� ����
    - ����� ������ ���

�������̵� ������, Ŭ���̾�Ʈ ���̵� ������
- SSR - ���� ���̵� ������
  - HTML ���� ����� �������� ���� �� �������� ����
  - �ַ� ������ ȭ�鿡 ���
  - ���ñ�� : JSP, Ÿ�Ӹ��� -> **�鿣�� �Թ���**
  - ![ssr](./readme_img/ssr.JPG)
    - ���������� html�� �������� �� ����.
- CSR - Ŭ���̾�Ʈ ���̵� ������
  - HTML ����� �ڹ� ��ũ��Ʈ�� ����� �� ���������� �������� �����ؼ� ����
  - �ַ� ������ ȭ�鿡 ���, �� ȯ���� ��ġ �� ó�� �ʿ��� �κкκ� ������ �� ����.
  - ex> ���� ����, Gmail, ���� Ķ����
  - ���ñ��: React, Vue.js -> **�� ����Ʈ�ص� ������**
  - ![csr](./readme_img/csr.JPG)
- ����
  - React, Vue.js�� CSR + SSR ���ÿ� �����ϴ� �� �����ӿ�ũ�� ����.
  - SSR�� ����ϴ���, �ڹٽ�ũ��Ʈ�� ����ؼ� ȭ�� �Ϻθ� �������� ���� ����

������ �˾ƾ� �ұ�? �鿣�� ������ ���忡�� UI ���
- �鿣�� - ���� ���̵� ������ ���
  - JSP, Ÿ�Ӹ���
  - ȭ���� �����̰�, �������� ���� �� ���
  - �鿣�� �����ڴ� ���� ���̵� ������ ��� �н� **�ʼ�**
- �� ����Ʈ���� - Ŭ���̾�Ʈ ���̵� ������ ���
  - React, Vue.js
  - �����ϰ� ������ UI ���
  - �� ����Ʈ���� �������� ���� �о�
- ���ð� ����
  - �鿣�� �������� �� ����Ʈ���� ��� �н��� **�ɼ�**
  - �鿣�� �����ڴ� ����, DB, ������ ��� �� ���� �鿣�� ����� �����ؾ��Ѵ�.
  - �� ����Ʈ���嵵 �����ְ� �� �Ϸ��� ���ÿ� ���� �ð��� �ʿ��ϴ�.

---

### �ڹ� �鿣�� �� ��� ����

���� ���
- ���� - 1997
  - html ������ �����
- JSP - 1999
  - HTML ������ ��������, ����Ͻ� �������� �ʹ� ���� ���� ���
- ����, JSP ���� MVC ���� ���
  - ��, ��, ��Ʈ�ѷ��� ������ ������ ����
- MVC �����ӿ�ũ ���� ���� �ô� - 2000�� �� ~ 2010�� ��
  - MVC ���� �ڵ�ȭ, ������ �� ����� ���ϰ� ����� �� �ִ� �پ��� ��� ����
  - ��Ʈ����, ����ũ, ������ MVC(���� ����)

���� ��� ���
- **�ֳ����̼� ����� ������ MVC ����**
  - @Controller
  - MVC �����ӿ�ũ�� ���� ���� �ô� ������
- ������ ��Ʈ�� ����
  - ������ ��Ʈ�� ������ ����
  - ���ſ��� ������ WAS�� ���� ��ġ�ϰ�, �ҽ��� War ������ ���� ��ġ�� WAS�� ����
  - ������ ��Ʈ�� ���� ���(Jar)�� WAS ���� ���� -> ���� ���� �ܼ�ȭ

�ֽ� ��� - ������ �� ����� ��ȭ
- Web Servlet - Spring MVC
- Web Reactive - Spring WebFlux
  - Ư¡
    - �񵿱� �� ��ŷ ó��
    - �ּ� ������� �ִ� ���� - ������ ���ؽ�Ʈ ����Ī ��� ȿ��ȭ
    - �Լ��� ��Ÿ�Ϸ� ���� - ����ó�� �ڵ� ȿ��ȭ
    - ���� ��� ��� X
  - �׷���
    - Web Flux�� ����� ���̵� �ſ� ����
    - ������ RDB ���� ����
    - �Ϲ� MVC�� ������ �𵨵� ����� ������.
    - �ǹ����� ���� ���� ��������� ����(��ü 1% ����)

�ڹ� �� ���ø� ����
- HTML�� ���ϰ� �����ϴ� �� ���
  - JSP
    - �ӵ� ����, ��� ����
  - ������Ŀ(Freemarker), Velocity(���ν�Ƽ)
    - �ӵ� ���� �ذ�, �پ��� ���
  - Ÿ�Ӹ���(Thymeleaf)
    - ���߷� ���ø�: HTML�� ����� �����ϸ鼭 �� ���ø� ���� ����
    - ������ MVC�� ������ ��� ����
    - **�ּ��� ����**, �� ������ ������Ŀ, ���ν�Ƽ�� �� ����

---
---

## ����

---
---

### ������Ʈ ����

- Gradle 
- Java
- 2.4.3
- Group : hello
- Artifact : servlet
- Packaging : War
  - ���� Jar�ε�, War�� �ؾ� jsp�� ����� �� ����.
  - War�� ���ϼ����� ������ ��ġ�ϰ� �� ���� ������ War�� �����ؼ� ������ Ȥ�� �ȿ� ������ �����ϴ°͵� ��.
- Java : 11
- Dependencies
  - Spring Web


---

### Hello ����

```java
@ServletComponentScan
@SpringBootApplication
public class ServletApplication {

	public static void main(String[] args) {
		SpringApplication.run(ServletApplication.class, args);
	}

}
```
- ��������Ʈ�� ������ ���� ����ؼ� ����� �� �ֵ��� `@ServletComponentScan`�� �����Ѵ�.

```java
package hello.servlet.basic;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(name = "heeloServlet",urlPatterns = "/hello")
public class HelloServlet extends HttpServlet {

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

        System.out.println("HelloServlet.service");
        System.out.println("request = " + request);
        System.out.println("response = " + response);

        String username = request.getParameter("username");
        System.out.println("username = " + username);

        //header�� ���°�
        response.setContentType("text/plain");
        response.setCharacterEncoding("utf-8");
        //data
        response.getWriter().write("hello "+username);
    }
}
```
- `@WebServlet` ���� �ֳ����̼�
  - name : ���� �̸�
  - urlPatterns : URL ����
  - ���� �ΰ��� �ߺ��� ������ �ȵ�.

HTTP ��û�� ���� ���ε� URL�� ȣ��Ǹ� ���� �����̳ʴ� ���� �޼��� ����.
```java
protected void service(HttpServletRequest request, HttpServletResponse response)
```

```java
//header�� ���°�
response.setContentType("text/plain");
response.setCharacterEncoding("utf-8");
//data
response.getWriter().write("hello "+username);
```
- �ĸ� ����

HTTP ��û �޽��� �α׷� Ȯ���ϱ�


resources/application.properites �� �Ʒ��� ���� �Է�
```
logging.level.org.apache.coyote.http11=debug
```

���
```
Host: localhost:8080
Connection: keep-alive
sec-ch-ua: "Chromium";v="88", "Google Chrome";v="88", ";Not A Brand";v="99"
sec-ch-ua-mobile: ?0
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.190 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Sec-Fetch-Site: none
Sec-Fetch-Mode: navigate
Sec-Fetch-User: ?1
Sec-Fetch-Dest: document
Accept-Encoding: gzip, deflate, br
Accept-Language: ko-KR,ko;q=0.9,en-US;q=0.8,en;q=0.7
Cookie: Idea-ac70df0f=3700b133-6e19-47ac-8150-fcb2b1f4a668
```
- �׷��� ������� �̷��� ��� ��û ������ �� ����� �������ϰ� �߻��� �� ������, ���� �ܰ迡���� ����

���� �����̳� ���� ��� ����
![servlet_logic](./readme_img/servlet_logic.JPG)
- ������ ��Ʈ�� ������ ������ ��Ʈ ����
- ������ ��Ʈ�� �����ϸ鼭 ������ ��Ʈ�� ���� ���� ������ ����ش�.
- �׷��鼭 ���� ������ ���ο� ���� �����̳� ����� ������ �ְ�, ���� �����̳ʸ� ���ؼ� ������ ��������.
- �׸��Ͽ� ���� �����̳ʾȿ� `helloServlet`�� ����.

![http](./readme_img/http.JPG)
- �� �������� ���Ͱ��� http �޼����� ���� ������ ������

![was_arch](./readme_img/was_arch.JPG)
- ������ WAS���� request, response ��ü�� ���� �̱������� ���ִ� `helloServlet`�� ȣ������.
- �ű⿡ ���� method�� ȣ���ϸ鼭 request, response�� �Ѱ���
- �׸��� �ʿ��� �۾�(ex> resopnse data���ٰ� Content-Type, hello world��� �޽���)�� �ϰ�, ����ǰ� �����鼭 WAS������ response ������ ������ HTTP ���� �޽����� ���Ͱ��� ����� ��ȯ�� ����.
- �׷��� �� ���������� hello world��� �� �� �ִ°Ŵ�.

> ����
>
> HTTp ���信�� Content-Length�� �� ���ø����̼� ������ �ڵ����� �������ش�.

---

### HttpServletRequest - ����

**HttpServletRequest ����**
- HTTP ��û �޽����� �����ڰ� ���� �Ľ��ؼ� ����ص� ������, �ſ� ����.
- ������ �����ڰ� HTTP ��û �޽����� ���ϰ� ����� �� �ֵ��� ������ ��ſ� HTTP ��û �޽����� �Ľ��Ѵ�.
- �׸��� �� ����� `HttpServletRequest` ��ü�� ��Ƽ� ����.

HttpServletRequest�� ����ϸ� ������ ���� HTTP ��û �޽����� ���ϰ� ��ȸ�� �� �ִ�.

**HTTP �伺 �޽���**
```
POST /save HTTP/1.1
Host: localhost:8080
Content-Type: applicatoin/x-www-form-urlencoded

username=kim&age=20
```

- START LINE(ù��° ��, �� �������� `POST /save HTTP/1.1` �̰�)
  - HTTP �޼ҵ�
  - URL
  - ���� ��Ʈ��
  - ��Ű��, ��������
- ���(�������� `Host: localhost:8080 Content-Type: applicatoin/x-www-form-urlencoded` �̰�)
  - ��� ��ȸ
- �ٵ�(�������� `username=kim&age=20` �̰�)
  - form �Ķ���� ���� ��ȸ
  - message body ������ ���� ��ȸ

**�ӽ� ����� ���**
- �ش� HTTP ��û�� ���ۺ��� ���� �� ���� �����Ǵ� �ӽ� ����� ���
  - ����: `request.setAttribute(name, value)`
  - ��ȸ: `request.getAttribute(name)`

**���� ���� ���**
- `request.getSession(create: true)`

> �߿�
>
> HttpServletRequest, HttpServletResponse�� ����� �� ���� �߿��� ���� �� ��ü���� HTTP ��û �޽���, HTTP ���� �޽����� ���ϰ� ����ϵ��� �����ִ� ��ü��� ���̴�.
>
> ���� �� ��ɿ� ���ؼ� �����ִ� ���ظ� �Ϸ��� **HTTP ������ �����ϴ� �C��, ���� �޽��� ��ü�� ����**�ؾ� �Ѵ�.

---

### HTttpServletRequest - �⺻ ����

�ڵ����� ��.

<details>
<summary>java/hello.servlet/basic/request/RequestHeaderServlet.java</summary>

```java
package hello.servlet.basic.request;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.Cookie;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.util.Enumeration;

@WebServlet(name = "requestHeaderServlet", urlPatterns = "/request-header")
public class RequestHeaderServlet extends HttpServlet {

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        printStartLine(request);
        printHeaders(request);
        printHeaderUtils(request);
        printEtc(request);

    }

    private void printStartLine(HttpServletRequest request) {
        System.out.println("--- REQUEST-LINE - start ---");
        System.out.println("request.getMethod() = " + request.getMethod()); //GET
        System.out.println("request.getProtocal() = " + request.getProtocol()); //HTTP/1.1
        System.out.println("request.getScheme() = " + request.getScheme()); //http
        // http://localhost:8080/request-header
        System.out.println("request.getRequestURL() = " + request.getRequestURL());
        // /request-test
        System.out.println("request.getRequestURI() = " + request.getRequestURI());
        //username=hi
        System.out.println("request.getQueryString() = " +
                request.getQueryString());
        System.out.println("request.isSecure() = " + request.isSecure()); //https ��� ����
        System.out.println("--- REQUEST-LINE - end ---");
        System.out.println();
    }
    //Header ��� ����
    private void printHeaders(HttpServletRequest request) {
        System.out.println("--- Headers - start ---");

//      ����
//        Enumeration<String> headerNames = request.getHeaderNames();
//        while(headerNames.hasMoreElements()){
//            String headerName = headerNames.nextElement();
//            System.out.println(headerName + ": " + headerName);
//        }

        //����
        request.getHeaderNames().asIterator()
                .forEachRemaining(headerName -> System.out.println(headerName + ": " + headerName));

        System.out.println("--- Headers - end ---");
        System.out.println();
    }

    //Header ���� ��ȸ
    private void printHeaderUtils(HttpServletRequest request) {
        System.out.println("--- Header ���� ��ȸ start ---");
        System.out.println("[Host ���� ��ȸ]");
        System.out.println("request.getServerName() = " +
                request.getServerName()); //Host ���
        System.out.println("request.getServerPort() = " +
                request.getServerPort()); //Host ���
        System.out.println();
        System.out.println("[Accept-Language ���� ��ȸ]");
        request.getLocales().asIterator()
                .forEachRemaining(locale -> System.out.println("locale = " +
                        locale));
        System.out.println("request.getLocale() = " + request.getLocale());
        System.out.println();
        System.out.println("[cookie ���� ��ȸ]");
        if (request.getCookies() != null) {
            for (Cookie cookie : request.getCookies()) {
                System.out.println(cookie.getName() + ": " + cookie.getValue());
            }
        }
        System.out.println();
        System.out.println("[Content ���� ��ȸ]");
        System.out.println("request.getContentType() = " +
                request.getContentType());
        System.out.println("request.getContentLength() = " +
                request.getContentLength());
        System.out.println("request.getCharacterEncoding() = " +
                request.getCharacterEncoding());
        System.out.println("--- Header ���� ��ȸ end ---");
        System.out.println();
    }

    //��Ÿ ����
    private void printEtc(HttpServletRequest request) {
        System.out.println("--- ��Ÿ ��ȸ start ---");
        // remote ���� : ��û�� �°ſ� ���� ����
        System.out.println("[Remote ����]");
        System.out.println("request.getRemoteHost() = " +
                request.getRemoteHost()); //
        System.out.println("request.getRemoteAddr() = " +
                request.getRemoteAddr()); //
        System.out.println("request.getRemotePort() = " +
                request.getRemotePort()); //
        System.out.println();
        // local ���� : ���� ���� ������ ���� ����
        System.out.println("[Local ����]");
        System.out.println("request.getLocalName() = " +
                request.getLocalName()); //
        System.out.println("request.getLocalAddr() = " +
                request.getLocalAddr()); //
        System.out.println("request.getLocalPort() = " +
                request.getLocalPort()); //
        System.out.println("--- ��Ÿ ��ȸ end ---");
        System.out.println();
    }
}

```
</details>

---

### HTTP ��û ������ - ����

HTTP ��û �޽����� ���� Ŭ���̾�Ʈ���� ������ �����͸� �����ϴ� �����.

**�ַ� ���� 3���� ����� ���**
- **GET - ���� �Ķ����**
  - /url<strong>?username=hello?age=20</strong>
  - �޽��� �ٵ� ����, URL�� ���� �Ķ���Ϳ� �����͸� �����ؼ� ����
  - ex> �˻�, ����, ����¡��� ���� ����ϴ� ���
- **POST - HTML Form**
  - ![html_form](./readme_img/html_form.JPG)
  - content-type : applicatoin/x-www-form-urlencoded
  - �޽��� �ٵ� ���� �Ķ���� �������� ���� username=hello&age=20
  - ex> ȸ�� ����, ��ǰ �ֹ�, HTML Form ���
- **HTTP message body**�� �����͸� ���� ��Ƽ� ��û
  - HTTP API���� �ַ� ���, JSON, XML, TEXT
  - ������ ������ �ַ� JSON ���
  - POST, PUT, PATCH

---

### HTTP ��û ������ - GET ���� �Ķ����

���� �����͸� client���� server�� �����غ���.

���� ������
- username=hello
- age=20

�޽��� �ٵ� ����, URL�� ���� �Ķ���͸� ����ؼ� �����͸� �����غ���.<br>
ex> �˻�, ����, ����¡��� ���� ����ϴ� ���

���� �Ķ���ʹ� URL�� ������ ���� `?`�� �������� ���� �� �ִ�. �߰� �Ķ���ʹ� `&`�� �����ϸ� �ȴ�.
- `http://localhost:8080/request-param?username=hello&age=20`

���������� `HttpServletRequest`�� �����ϴ� ���� �޼��带 ���� ���� �Ķ���͸� ���ϰ� ��ȸ�� �� �ִ�.

```
[��ü �Ķ���� ��ȸ] - start
username=hello
age=20
[��ü �Ķ���� ��ȸ] - end

[���� �Ķ���� ��ȸ]
username = hello
age = 20

[�̸��� ���� ���� �Ķ���� ��ȸ]
name = hello
name = hello2
```

**���� �Ķ���Ϳ��� ���� �Ķ���� ��ȸ**
- `username=hello&username=kim`�� ���� �Ķ���� �̸��� �ϳ��ε�, ���� �ߺ��Ǹ� ��� �ɱ�?
- `request.getParameter()`�� �ϳ��� �Ķ���� �̸��� ���ؼ� �� �ϳ��� ���� ���� �� ����ؾ��Ѵ�. ����ó�� �ߺ��϶��� `request.getParameterValues()`�� ����ؾ� �Ѵ�.
- ����� �̷��� �ߺ��� �� `request.getParameter()`�� ����ϸ� `request.getParameterValues`�� ù ��° ���� ��ȯ.

---

### HTTP ��û ������ - POST HTML Form

�̹����� HTML�� Form�� ����ؼ� client ���� server�� �����͸� �����غ���.<br>
�ַ� ȸ�� ����, ��ǰ �ֹ� ��� ����ϴ� ����̴�.

**Ư¡**
- content-type: `application/x-www-form-urlencoded`
- �޽��� �ٵ� ���� �Ķ���� �������� �����͸� �����Ѵ�. `username=hello&age=20`

`src/main/webapp/basic/hello-form.html`����

```html
<!DOCTYPE html>
<html>
<head>
 <meta charset="UTF-8">
 <title>Title</title>
</head>
<body>
<form action="/request-param" method="post">
 username: <input type="text" name="username" />
 age: <input type="text" name="age" />
 <button type="submit">����</button>
</form>
</body>
</html>
```

POST�� HTML Form�� �����ϸ� �� �������� ���� �������� HTTP �޽����� �����. (�� ������ ������ ��� Ȯ��)
- **��û URL** : `http://localhost:8080/request-param`
- **content-type**: `applicatoin/x-www-form-urlencoded`
- **message body** : `username=hello&age=20`

`application/x-www-form-urlencoded` ������ �ռ� GET���� ���캻 �����Ķ���� ���İ� ����. ���� **���� �Ķ���� ��ȸ �޼��带 �״�� ���**�ϸ� �ȴ�. <br>
client(�� ������) ���忡���� �� ��Ŀ� ���̰� ������, server ���忡���� ���� ������ �����ϹǷ�, `request.getParameter()`�� ���ϰ� ���о��� ��ȸ�� �� �ִ�.

�����ϸ� `request.getParameter()`�� GET URL ���� �Ķ���� ���ĵ� �����ϰ�, POST HTML Form ���ĵ� �� �� �����Ѵ�.

> **����**
>
> contnet-type�� HTTP �޽��� �ٵ��� ������ ������ �����Ѵ�. <br>
> **GET URL ���� �Ķ���� ����**���� client���� server�� �����͸� ���� �� ���� HTTP �޽��� �ٵ� ������� �ʱ� ������ content-type�� ����. <br>
> **POST HTML Form** �������� �����͸� �����ϸ� HTTP �޽��� �ٵ� �ش� �����͸� �����ؼ� ������ ������ �ٵ� ���Ե� �����Ͱ� � �������� content-type�� �� �����ؾ� �Ѵ�. �̷��� ������ �����͸� �����ϴ� ������ `applicaton/x-www-form-urlencoded`'�� �Ѵ�.

Postman�� ����� �׽�Ʈ
- �̷� ������ �׽�Ʈ���� HTML form�� ������ ������. �̶� Postman�� ����ϸ� �ȴ�.

**Postman** �׽�Ʈ ���ǻ���
- POST ���۽�
  - Body -> `x-www-form-urlencoded` ����
  - Headers���� content-type: `application/x-www-form-urlencoded`�� ������ �κ� �� Ȯ��

---

### HTTP ��û ������ - API �޽��� �ٵ� - �ܼ� �ؽ�Ʈ

- **HTTP message body**�� �����͸� ���� ��Ƽ� ��û
  - HTTP API���� �ַ� ���, JSON, XML, TEXT
  - ������ ������ �ַ� JSON ���
  - POST, PUT, PATCH

- ���� ���� �ܼ��� �ؽ�Ʈ �޽����� HTTP �޽��� �ٵ� ��Ƽ� �����ϰ� �о��.
- HTTP �޽��� �ٵ��� �����͸� InputStream�� ����ؼ� ���� ���� �� �ִ�.

> ����<br>
> inputStream�� byte �ڵ带 ��ȯ�Ѵ�. byte �ڵ带 �츮�� ���� �� �ִ� ����(String)�� ������ ����ǥ(Charset)�� �������־�� �Ѵ�. ���⼭�� UTF_8 Charset�� �������־���.


### HTTP ��û ������ - API �޽��� �ٵ� - JSON

�̹����� HTTP API���� �ַ� ����ϴ� JSON �������� �����͸� �����غ���.

**JSON ���� ����**
- POST http://localhost:8080/request-body-json
- content-type: **application/json**
- message body: `{"username": "hello", "age": 20}
- ���: `messageBody = {"username": "hello", "age": 20}

**JSON ���� �Ľ� �߰�**<br>
JSON �������� �Ľ��� �� �ְ� ��ü�� �ϳ� ����.<BR>
`heelo.servlet.basic.HelloData`
- lombok ���

> ����<br>
> JSON ����� �Ľ��ؼ� ����� �� �ִ� �ڹ� ��ü�� ��ȯ�Ϸ��� Jackson, Gson ���� JSON ��ȯ ���̺귯���� �߰��ؼ� ����ؾ� �Ѵ�. ������ ��Ʈ�� Spring MVC�� �����ϸ� �⺻���� Jackson ���̺귯��(`ObjectMapper`)�� �Բ� �����Ѵ�.

> ����<br>
> HTML form �����͵� �޽��� �ٵ� ���� ���۵ǹǷ� ���� ���� �� �ִ�. ������ ���� �Ķ���� ��ȸ ��� (`request.getParameter(...)`)�� �̹� �����ϱ� ������ �Ķ���� ��ȸ ����� ����ϸ� �ȴ�.

---

### HttpServletResponse - �⺻ ����

HttpServletResponse ����

**HTTP ���� �޽��� �ۼ�**
- HTTP �����ڵ� ����(ex>200,400,500,403...)
- ��� ����
- �ٵ� ����

**���� ��� ����**
- Content-Type, ��Ű, Redirect(�ڵ�� Ȯ�� main/java/hello.servlet/basic/response)

---

### HTTP ���� ������ - �ܼ� �ؽ�Ʈ, HTML

HTTP ���� �޽����� �ַ� ���� ������ ��Ƽ� �����Ѵ�.

- �ܼ� �ؽ�Ʈ ����
  - `writer.println("ok");`
- HTML ����
- HTTP API - MessageBody JSON ����

<details>
<summary>�ڵ�</summary>

```java

@WebServlet(name = "responseHtmlServlet", urlPatterns = "/response-html")
public class ResponseHtmlServlet extends HttpServlet {

    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        //Content-Type: text/html;charset=utf-8
        response.setContentType("text/html");
        response.setCharacterEncoding("utf-8");

        PrintWriter writer = response.getWriter();
        writer.println("<html>");
        writer.println("<body>");
        writer.println("  <div>�ȳ�?</div>");
        writer.println("</body>");
        writer.println("</html>");

    }
```

</details>

- HTTP �������� HTML�� ��ȯ�� �� content-type�� `text/html`�� �����ؾ� �Ѵ�.

---

### HTTP ���� ������ - API JSON

<details>
<summary>�ڵ�</summary>

```java
@WebServlet(name = "responseJsonServlet", urlPatterns = "/response-json")
public class ResponseJsonServlet extends HttpServlet {
    
  private ObjectMapper objectMapper = new ObjectMapper();

  @Override
  protected void service(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
      //Content-Type: application/json
      response.setContentType("application/json");
      response.setCharacterEncoding("utf-8");

      HelloData helloData = new HelloData();
      helloData.setUsername("kim");
      helloData.setAge(20);
      
      //�� ���ڸ� ���� ��ȯ�ؾ��� {"username":"kim", "age":20} -> objectMapper ���
      String result = objectMapper.writeValueAsString(helloData);
      response.getWriter().write(result);
  }
}
```
- Jackson ���̺귯���� �����ϴ� objectMapper.writeValueAsString() �� ����ϸ� ��ü�� JSON ���ڷ� ������ �� �ִ�

</details>

---
---

## ����, JSP, MVC ����

---
---

### ȸ�� ���� �� ���ø����̼� �䱸����

**ȸ�� ����**
- �̸� : `username`
- ���� : `age`

**��� �䱸����**
- ȸ�� ����
- ȸ�� ��� ��ȸ

---

### �������� ȸ�� ���� �� ���ø����̼� �����

�������� ȸ�� ��� HTML ���� �����غ���.
(html �ۼ��� ���� ����)(�ڹ��ڵ忡�ٰ� html�� ����� �ִ°�)

**���ø� ��������**
- ���ݱ��� ������ �ڹ� �ڵ常���� HTML�� �������. ���� ���п� �������� ���ϴ� HTML�� ������ ���� �� �ִ�.
- ������ HTML ������� ȭ���� ��� �޶����� ȸ���� ���� ��������, ȸ�� ��� ���� ������ HTML�� ����� ���� �Ұ��� �� ���̴�.
- �׷���, �ڵ忡�� ������ �ſ� �����ϰ� ��ȿ����.
- �ڹ� �ڵ�� HTML�� ����� ���� �� ���� ���� HTML ������ �������� �����ؾ� �ϴ� �κи� �ڹ� �ڵ带 ���� �� �ִٸ� ���� ���̴�.
- �̰��� �ٷ� ���ø� ������ ���� �����̴�. ���ø� ������ ����ϸ� HTML �������� �ʿ��� ���� �ڵ带 �����ؼ� �������� ���� ����.
- ���ø� �������� JSP, Thymeleaf, Freemarker, Velocity���� �ִ�.

> **����**
>
> JSP�� ���ɰ� ��ɸ鿡�� �ٸ� ���ø� �������� ���￡�� �и��鼭, ���� ����Ǿ� ���� �߼��̴�.<BR>
> ���ø� �������� ���� ������� �ִµ�, ���ǿ����� JSP�� �պκп��� ��� �ٷ��, �������� �� ���յǴ� Thymeleaf�� ����Ѵ�.

---

### JSP�� ȸ�� ���� �� ���ø����̼� �����

- `<% page contentType="text/html;charset=UTF-8" language="java" %>`
  - ù ���� JSP������� ���̴�. JSP�� �̷��� �����ؾ���.

ȸ�� ��� �� JSP�� ���� ù ���� �����ϰ�� ������ HTML�� �Ȱ���. JSP�� ���� ���ο��� �������� ��ȯ�Ǵµ�, �츮�� ������� MemberFormServlet�� ���� ����� ����̴�.

JSP�� �ڹ� �ڵ带 �״�� �� ����� �� �ִ�.
- `<%@ page import"hello.servlet.domain.member.MemberRepository" %>`
  - �ڹ��� import ���� ����.
- `<% ~~~ %>`
  - �� �κп��� �ڹ� �ڵ带 �Է��� �� �ִ�.
- `<%= ~~ %>`
  - �� �κп��� �ڹ� �ڵ带 ����� �� �ִ�.

ȸ�� ���� JSP�� ����, ȸ�� ���� ���� �ڵ�� ����. �ٸ� ���� �ִٸ� HTML�� �߽����� �ϰ�, �ڹ� �ڵ带 �κкκ� �Է����־���. `<% ~ %>`�� ����ؼ� HTML �߰��� �ڹ� �ڵ带 ����ϰ� �ִ�.

ȸ�� �������丮�� ���� ��ȸ�ϰ�, ��� List�� ����ؼ� �߰��� `<tr><td>` HTML �±׸� �ݺ��ؼ� ����ϰ� �ִ�.

������ JSP�� �Ѱ�

- �������� ������ ���� ��(View)ȭ���� ���� HTML�� ����� �۾��� �ڹ� �ڵ忡 ������ �������ϰ� �����ߴ�.
- JSP�� ����� ���п� �並 �����ϴ� HTML �۾��� ����ϰ� ��������, �߰��߰� �������� ������ �ʿ��� �κп��� �ڹ� �ڵ带 �����ߴ�. �׷��� �̷��� �ص� �ذ���� �ʴ� ��� ����� ���´�.
<BR>

- ȸ�� ���� JSP�� ����.
- �ڵ��� ���� ������ ȸ���� �����ϱ� ���� ����Ͻ� �����̰�, ������ ���� ���ݸ� ����� HTML�� �����ֱ� ���� �� �����̴�. ȸ�� ����� ��쿡�� ����������.
- �ڵ带 �� ����, JAVA �ڵ�, �����͸� ��ȸ�ϴ� �������丮 ��� �پ��� �ڵ尡 ��� JSPDP ����Ǿ� �ִ�. JSP�� �ʹ� ���� ������ �Ѵ�. �̷��� ���� ������Ʈ�� ���� �Ӹ��� ���Ŀ��µ�, ���� ��õ���� �Ѿ�� JSP�� ���÷����� ���� ������ ���� ���̴�.(�������� ���� ��)

**MVC ������ ����**

����Ͻ� ������ ���� ó�� �ٸ������� ó���ϰ�, JSP�� ������ �°� HTML�� ȭ��(View)�� �׸��� �Ͽ� ����.

���� �����ڵ鵵 ��� ����� ����� �־���, �׷��� MVC������ �����ߴ�.

---

### MVC ���� - ����

**�ʹ� ���� ����**<BR>
- �ϳ��� �����̳� JSP������ ����Ͻ� ������ �� ���������� ��� ó���ϰ� �Ǹ�, �ʹ� ���� ������ �ϰԵǰ�, ��������� ���������� ���������. 
- ����Ͻ� ������ ȣ���ϴ� �κп� ������ �߻��ص� �ش� �ڵ带 �մ�� �ϰ�, UI�� ������ ���� �־ ����Ͻ� ������ �Բ� �ִ� �ش� ������ �����ؾ� �Ѵ�. 
  - HTML �ڵ� �ϳ� �����ؾ� �ϴµ�, �������� �ڹ� �ڵ尡 �Ա� �ִٰ� ����ϸ� �����ϴ�. 
  - �Ǵ� ����Ͻ� ������ �ϳ� �����ؾ� �ϴµ� ���� ��õ���� HTML �ڵ尡 �Բ� �ִٸ� �����ϴ�.

**������ ������ ����Ŭ**<BR>
- ��� �̰� �߿��ѵ�, ��¥ ������ �� ���̿� ������ ������ ����Ŭ�� �ٸ��ٴ� ���̴�.
- ���� �� UI�� �Ϻ� �����ϴ� �ϰ� ����Ͻ� ������ �����ϴ� ���� ���� �ٸ��� �߻��� ���ɼ��� �ſ� ���� ��κ� ���� ������ ���� �ʴ´�.
- �̷��� ������ ������ ����Ŭ�� �ٸ� �κ��� �ϳ��� �ڵ�� �����ϴ� ���� ���������ϱ� ���� �ʴ�. (���� UI�� ���� ���ϸ� �Բ� ����� ���ɼ��� �ִ�.)

**��� Ưȭ**
- Ư�� JSP ���� �� ���ø��� ȭ���� ������ �ϴµ� ����ȭ �Ǿ� �ֱ� ������ �� �κ��� ������ ����ϴ� ���� ���� ȿ�����̴�.

**Model View Control**
- MVC ������ ���ݱ��� �н��� �� ó�� �ϳ��� �����̳�, JSP�� ó���ϴ� ���� ��Ʈ�ѷ�(Controller)�� ��(View)��� �������� ���� ������ ���� ���� ���Ѵ�. �� ���ø����̼��� ���� �� MVC ������ ����Ѵ�.

**��Ʈ�ѷ�** : HTTP ��û�� �޾Ƽ� �Ķ���͸� �����ϰ�, ����Ͻ� ������ �����Ѵ�. �׸��� �信 ������ ��� �����͸� ��ȸ�ؼ� �𵨿� ��´�.

**��**: �信 ����� �����͸� ��Ƶд�. �䰡 �ʿ��� �����͸� ��� �𵨿� ��Ƽ� �������ִ� ���п� ��� ����Ͻ� �����̳� ������ ������ ���� �ǰ�, ȭ���� ������ �ϴ� �Ͽ� ������ �� �ִ�.

**��** : �𵨿� ����ִ� �����͸� ����ؼ� ȭ���� �׸��� �Ͽ� �����Ѵ�. ���⼭�� HTML�� �����ϴ� �κ��� ���Ѵ�.

> **����**<BR>
> ��Ʈ�ѷ��� ����Ͻ� ������ �� ���� ������, �̷��� �Ǹ� ��Ʈ�ѷ��� �ʹ� ���� ������ ����Ѵ�.<BR>
> �׷��� �Ϲ������� ����Ͻ� ������ ����(Service)��� ������ ������ ���� ó���Ѵ�.(�� ������ ���� ���°��(�ܼ��� ����...)�� repository�� �ٷ� ����ϱ⵵ ��)<br>
> �׸��� ��Ʈ�ѷ��� ����Ͻ� ������ �ִ� ���񽺸� ȣ���ϴ� ����Ѵ�.<br>
> ����� ����Ͻ� ������ �����ϸ� ����Ͻ� ������ ȣ���ϴ� ��Ʈ�ѷ��� �ڵ嵵 ����� �� �ִ�. �տ����� �����ꤩ ���� ���� ����Ͻ� ������ ȣ���Ѵٴ� ǥ�� ���ٴ�, ����Ͻ� �����̶� �����ߴ�.

![mvc1](./readme_img/mvc1.JPG)
- ���� ��û�� ��.
- Controller���� ����Ͻ� ���� ����(servlet)
- Model���ٰ� �����͸� ��´�
- �׸��� �� ������ ����(�� �������� ������� �ѱ��.)(jsp)
- jsp�� �̶����� ���� �Ǹ鼭 Model�� �ִ� �����͸� �����ؼ� view�� �׷��� ��������.

![mvc2](./readme_img/mvc2.JPG)
- ���� �� �׸��� ����
- client�� controller ȣ���Ѵ�.
- controller�� �Ķ���� ������ �� ���� ����� ��û�Ѱ���, http ��û�� ����� �´��� ������ Ȯ��(�߸��Ǹ� 400 ����...), ������ �� ������ service�� repository�� ȣ���ؼ� ����Ͻ� �����̳� ������ ������ ��.
- �׸��� controller�� �̿� ���� ����� ����.
- �׸��� Model���ٰ� �����͸� ������
- �� �������� ������� �ѱ��
- �� ������ Model���� ���� ������ ó����.

---

### MVC ���� - ����

������ controller�� ����ϰ�, JSP�� view�� ����ؼ� MVC ������ �����غ���.<br>
Model�� HttpServletRequest ��ü�� ����Ѵ�. request�� ���ο� ������ ����Ҹ� ������ �ִµ�, `request.setAttribute()`,`request.getAttribute()`�� ����ϸ� �����͸� �����ϰ�, ��ȸ�� �� �ִ�.

`dispatcher.forward()`: �ٸ� �����̳� JSP�� �̵��� �� �ִ� ����̴�. ���� ���ο��� �ٽ� ȣ���� �߻��Ѵ�.(client���� server�� ȣ���� �Ѱ���, server�ȿ��� �ڱ�� ���� ������ ȣ��Ǿ��ٰ� jsp�� ȣ���ϰ� jsp���� ������ ���� ������ ��������)

`/WEB-INF`<br>
�� ��ξȿ� JSP�� ������ �ܺο��� ���� JSP�� ȣ���� �� ����. �츮�� ����ϴ� ���� �׻� ��Ʈ�ѷ��� ���ؼ� JSP�� ȣ���ϴ� ���̴�.

**redirect vs forward**<br>
redirect�� ���� client(�� ������)�� ������ �����ٰ�, client�� redirect ��η� �ٽ� ��û�Ѵ�. ���� client�� ������ �� �ְ�, URL ��ε� ������ ����ȴ�.(ȣ���� 2��)<BR>
�ݸ鿡 forward�� ���� ���ο��� �Ͼ�� ȣ���̱� ������ client�� ���� �������� ���Ѵ�.

```html
<!-- ����� ���, [���� URL�� ���� ���� ��� + /save] -->
<form action="save" method="post">
    username: <input type="text" name="username" />
    age: <input type="text" name="age" />
    <button type="submit">����</button>
</form>
```
- ���⼭ form�� action�� ���� ���� ���(/�� ����)�� �ƴ϶� �����(/�� ���� x)�ϴ� ���� Ȯ���� �� �ִ�. �̷��� ����θ� ����ϸ� �� ���۽� ���� URL�� ���� ���� ��� + save�� ȣ��ȴ�.<br>
- ���� ���� ��� : `/servlet-mvc/members/`
- ��� : `servlet-mvc/members/save`


**ȸ�� ���� - ��Ʈ�ѷ�**<br>
HttpServletRequest�� Model�� ����Ѵ�.<br>
request�� �����ϴ� `setAttribute()`�� ����ϸ� request ��ü�� �����͸� �����ؼ� �信 ������ �� �ִ�.<br>
��� `request.getAttribute()`�� ����ؼ� �����͸� ������ �ȴ�.

**ȸ�� ���� - ��**<br>
`<%= request.getAttribute("member")%>`�� �𵨿� ������ member ��ü�� ���� �� ������, �ʹ� ����������.<br>
JSP�� `${}` ������ �����ϴµ�, �� ������ ����ϸ� request�� attribute�� ��� �����͸� ���ϰ� ��ȸ�� �� �ִ�.

**ȸ�� ��� ��ȸ - ��Ʈ�ѷ�**<br>
request ��ü�� ����ؼ� `List<Member> members`�� �𵨿� �����ߴ�.

**ȸ�� ��� ��ȸ - ��**<br>
�𵨿� ��Ƶ� members�� JSP�� �����ϴ� taglib����� ����ؼ� �ݺ��ϸ鼭 ����ߴ�.<br>
`members` ����Ʈ���� `member`�� ������� ������ `item` ������ ���, ����ϴ� ������ �ݺ��Ѵ�.

`<c:forEach>` �� ����� ����Ϸ��� ������ ���� �����ؾ� �Ѵ�.<br>
`<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core"%>`

MVC ���п� ��Ʈ�ѷ� ������ �� ������ Ȯ���ϰ� �и��� ���� Ȯ���� �� �ִ�. ���� ȭ�鿡 ������ �߻��ϸ� �� ������ �����ϸ� �ȴ�.
