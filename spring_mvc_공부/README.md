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
    - [MVC ���� - �Ѱ�](#mvc-����---�Ѱ�)
  - [MVC �����ӿ�ũ �����](#mvc-�����ӿ�ũ-�����)
    - [����Ʈ ��Ʈ�ѷ� ���� �Ұ�](#����Ʈ-��Ʈ�ѷ�-����-�Ұ�)
    - [����Ʈ ��Ʈ�ѷ� ���� - v1](#����Ʈ-��Ʈ�ѷ�-����---v1)
    - [View �и� - v2](#view-�и�---v2)
    - [Model �߰� - v3](#model-�߰�---v3)
    - [�ܼ��ϰ� �ǿ����� ��Ʈ�ѷ� - V4](#�ܼ��ϰ�-�ǿ�����-��Ʈ�ѷ�---v4)
    - [������ ��Ʈ�ѷ�1 - v5](#������-��Ʈ�ѷ�1---v5)
    - [������ ��Ʈ�ѷ�2 - V5](#������-��Ʈ�ѷ�2---v5)
    - [����](#����)
  - [������ MVC - ���� ����](#������-mvc---����-����)
    - [������ MVC ��ü ����](#������-mvc-��ü-����)
    - [�ڵ鷯 ���ΰ� �ڵ鷯 �����](#�ڵ鷯-���ΰ�-�ڵ鷯-�����)
      - [Controller �������̽�](#controller-�������̽�)
    - [������ MVC - �����ϱ�](#������-mvc---�����ϱ�)
    - [������ MVC - ��Ʈ�ѷ� ����](#������-mvc---��Ʈ�ѷ�-����)
  - [������ MVC - �ǿ����� ���](#������-mvc---�ǿ�����-���)
  - [������ MVC - �⺻ ���](#������-mvc---�⺻-���)
    - [������Ʈ ����](#������Ʈ-����-1)
    - [�α� ������ �˾ƺ���](#�α�-������-�˾ƺ���)
    - [��û ����](#��û-����)
    - [��û ���� - API ����](#��û-����---api-����)
    - [HTTP ��û - �⺻, ��� ��ȸ](#http-��û---�⺻-���-��ȸ)
    - [Http ��û �Ķ���� - ���� �Ķ����, HTML Form](#http-��û-�Ķ����---����-�Ķ����-html-form)
      - [HTTP ��û ������ ��ȸ - ����](#http-��û-������-��ȸ---����)
      - [��û �Ķ���� - ���� �Ķ����, HTML Form](#��û-�Ķ����---����-�Ķ����-html-form)
    - [HTTP ��û �Ķ���� - @RequestParam](#http-��û-�Ķ����---requestparam)
    - [HTTp ��û �Ķ���� - @ModelAttribute](#http-��û-�Ķ����---modelattribute)
    - [HTTP ��û �޽��� - �ܼ� �ؽ�Ʈ](#http-��û-�޽���---�ܼ�-�ؽ�Ʈ)
    - [HTTP ��û �޽��� - JSON](#http-��û-�޽���---json)
    - [���� - ���� ���ҽ�, �� ���ø�](#����---����-���ҽ�-��-���ø�)
      - [���� ���ҽ�](#����-���ҽ�)
      - [�� ���ø�](#��-���ø�)
    - [HTTP ���� - HTTP API, �޽��� �ٵ� ���� �Է�](#http-����---http-api-�޽���-�ٵ�-����-�Է�)


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

---

### MVC ���� - �Ѱ�

MVC ������ ������ ���п� controller�� ���Ұ� view�� ������ �ϴ� ������ ��Ȯ�ϰ� ������ �� �ִ�.<br>
Ư�� view�� ȭ���� �׸��� ���ҿ� ����� ���п�, �ڵ尡 ����ϰ� �������̴�. �ܼ��ϰ� �𵨿��� �ʿ��� �����͸� ������, ȭ���� ����� �ȴ�.<br>
�׷��� controller�� �� ���� �ߺ��� ����, �ʿ����� �ʴ� �ڵ�鵵 ���� ���δ�.

**MVC controller�� ����**

- **������ �ߺ�**
  - View�� �̵��ϴ� �ڵ尡 �׻� �ߺ� ȣ��Ǿ�� �Ѵ�. ���� �� �κ��� �޼���� ����ȭ�ص� ������, �ش� �޼��嵵 �׻� ���� ȣ���ؾ� �Ѵ�.
  - 
  ```java
  RequestDispatch dispatcher = request.getRequestDispatcher(viewPath);
  dispatcher.forward(request, response);
  ```

- **ViewPath�� �ߺ�**
  - 
  ```java
  String viewPath = "/WEB-INF/views/new-form.jsp";
  ```
  - prefix: `/WEB-INF/views/`
  - suffix: `.jsp`
  - �׸��� ���� jsp�� �ƴ� thymeleaf ���� �ٸ� ��� �����Ѵٸ� ��ü �ڵ带 �� �����ؾ� �Ѵ�.

- **������� �ʴ� �ڵ�**
  - ���� �ڵ带 ����� ���� �ְ�, ������� ���� ���� �ִ�. Ư�� response�� ���� �ڵ忡�� ������ �ʴ´�.
  - 
  ```java
  HttpServletRequest request, HttpServletResponse response
  ```
  - �׸��� �̷� `HttpServletRequest`,`HttpServletResponse`�� ����ϴ� �ڵ�� �׽�Ʈ ���̽��� �ۼ��ϱ⵵ ��ƴ�.

- **���� ó���� ��ƴ�**
  - ����� �������� ���� controller���� �������� ó���ؾ� �ϴ� �κ��� ���� �� ���� ������ ���̴�. �ܼ��� ���� ����� �޼���� ������ �� �� ������, ��������� �ش� �޼��带 �׻� ȣ���ؾ� �ϰ�, �Ǽ��� ȣ������ ������ ������ �� ���̴�. �׸��� ȣ���ϴ� �� ��ü�� �ߺ��̴�.

- **�����ϸ� ���� ó���� ��ƴٴ� ������ �ִ�**
  - �� ������ �ذ��Ϸ��� controller ȣ�� ���� ���� ���� ����� ó���ؾ� �Ѵ�. ���� **������ ����**�� �ϴ� ����� �ʿ��ϴ�. **����Ʈ ��Ʈ�ѷ�(Front Controller) ����**�� �����ϸ� �̷� ������ ����ϰ� �ذ��� �� �ִ�.(�Ա��� �ϳ���)<br>
  - ������ MVC�� �ٽɵ� �ٷ� �� front controller�� �ִ�.

---
---

## MVC �����ӿ�ũ �����

---
---

### ����Ʈ ��Ʈ�ѷ� ���� �Ұ�

����Ʈ ��Ʈ�ѷ� ������(���� ������ �ߺ�)
![before_front_controller](./readme_img/before_front_controller.JPG)

����Ʈ ��Ʈ�ѷ� ���� ��(���� �ϳ� �����ϰ� �װ����ٰ� ���� ������ ����, controller A,B,C ���� �ʿ��� ������ ���� ó���ϼ���)
![after_front_controller](./readme_img/after_front_controller.JPG)


**FrontController ���� Ư¡**
- Front Controller Servlet �ϳ��� client�� ��û�� ����
- Front Controller�� ��û�� �´� controller�� ã�Ƽ� ȣ��.
- �Ա��� �ϳ���!
- ���� ó�� ����
- Front Controller�� ������ ������ Controller�� Servlet�� ������� �ʾƵ� ��.

**������ �� MVC�� front controller**<br>
������ �� MVC�� �ٽɵ� �ٷ� **FrontController**<br>
������ �� MVC�� **DispatcherServlet**�� FrontController �������� �����Ǿ� ����

---

### ����Ʈ ��Ʈ�ѷ� ���� - v1

����Ʈ ��Ʈ�ѷ��� �ܰ������� ����<br>
�̹� ��ǥ�� ���� �ڵ带 �ִ��� �����ϸ鼭, ����Ʈ ��Ʈ�ѷ��� ����.<br>
���� ������ ���߾�ΰ� ���������� �����͸���.

**V1 ����**
![v1](./readme_img/v1.JPG)

- client�� http��û�� ��
- front controller��� ������ ��û�� ����
- http ��û�� URL ���� ������ ������ ��Ʈ�ѷ��� ���������� �־��.
- � ��Ʈ�ѷ��� ȣ��Ǿ���ϴ��� ã�� �� �ش� ��Ʈ�ѷ� ȣ��
- ��Ʈ�ѷ��� �ڱ� ���� �����ϰ� ��Ʈ�ѷ����� JSP forward
- http ����

ControllerV1
- �������̽��� �����
- ������ ����� ����� ��Ʈ�ѷ� �������̽���. �� ��Ʈ�ѷ����� �� �������̽��� �����ϸ� �ȴ�. ����Ʈ ��Ʈ�ѷ��� �� �������̽��� ȣ���ؼ� ������ ������� ������ �ϰ����� ������ �� �ִ�.

���� �� �������̽��� ������ ��Ʈ�ѷ��� ������. ���� �ܰ迡���� ���� ������ �ִ��� �����ϴ°� �ٽ�.
- MemberFormControllerV1

**����Ʈ ��Ʈ�ѷ� �м�**

**urlPatterns**
- `urlPatterns = "/front-controller/v1/*"`: `front-controller/v1` �� ������ ���� ��� ��û�� �� �������� �޾Ƶ��δ�
- ex> `/front-controller/v1`,`/front-controller/v1/a`,`/front-controller/v1/a/b`

**controllerMap**
- key: ���� URL
- value: ȣ��� ��Ʈ�ѷ�

**service()**

���� `requestURI`�� ��ȸ�ؼ� ���� ȣ���� ��Ʈ�ѷ��� `controllerMap`���� ã�´�. ���� ���ٸ� 404(SC_NOT_FOUND) ���� �ڵ带 ��ȯ�Ѵ�.<BR>
��Ʈ�ѷ��� ã�� `controller.procesS(request,response);`�� ȣ���ؼ� �ش� ��Ʈ�ѷ��� �����Ѵ�.

**JSP**<br>
JSP�� ���� MVC���� ����ߴ� ���� �״�� ����Ѵ�.

---

### View �и� - v2

��� ��Ʈ�ѷ����� ��� �̵��ϴ� �κп� �ߺ��� �ְ�, ������� �ʴ�.
```java
String viewPath = "/WEB-INF/views/new-form.jsp";
RequestDispatcher dispatcher = request.getRequestDispatcher(viewPath);
dispatcher.forward(request,response);
```

�� �κ��� ����ϰ� �и��ϱ� ���� ������ �並 ó���ϴ� ��ü�� ������.

**V2 ����**
![v2](./readme_img/v2.JPG)
- client�� http ��û�� ��.
- front controller�� ���� �������� controller ��ȸ
- �� ��, controller ȣ��
- controller���� MyView ��ȯ
- frontcontroller�� ��� myview�� render()�� ȣ���ؼ�
- MyView�� JSP�� forward�ϵ��� ��.

�� ���� ���ؼ� controller�� ���̻� JSP forward �̷��ſ� ���ؼ� ������� �ʾƵ� ��. �ܼ��ϰ� myview�� �����ؼ� ȣ���ϸ� �ȴ�.

**MyView**<br>
�� ��ü�� ���� �ٸ� ���������� �Բ� ����ϹǷ� ��Ű�� ��ġ�� `frontcontroller`�� �ξ���.

����Ʈ ��Ʈ�ѷ��� �������� `MyView` ��ü�� `render()`�� ȣ���ϴ� �κ��� ��� �ϰ��ǰ� ó���� �� �ִ�. ������ ��Ʈ�ѷ��� `MyView` ��ü�� ������ �ؼ� ��ȯ�ϸ� �ȴ�.

---

### Model �߰� - v3

**���� ���Ӽ� ����**<br>
controller ���忡�� HttpServletRequest, HttpServletResponse�� �� �ʿ��ұ�?<br>
��û �Ķ���� ������ �ڹ��� Map���� ��� �ѱ⵵�� �ϸ� ���� ���������� **controller�� servlet ����� ���� ����**�� �� �ִ�.<br>
�׸��� request ��ü�� Model�� ����ϴ� ��ſ� ������ Model ��ü�� ���� ��ȯ�ϸ� �ȴ�.<Br>
�츮�� �����ϴ� controller�� servlet ����� ���� ������� �ʵ��� �����غ���.<br>
�̷��� �ϸ� ���� �ڵ嵵 �ſ� �ܼ�������, �׽�Ʈ �ڵ� �ۼ��� ����.

**�� �̸� �ߺ� ����**<br>
controller���� �����ϴ� view �̸��� �ߺ��� �ִ� ���� Ȯ���� �� �ִ�.<br>
controller�� **view�� �� �̸�**�� ��ȯ�ϰ�, ���� ���� ��ġ�� �̸��� front controller���� ó���ϵ��� �ܼ�ȭ ����.<br>
�̷��� �صθ� ���� view�� ���� ��ġ�� �Բ� �̵��ص� front controller�� ��ġ�� �ȴ�

- `/WEB-INF/views/new-form.jsp` -> **new-form**
- `/WEB-INF/views/save-result.jsp` -> **save-result**
- `/WEB-INF/views/members.jsp` -> **members**

**V3 ����**
![v3](./readme_img/v3.JPG)
- client�� http ��û�� ��
- front controller���� ���� ������ �����ͼ�
- controller�� ȣ����
- controller���� ModelView ��ȯ
- viewResolver ȣ��
- MyView ��ȯ
- render(model) ȣ��

**ModelView**<br>
���ݱ��� controller���� servlet�� �������� HtppServletRequest�� ����ߴ�. �׸��� Model�� `request.setAttribute()`�� ���� �����͸� �����ϰ� view�� �����ߴ�.<br>
servlet�� ���Ӽ��� �����ϱ� ���� Model�� ���� �����, �߰��� View �̸����� �����ϴ� ��ü�� ������.<br>
(�̹� ���������� controller���� HttpServletRequest�� ����� �� ����. ���� ���� `request.setAttribute()`�� ȣ���� �� �� ����. ���� Model�� ������ �ʿ��ϴ�.)

����� `ModelView`��ü�� �ٸ� ���������� ����ϹǷ� ��Ű���� `frontcontroller`�� �д�.

`createParamMap()`<br>
HttpServletRequest���� �Ķ���� ������ ������ Map���� ��ȯ�Ѵ�. �׸��� �ش� Map(`paramMap`)�� ��Ʈ�ѷ��� �����ϸ鼭 ȣ���Ѵ�.

**viewResolver**<br>
`MyView view = viewResolver(viewName)`<br>
��Ʈ�ѷ��� ��ȯ�� �� �� �̸��� ���� ���� �� ��η� �����Ѵ�. �׸��� ���� ���� ��ΰ� �ִ� MyView ��ü�� ��ȯ�Ѵ�.
- �� �� �̸� : `members`
- ���� �� ��� : `/WEB-INF/views/members.jsp`

`view.render(mv.getModel(), request, response)`
- �� ��ü�� ���ؼ� HTML ȭ���� ������ �Ѵ�.
- �� ��ü�� `render()`�� �� ������ �Բ� �޴´�.
- JSP�� `request.getAttribute()`�� �����͸� ��ȸ�ϱ� ������, ���� �����͸� ������ `request.setAttribute()`�� ��Ƶд�.
- JSP�� ������ �ؼ� JSP�� ������ �Ѵ�.

---

### �ܼ��ϰ� �ǿ����� ��Ʈ�ѷ� - V4

�ռ� ���� V3 ��Ʈ�ѷ��� servlet ���Ӽ��� �����ϰ� view ����� �ߺ��� �����ϴ� ��, �� ����� controller�̴�, �׷��� ���� controller interface�� �����ϴ� ������ ���忡�� ����, �׻� ModelView ��ü�� �������ϰ� ��ȯ�ؾ� �ϴ� �κ��� ���� ���ŷӴ�.<br>
���� �����ӿ�ũ�� ��Ű���ĵ� �߿�������, �׿� ���Ҿ� ���� �����ϴ� �����ڰ� �ܼ��ϰ� ���ϰ� ����� �� �־�� �Ѵ�. ���� �ǿ뼺�� �־�� �Ѵ�.

�̹����� v3�� ���� �����ؼ� ���� �����ϴ� �����ڵ��� �ſ� ���ϰ� ������ �� �ִ� v4 ������ �����غ���.

**V4 ����**
![v4](./readme_img/v4.JPG)
- �⺻���� ������ v3�� ����. ��ſ� controller�� `ModelView`�� ��ȯ���� ��Ȥ, `ViewName`�� ��ȯ�Ѵ�.

**ControllerV4**

�̹� ������ �������̽��� ModelView�� ����. model ��ü�� �Ķ���ͷ� ���޵Ǳ� ������ �׳� ����ϸ� �ǰ�, ����� view�� �̸��� ��ȯ���ָ� �ȴ�. 

**�� ��ü ����**<br>
`Map<String, Object> model = new HashMap<>(); //�߰�`<br>
�� ��ü�� ����Ʈ ��Ʈ�ѷ����� �����ؼ� �Ѱ��ش�. ��Ʈ�ѷ����� �� ��ü�� ���� ������ ���⿡ �״�� ����ְ� �ȴ�.

**���� �� �̸��� ���� ��ȯ**
```java
String viewName = controller.process(paramMap,model);
MyView view = viewResolver(viewName);
```
��Ʈ�ѷ��� ���� ���� �� �̸��� ��ȯ�ϹǷ� �� ���� ����ؼ� ���� ���� �並 ã�� �� �ִ�.

**����**<br>
�̹� ������ ��Ʈ�ѷ��� �ſ� �ܼ��ϰ� �ǿ����̴�. ���� �������� ���� �Ķ���ͷ� �ѱ��, ���� �� �̸��� ��ȯ�Ѵٴ� ���� ���̵� �������� ���ε�, controller�� �����ϴ� ������ ���忡�� ���� ���� �������� ���� �ڵ带 �ۼ� �� �� �ִ�.<br>
���� �߿��� ����� ������� �ѹ��� �� ���� �ƴ϶�� ���̴�. �����ӿ�ũ�� ���������� �����ϴ� ���� �ӿ��� �̷� ����� ã�� �� �־���.

**�����ӿ�ũ�� ���� ����� ����ο��� ����ϴ� �����ڰ� ��������.**

---

### ������ ��Ʈ�ѷ�1 - v5

���� `ControllerV3` ������� �����ϰ� �Ͱ�, �� `ControllerV4` ������� �����ϰ� �ʹٸ�??

```java
public interface ControllerV3{
  ModelView process(Map<String,String> paramMap);
}
```

```java
public interface ControllerV4{
  String process(Map<String,String> paramMap, Map<String, Object> model);
}
```

**����� ����**

`ControllerV3`,`ControllerV4`�� ������ �ٸ� �������̽� �̹Ƿ� ȣȯ�� �Ұ����ϴ�. �̷��� ����ϴ� ���� `�����`�̴�.

����� ������ ����ؼ� ����Ʈ ��Ʈ�ѷ��� �پ��� ����� ��Ʈ�ѷ��� ó���� �� �ֵ��� �����Ѵ�.

**V5 ����**
![v5](./readme_img/v5.JPG)
- client�� http ��û
- �ڵ鷯 ���ο��� �ڵ鷯 ��ȸ
- �ڵ鷯 ����� ��Ͽ��� �ڵ鷯�� ó���� �� �ִ� �ڵ鷯 ����� ��ȸ
- �ڵ鷯 ����͸� ���ؼ� ȣ���ؾ���(handle(handler))
  - ��, ����Ϳ��� controller�� �Ѱ���.
- �׷��� �ڵ鷯 ����Ͱ� handler�� ȣ������.
- �� ��, �ڵ鷯 ����Ͱ� ModelView�� ��ȯ���ش�.
- ������ logic�� �Ȱ���.

**�ڵ鷯 �����** : �߰��� ����� ������ �ϴ� ����Ͱ� �߰��Ǿ��µ�, �̸��� �ڵ鷯 ������̴�. ��???�� ����� ������ ���ִ� ���п� �پ��� ������ controller�� ȣ�� �� �� �ִ�

**�ڵ鷯** : controller�� �̸��� �� ���� ������ handler�� �����ߴ�. �� ������ ���� ����Ͱ� �ֱ� ������ �� controller�� ���� �� �ƴ϶� ��� ���̵� �ش��ϴ� ������ ����͸� ������ �� ó���� �� �ֱ� �����̴�.

**MyHandlerAdpater**

����ʹ� �̷��� �����ؾ� �Ѵٴ� ����Ϳ� �������̽��̴�.

- `boolean supports(Object handler)`
  - handler�� controller�� ���Ѵ�.
  - ����Ͱ� �ش� controller�� ó���� �� �ִ��� �Ǵ��ϴ� �޼���.
- `ModelView handle(HttpServletRequest request), HttpServletResponse response, Object handler) throws ServletException, IOException;`
  - ����ʹ� ���� controller�� ȣ���ϰ�, �� ����� ModelView�� ��ȯ.
  - ���� controller�� ModelView�� ��ȯ���� ���ϸ�, ����Ͱ� ModelView�� ���� �����ؼ��� ��ȯ�ؾ� �Ѵ�.
  - �������� front controller�� ���� controller�� ȣ�������� ������ �� ����͸� ���ؼ� ���� controller�� ȣ��ȴ�. 

**controller -> handler**<br>
�������� controller�� ���� �����ؼ� ����ߴ�. �׷��� ������ ����͸� ����ϱ� ������, controller �Ӹ� �ƴ϶� ����Ͱ� �����ϱ⸸ �ϸ�, � ���̶� URL�� �����ؼ� ����� �� �ִ�. �׷��� �̸��� controller���� �� ���� ������ handler�� ����.

**������**

```java
public FrontControllerServletV5() {
 initHandlerMappingMap(); //�ڵ鷯 ���� �ʱ�ȭ
 initHandlerAdapters(); //����� �ʱ�ȭ
}
```
�����ڴ� �ڵ鷯 ���ΰ� ����͸� �ʱ�ȭ(���)�Ѵ�.

**���� ����**
```java
private final Map<String, Object> handlerMappingMap = new HashMap<>();
```
���� ������ ���� ControllerV3 , ControllerV4 ���� �������̽����� �ƹ� ���̳� ���� �� �ִ�
Object �� ����Ǿ���.

**�ڵ鷯 ����**
```java
Object handler = getHandler(request)
private Object getHandler(HttpServletRequest request) {
 String requestURI = request.getRequestURI();
 return handlerMappingMap.get(requestURI);
}
```
�ڵ鷯 ���� ������ handlerMappingMap ���� URL�� ���ε� �ڵ鷯(��Ʈ�ѷ�) ��ü�� ã�Ƽ� ��ȯ�Ѵ�.

**�ڵ鷯�� ó���� �� �ִ� ����� ��ȸ**
```java
MyHandlerAdapter adapter = getHandlerAdapter(handler)
for (MyHandlerAdapter adapter : handlerAdapters) {
 if (adapter.supports(handler)) {
 return adapter;
 }
}
```
handler �� ó���� �� �ִ� ����͸� adapter.supports(handler) �� ���ؼ� ã�´�.<br>
handler�� ControllerV3 �������̽��� �����ߴٸ�, ControllerV3HandlerAdapter ��ü��
��ȯ�ȴ�.


**����� ȣ��**
```java
ModelView mv = adapter.handle(request, response, handler);
```
������� handle(request, response, handler) �޼��带 ���� ���� ����Ͱ� ȣ��ȴ�.<br>
����ʹ� handler(��Ʈ�ѷ�)�� ȣ���ϰ� �� ����� ����Ϳ� ���߾� ��ȯ�Ѵ�.<br>
ControllerV3HandlerAdapter �� ��� ������� ���� ��Ʈ�ѷ��� ����� �����ؼ� ��ȯ ������
�ܼ��ϴ�.

---

### ������ ��Ʈ�ѷ�2 - V5

`FrontControllerServletV5`�� `ControllerV4` ��ɵ� �߰��غ���.

---

### ����

v1 : front controller ����
- ���� ������ �ִ��� �����ϸ鼭 front controller�� ����.

v2 : View �з�
- �ܼ� �ݺ� �Ǵ� view ���� �и�

v3 : Model �߰�
- servlet ���Ӽ� ����
- view �̸� �ߺ� ����

v4 : �ܼ��ϰ� �ǿ����� controller
- v3�� ���� ���
- ���� ���忡�� ModelView�� ���� �����ؼ� ��ȯ���� �ʵ��� ���� �������̽� ����

v5 : ������ controller
- ����� ����
- ����͸� �߰��ؼ� �����ӟp���� �����ϰ� Ȯ�强 �ְ� ����

�ֳ����̼��� ����ؼ� controller�� �� ���ϰ� ������ų �� �ִ�. ���� �ֳ����̼��� ����ؼ� controller�� ���ϰ� ����� �� �ְ� �ҷ��� ��� �ؾ� �ұ�?<br>
-> �ٷ� �ֳ����̼��� �����ϴ� ����͸� �߰��ϸ� �ȴ�.<br>
�������� ����� ���п� ���� ������ �����ϸ鼭, �����ӿ�ũ�� ����� Ȯ���� �� �ִ�.

**������ MVC**<br>
���ݱ��� �ۼ��� �ڵ�� ������ MVC �����ӿ�ũ�� �ٽ� �ڵ��� ��� �����̰�, ������ ���� ����.


---
---

## ������ MVC - ���� ����

---
---

### ������ MVC ��ü ����

**���� ���� MVC �����ӿ�ũ ����**
![made](./readme_img/made.JPG)

**SpringMVC ����**
![mvc_archi](./readme_img/mvc_archi.JPG)

**��**
- FrontController -> DispatcherServlet(�߿�)
- handlerMappingMap -> HandlerMapping
- MyHandlerAdatper -> HandlerAdapter
- ModelView -> ModelAndView
- viewResolver -> ViewResolver
- MyView -> View

DispatcherServlet ���� ���캸��

```
org.springframework.web.servlet.DispatcherServlet
```

������ MVC�� front controller �������� �����Ǿ� �ִ�.<br>
������ MVC�� front controller�� �ٷ� DispatcherServlet�̴�.<br>
�׸��� �� DispatcherServlet�� �ٷ� Spring MVC�� �ٽ��̴�.

**DispatcherServlet ���� ���**
- `DispatcherServlet`�� �θ� Ŭ�������� `HttpServlet`�� ��� �޾Ƽ� ����ϰ�, �������� �����Ѵ�.
  - DispatcherServlet -> FrameworkServlet -> HttpServletBean -> HttpServlet
- ������ ��Ʈ�� `DispatcherServlet`�� �������� �ڵ����� ����ϸ鼭 `��� ���(urlPatterns="/")`�� ���ؼ� �����Ѵ�.
  - �� �ڼ��� ��ΰ� �켱������ ����.

**��û �帧**
- ������ ȣ��Ǹ� `HttpServlet`�� �����ϴ� `service()`�� ȣ��ȴ�.
- ������ MVC�� `DispatcherServlet`�� �θ��� `FrameworkServlet`���� `service()`�� �������̵� �صξ���.
- `FrameworkServlet.service()`�� �������� ���� �޼��尡 ȣ��Ǹ鼭 `DispatcherServlet.doDispatch()`�� ȣ��ȴ�.

**���ۼ���**
1. **�ڵ鷯 ��ȸ** : �ڵ鷯 ������ ���� ��û URL�� ���ε� �ڵ鷯(Controller)�� ��ȸ.
2. **�ڵ鷯 ����� ��ȸ** : �ڵ鷯�� ������ �� �ִ� �ڵ鷯 ����� ��ȸ.
3. **�ڵ鷯 ����� ����** : �ڵ鷯 ����͸� ����.
4. **�ڵ鷯 ����** : �ڵ鷯 ����Ͱ� ���� �ڵ鷯�� ����.
5. **ModelAndView ��ȯ** : �ڵ鷯 ����ʹ� �ڵ鷯�� ��ȯ�ϴ� ������ ModelAndView�� **��ȯ**�ؼ� ��ȯ.
6. **viewResolver ȣ��** : �� �������� ã�� ����.
   - JSP�� ��� : `InternalResourceViewResolver`�� �ڵ� ��ϵǰ�, ���ȴ�.
7. **View ��ȯ** : �� �������� ���� �� �̸��� ���� �̸����� �ٲٰ�, ������ ������ ����ϴ� �� ��ü�� ��ȯ.
   - JSP�� ��� : `InternalResourceView(JstlView)`�� ��ȯ�ϴµ�, ���ο� `forward()`������ �ִ�.
8. **�� ������** : �並 ���ؼ� �並 ������ �Ѵ�.

**�������̽� ���캸��**
- ������ MVC�� ū ����
  - `DispatcherServlet` �ڵ��� ���� ����, ���ϴ� ����� �����ϰų� Ȯ���� �� �ִ�.(�������̽��� �����ؼ�)
- �� �������̽��鸸 �����ؼ� `DispatcherServlet`�� ����ϸ� �츮�鸸�� controller�� ���� �� �ִ�.

�ֿ� �������̽� ���
- **�ڵ鷯 ����** : `org.springframework.web.servlet.HandlerMappgin`
- **�ڵ鷯 �����** : `org.springframework.web.servlet.HandlerAdapter`
- **�� ������** : `org.springframework.web.servlet.ViewResolver
- **��** : `org.springframework.web.servlet.View`

---

### �ڵ鷯 ���ΰ� �ڵ鷯 �����

������ ���� ������� ������, ���ſ� �ַ� ����ߴ� �������� �����ϴ� ������ controller�� �ڵ鷯 ���ΰ� ����͸� �����غ���.

#### Controller �������̽�
**���� ���� ������ ��Ʈ�ѷ�**
```java
public interface Controller{
  ModelAndView handleRequest(HttpServletRequest request, HttpServletResponse response) throws Exception;
}
```

>**����**
>
> `Controller` �������̽��� `@Controller`�� �ٸ���.

�� ��Ʈ�ѷ��� ȣ��Ƿ��� ���� 2������ �ʿ��ϴ�.

- **HandlerMapping(�ڵ鷯 ����)**
  - �ڵ鷯 ���ο��� �� controller�� ã�� �� �־�� �Ѵ�.
  - ex> **������ ���� �̸����� �ڵ鷯�� ã�� �� �ִ� �ڵ鷯 ����**�� �ʿ��ϴ�.
- **HandlerAdapter(�ڵ鷯 �����)**
  - �ڵ鷯 ������ ���ؼ� ã�� �ڵ鷯�� ������ �� �ִ� �ڵ鷯 ����Ͱ� �ʿ��ϴ�.
  - ex> `Controller` �������̽��� ������ �� �ִ� �ڵ鷯 ����͸� ã�� �����ؾ� �Ѵ�.

�������� �̹� �ʿ��� �ڵ鷯 ���ΰ� �ڵ鷯 ����͸� ��κ� �����س���. �����ڰ� ���� �ڵ鷯 ���ΰ� �ڵ鷯 ����͸� ����� ���� ���� ����.

**������ ��Ʈ�� �ڵ� ����ϴ� �ڵ鷯 ���̰� �ڵ鷯 �����**

**HandlerMapping**
- 0 ���� : RequestMappingHandlerMapping
  - �ֳ����̼� ����� ��Ʈ�ѷ��� `@RequestMapping`���� ���
- 1 ���� : BeanNameUrlHandlerMapping
  - ������ ���� �̸����� �ڵ鷯�� ã�´�.

**HandlerAdapter**
- 0 ���� : RequestMappingHandlerAdapter
  - �ֳ����̼� ����� ��Ʈ�ѷ��� `@RequestMapping`���� ���
- 1 ���� : HttpRequestHandlerAdapter
  - HttpRequestHandler ó��
- 2 ���� : SimpleControllerHandlerAdapter
  - Controller �������̽�(�ֳ����̼�x, ���ſ� ���) ó��

�ڵ鷯 ���ε�, �ڵ鷯 ����͵� ��� ������� ã�� ���� ������ ���� ������ �Ѿ��.

1. �ڵ鷯 �������� �ڵ鷯 ��ȸ
- `HandlerMapping`�� ������� �����ؼ�, �ڵ鷯�� ã�´�.
- �� ��� �� �̸����� �ڵ鷯�� ã�ƾ� �ϱ� ������ �̸� �״�� �� �̸����� �ڵ鷯�� ã���ִ� `BeanNameUrlHandlerMapping`�� ���࿡ �����ϰ� �ڵ鷯�� `OldController`�� ��ȯ�Ѵ�.
2. �ڵ鷯 ����� ��ȸ
- `HandlerAdapter`�� `supports()`�� ������� ȣ��.
- `SimpleControllerHandlerAdapter`�� `Controller` �������̽��� �����ϹǷ� ����� �ȴ�.
3. �ڵ鷯 ����� ����
- Dispatcher Servlet�� ��ȸ�� `SimpleControllerHandlerAdapter`�� �����ϸ鼭 �ڵ鷯 ������ �Բ� �Ѱ��ش�.
- `SimpleControllerHandlerAdapter`�� �ڵ鷯�� `OldController`�� ���ο��� �����ϰ�, �� ����� ��ȯ�Ѵ�.

**���� - OldController �ڵ鷯����, �����**
- `OldController`�� �����ϸ鼭 ���� ��ü�� ������ ����.
  - `HandlerMapping = BeanNameUrlHandlerMapping`
  - `HandlerAdapter = SimpleControllerHandlerAdapter`

---

### ������ MVC - �����ϱ�

�������� �����ϴ� controller�� �ֳ����̼� ������� �����ؼ�, �ſ� �����ϰ� �ǿ����̴�. ���ſ��� �ڹ� �� �ֳ����̼��� ���⵵ �߰�, �������� ó������ �̷� ������ controller�� ������ ���� �ƴϴ�.

**@RequestMapping**<br>
�������� �ֳ����̼��� Ȱ���� �ſ� �����ϰ�, �ǿ����� controller�� ������µ�, �̰��� �ٷ� `@RequestMapping` �ֳ����̼��� ����ϴ� controller�̴�.

`@RequestMapping`
- `RequestMappingHandlerMapping`
- `RequestMappingHandlerAdapter`

�ռ� ���ҵ��� ���� �켱������ �ڵ鷯 ���ΰ� �ڵ鷯 ����ʹ� `RequestMappingHandlerMapping`�� `RequestMappingHandlerAdapter`�̴�.<br>
`@RequestMapping`�� �ձ��ڸ� ���� ���� �̸��ε�, �̰��� �ٷ� ���� ���������� �ַ� ����ϴ� �ֳ����̼� ����� controller�� �����ϴ� �ڵ鷯 ���ΰ� ������̴�.


**SpringMemberFormControllerV1 - ȸ�� ��� ��**
```java
@Controller
public class SpringMemberFormControllerV1 {

  @RequestMapping("/springmvc/v1/members/new-form")
  public ModelAndView process(){
      return new ModelAndView("new-form");
  }
}
```
- `@Controller`
  - �������� �ڵ����� ������ ������ ����Ѵ�. (���ο� `@Component` �ֳ����̼��� �־ ������Ʈ ��ĵ�� ����� ��.)
  - ������ MVC���� �ֳ����̼� ��� controller�� �ν�.
- `@RequestMapping` : ��û ������ �����Ѵ�. �ش� URL�� ȣ��Ǹ� �� �޼��尡 ȣ��ȴ�. �ֳ����̼��� ������� �����ϱ� ������, �޼����� �̸��� ���Ƿ� ������ �ȴ�.
- `ModelAndView` : �𵨰� �� ������ ��Ƽ� ��ȯ�ϸ� �ȴ�.

`RequestMappingHandlerMapping`�� ������ �� �߿��� `@RequestMapping` �Ǵ� `@Controller`�� Ŭ���� ������ �پ� �ִ� ��쿡 ���� ������ �ν��Ѵ�.<br>
���� ���� �ڵ嵵 �����ϰ� ����.
```java
@Component
@RequestMapping
public class SpringMemberFormControllerV1{
  @RequestMapping("/spring/v1/members/new-form")
  public ModelAndView process(){
    return new ModelandView("new-form");
  }
}
}
```

---

### ������ MVC - ��Ʈ�ѷ� ����

`@RequestMapping`�� �� ���� Ŭ���� ������ �ƴ϶� �޼��� ������ ����� ���� Ȯ���� �� �ִ�. ���� ��Ʈ�ѷ� Ŭ������ �����ϰ� �ϳ��� ������ �� �ִ�.

---

## ������ MVC - �ǿ����� ���

MVC �����ӿ�ũ ����⿡�� v3�� ModelView�� �����ڰ� ���� �����ؼ� ��ȯ�߱� ������, �����ߴ�. ���� v4�� ����鼭 �ǿ������� ������.

������ MVC�� �����ڰ� ���ϰ� ������ �� �ֵ��� �� ���� ���� ����� ����.

**�ǹ������� ���ݺ��� �����ϴ� ����� �ַ� ���**

**Model �Ķ����**
- `save()`, `members()`�� ���� Model�� �Ķ���ͷ� �޴� ���� Ȯ���� �� �ִ�. ������ MVC�� �̷� ���� ����� ����.

**ViewName ���� ��ȯ**
- ���� �� �̸��� ��ȯ�� �� �ִ�.

**@RequestParam ���**
- �������� HTTP ��û �Ķ���͸� `@RequestParam`���� ���� �� �ִ�.
- `@RequestParam("username")`�� `request.getParameter("username")`�� ���� ���� �ڵ�.
- ���� GET ���� �Ķ����, POST Form ��� ��� ����

**@RequestMapping -> @GetMapping, @PostMapping**
- `@RequestMapping`�� URL�� ��Ī�ϴ� ���� �ƴ϶�, HTTP Method�� �Բ� ������ �� �ִ�.
- ���� �� URL�� `/new-form`�̰�, HTTP Method�� GET�� ��츦 ��� �����ϴ� ������ �Ϸ��� ������ ���� ó��.
```java
@RequestMapping(value = "/new-form",method=RequestMethod.GET)
```

�̰��� `@GetMapping`, `@PostMapping`���� �� ���ϰ� ��밡��.

����� Get,Post,Delte,Patch ��� �ֳ����̼��� �غ��.

---
---

## ������ MVC - �⺻ ���

---
---

### ������Ʈ ����

start.spring.io

- Project : Gradle
- Language : Java
- Spring Boot : 2.4.4
- Project Metadata
  - Group : hello
  - Artifact : springmvc
- Packaing : Jar
- Java : 11
- Dependencies
  - Spring Web
  - Thymeleaf
  - Lombok

�� Jar�ΰ�?
- JSP�� ������� �ʱ� ������ Jar�� ����ϴ� ���� ����.
- Jar�� ����ϸ� �׻� ���� ����(��Ĺ��)�� ����ϰ�, `webapp` ��ε� ������� �ʴ´�. ���� ���� ��뿡 ����ȭ �Ǿ� �ִ� ����̴�. �ֱٿ� �ַ� �̹���� ���.
- War�� ����ϸ� ���� ������ ��밡�� ������, �ַ� �ܺ� ������ �����ϴ� �������� ���.
  - War�� ���� ��Ĺ���� WAS������ ������ ��ġ�ϰ� �ű⿡ ����� ������ ������
  - Ȥ�� jsp�� ����Ҷ�

���� localhost:8080�ߴµ� ������ �ϴ��� ���´�??<br>
-> �� ������ ĳ�ö�����. �׳� refresh�ϸ� ����ȭ���� ����� ���´�.(�츮�� ĳ���� �����ʴ´ٰ� ���� �ʾƼ� �׷�.)

������ ��Ʈ�� `Jar`�� ����ϸ� `/resource/static/index.html` ������ �θ� Welcome�������� ó�����ش�.(������ ��Ʈ�� �����ϴ� ���� ������ ��ġ�� `/index.html`�� ������ �ȴ�.)

> ����
>
> ������ ��Ʈ Welcome ������ ���� �ڼ��� ��
> > https://docs.spring.io/spring-boot/docs/current/reference/html/spring-bootfeatures.html#boot-features-spring-mvc-welcome-page

---

### �α� ������ �˾ƺ���

� �ý��ۿ����� `SYstem.out.println()`���� �ý��� �ܼ��� ����ؼ� �ʿ��� ������ ������� �ʰ�, ������ �α� ���̺귯���� ����ؼ� �α׸� ����Ѵ�.

**�α� ���̺귯��**<br>
������ ��Ʈ ���̺귯���� ����ϸ� ������ ��Ʈ �α� ���̺귯��(`spinrg-boot-starter-logging`)�� �Բ� ���Եȴ�.<Br>
������ ��Ʈ �α� ���̺귯���� �⺻���� ���� �α� ���̺귯���� ����Ѵ�.

- SLF4J(�������̽�)
- Logback(����ü)

������ ��Ʈ�� �⺻���� �����ϴ� Logback�� ��κ� �����.

**�α� ����**<br>
- `private Logger log = LoggerFactory.getLogger(getClass());`
- `private static final Logger log = LoggerFactory.getLogger(Xxx.class)`
- `@Slf4j` : �Һ� ��밡��

**�α� ȣ��**<br>
- `log.info("hello")`
- `System.out,println("hello")`
  - �ý��� �ַܼ� ���� ����ϴ� �� ���� �α׸� ����ϸ� ������ ���� ������ �ִ�. �׻� �α� ���!

```
2021-03-23 01:46:46.056  INFO 2328 --- [nio-8080-exec-9] hello.springmvc.basic.LogTestController  :  info log =Spring
```
- ���� ���� �αװ� ����
- �ð�, INFO, process ID, ���� ������ ������, ������ ���� Controller�̸�, �޽��� ���

```java
log.trace("trace log={}",name);
log.debug("debug log={}",name);
log.info(" info log ={}",name);
log.warn(" warn log ={}",name);
log.error("error log={}",name);
```
- log�� ������ level�� ���� �� �ִ�.(�� log�� � ������ �����̴�.)
- ex> debug -> ���� �α״� ������Ҷ� ���°Ŵ�.(���� ����)
- ex> info -> ���� �α״� �߿��� ������(����Ͻ� ����, ��ý��ۿ��� ������ ����..)
- ex> warn -> ���
- ex> error -> Ȯ���ؾ��� error!
- trace�� debug�� �Ⱥ���

���� ������ ���ÿ��� �����Ѵٰ� �����ϰ�, ��� �α׸� ���� ������ application.properites���� ����
```
#hello.springmvc ��Ű���� �� ���� �α� ���� ���� ����
logging.level.hello.springmvc=trace
```
- �̷����ϸ�, trace�� debug�α׵� �߰��� ����

```
#hello.springmvc ��Ű���� �� ���� �α� ���� ���� ����
logging.level.hello.springmvc=debug
```
- �̷���, debug,info,warn,error�� ����

��, ���߼����� debug������ �صΰ� ���� ����pc������ trace�� �ٲٰ� debug�� �ٲٰ� �̷��� ���°���<br>
�׷��ٰ� ��������� info level�� ������.
```
logging.level.hello.springmvc=info
```

**���� ����**
- `@RestController`
  - `@Controller`�� ��ȯ ���� `String`�̸� �� �̸����� �νĵȴ�. �׷��� **�並 ã�� �䰡 ������**�ȴ�.
  - `@RestController`�� ��ȯ ������ �並 ã�� ���� �ƴ϶�, **HTTP �޽��� �ٵ� �ٷ� �Է�**�Ѵ�. ���� ���� ����� ok �޼����� ���� �� �ִ�. `@ResponseBody`�� ������ �ִµ�, �ڿ��� �� �ڼ��� �����Ѵ�.

**�׽�Ʈ**
- �αװ� ��µǴ� ���� Ȯ��
  - �ð�, �α� ����, ���μ��� ID, ������ ��, Ŭ���� ��, �α� �޽���
- �α� ���� ������ �����ؼ� ��� ����� ����.
  - LEVEL : `TRACE > DEBUG > INFO > WARN > ERROR`
  - ���� ������ debug ���
  - � ������ info ���
- `@Slf4j`�� ����

**�α� ���� ����**
```
#��ü �α� ���� ����(�⺻ info)
logging.level.root=info
#hello.springmvc ��Ű���� �� ���� �α� ���� ����
logging.level.hello.springmvc=debug
```

`@Slf4j`�� ������ �Ʒ��� ���� ����.
```java
@Slf4j
@RestController
public class LogTestController {

//    private final Logger log = LoggerFactory.getLogger(getClass());

    @RequestMapping("/log-test")
    public String logTest(){
        String name = "Spring";
        System.out.println("name = " + name);

        log.trace("trace log={}",name);
        log.debug("debug log={}",name);
        log.info(" info log ={}",name);
        log.warn(" warn log ={}",name);
        log.error("error log={}",name);


        return "ok";
    }
}
```

**�ùٸ� �α� ����**<br>
- `log.debug("data="+data)`
  - �α� ��� ������ info�� �����ص� �ش� �ڵ忡 �ִ� "data="+data�� ���� ������ �Ǿ� ������. ��������� **���� ���ϱ� ������ �߻��Ѵ�.**
- `log.debug("data={}",data)`
  - �α� ��� ������ info�� �����ϸ� �ƹ��ϵ� �߻����� �ʴ´�. ���� �հ� ���� **�ǹ̾��� ������ �߻����� �ʴ´�.**


**�α� ���� ����**
- ������ ����, Ŭ���� �̸� ���� �ΰ� ������ �Բ� �� �� �ֲ�, ��� ����� ������ �� �ִ�.
- �α� ������ ���� ���� ���������� ��� �α׸� ����ϰ�, ����������� ������� �ʴ� �� �α׸� ��Ȳ�� �°� ������ �� �ִ�.
- �ý��� �ƿ� �ֿܼ��� ����ϴ� ���� �ƴ϶�, �����̳� ��Ʈ��ũ ��, �α׸� ������ ��ġ�� ���� �� �ִ�. Ư�� ���Ϸ� ���� ���� �Ϻ�, Ư�� �뷮�� ���� �α׸� �����ϴ� �͵� �����ϴ�.
- ���ɵ� �Ϲ� System.out���� ����.(���� ���۸�, ��Ƽ ������ ���) �׷��� �ǹ������� �� �α׸� �����.

**�� �������ڸ�?**<br>
- �α׿� ���ؼ� �� �ڼ��� ������ slf4j, logback �˻�
  - SLF4J = http://www.slf4j.org
  - Logback = http://logback.qos.ch

---

### ��û ����

- ��û �����̶�
  - ��û�� ������ � controller�� ȣ���� �Ǿ�� ��! �̰��� �����ϴ� ��

**���� ����**
- `@RestController`
  - `@Controller`�� ��ȯ ���� `String`�̸� �� �̸����� �ν�. �׷��� **�並 ã�� �䰡 ������** �ȴ�.
  - `@RestController`�� ��ȯ ������ �並 ã�� ���� �ƴ϶�, **HTTP �޽��� �ٵ� �ٷ� �Է�**�Ѵ�. ���� ���� ���� ok �޼����� ���� �� �ִ�. `ResponseBody`�� ������ �ִ�.
- `@RequestMapping("/hello-basic")`
  - `/hello-basic` URL ȣ���� ���� �� �޼��尡 ����ǵ��� ����.
  - ��κ��� �Ӽ��� `�迭[]`�� �����ϹǷ� ���� ������ ����. `{"/hello-basic","/hello-go"}`

**�Ѵ� ���** 
- �ٸ� URL������, �������� ���� URL ��û���� ���� ��û���� ����.
  - ���� : `/hello-basic`
  - URL ��û : `/hello-basic`, `/hello-basic/`

**HTTP �޼���**
- `@RequestMapping`�� `method` �Ӽ����� HTTP �޼��带 �������� ������ HTTP �޼���� �����ϰ� ȣ��ȴ�. 
- ��� ��� GET, HEAD, POST, PUT, PATCH, DELETE

**HTTP �޼��� ���� ���**
- `@GetMapping`
- `@PostMapping`
- `@PutMapping`
- `@DeleteMapping`
- `@PatchMapping`

**PathVariable(��� ����) ���(���� �̷��� ���� ���)**

```java
/**
  * PathVariable ���
  * �������� ������ ���� ����
  * @PathVariable("userId") String userId -> @PathVariable userId
  * ��û URL�� /mapping/userA �̷������� ��
  */
@GetMapping("/mapping/{userId}")
public String mappingPath(@PathVariable("userId") String data){
    log.info("mappingPath userId=[}", data);
    return "ok";
}
```

�ֱ� HTTP API�� ������ ���� ���ҽ� ��ο� �ĺ��ڸ� �ִ� ��Ÿ���� ��ȣ�Ѵ�.
- `/mapping/userA`
- `/users/1`
- ����Ѱ� ���� �Ķ���� ���
  - ex> `?userId=userA`
<br>

- `@RequestMapping`�� URL ��θ� ���ø�ȭ �� �� �ִµ�, `@PathVariable`�� ����ϸ� ��Ī �Ǵ� �κ��� ���ϰ� ��ȸ�� �� �ִ�.
- `@PathVariable`�� �̸��� �Ķ���� �̸��� ������ ������ �� �ִ�.
  - 
  ```java
  @GetMapping("/mapping/{userId}")
  public String mappingPath(@PathVariable String userId){
      log.info("mappingPath userId=[}", userId);
      return "ok";
  }
  ```

**PathVariable ��� - ����**

```java
/**
  * PathVariable ��� ����
  */
@GetMapping("/mapping/users/{userId}/orders/{orderId}")
public String mappingPath(@PathVariable String userId, @PathVariable Long orderId){
    log.info("mappingPath userId={}, orderId={}",userId,orderId);
    return "ok";
}
```

**Ư�� �Ķ���� ���� ���� (�� ��������� ����)**

```java
/**
 * �Ķ���ͷ� �߰� ����
 * params="mode",
 * params="!mode"
 * params="mode=debug"
 * params="mode!=debug" (! = )
 * params = {"mode=debug","data=good"}
 */
@GetMapping(value = "/mapping-param", params = "mode=debug")
public String mappingParam() {
 log.info("mappingParam");
 return "ok";
}
```
- Ư�� �Ķ���Ͱ� �ְų� ���� ������ �߰��� �� �ִ�. �� ��������� �ʴ´�.

**Ư�� ��� ���� ����**

```java
/**
 * Ư�� ����� �߰� ����
 * headers="mode",
 * headers="!mode"
 * headers="mode=debug"
 * headers="mode!=debug" (! = )
 */
@GetMapping(value = "/mapping-header", headers = "mode=debug")
public String mappingHeader() {
 log.info("mappingHeader");
 return "ok";
}
```
- �Ķ���� ���ΰ� ���������, HTTP ����� ����Ѵ�.
- **Postman���� �׽�Ʈ �ؾ� ��.**

**�̵�� Ÿ�� ���� ���� - HTTP ��û Content-Type, consume**

```java
/**
 * Content-Type ��� ��� �߰� ���� Media Type
 * consumes="application/json"
 * consumes="!application/json"
 * consumes="application/*"
 * consumes="*\/*"
 * MediaType.APPLICATION_JSON_VALUE
 */
@PostMapping(value = "/mapping-consume", consumes = "application/json")
public String mappingConsumes() {
 log.info("mappingConsumes");
 return "ok";
}
```
- **Postman���� �׽�Ʈ �ؾ� �Ѵ�.**
- �� �ڵ�� ����� Content-Type�� application/json�̾�߸� ȣ���� ��.
- HTTP ��û�� Content-Type ����� ������� �̵�� Ÿ������ �����Ѵ�.
- ���� ���� ������ HTTP 415 �����ڵ�(Unsupported Media Type)�� ��ȯ.
- ���� ���忡���� �Һ��ϴϱ� consume

**�̵�� Ÿ�� ���� ���� - HTTP ��û Accept, produce**

```java
/**
 * Accept ��� ��� Media Type
 * produces = "text/html"
 * produces = "!text/html"
 * produces = "text/*"
 * produces = "*\/*"
 */
@PostMapping(value = "/mapping-produce", produces = "text/html")
public String mappingProduces() {
 log.info("mappingProduces");
 return "ok";
}
```
- HTTP ��û�� Accept ����� ������� �̵�� Ÿ������ �����Ѵ�.
- ���� ���� ������ HTTP 406 �����ڵ�(Not Acceptable)��ȯ.

---

### ��û ���� - API ����

ȸ�� ������ HTTP API�� ����� �����ϰ� ������ ��� �ϴ��� �˾ƺ���.(���� �����Ͱ� �Ѿ�� �κ��� �����ϰ� URL ���θ�)

**ȸ�� ���� API**
- ȸ�� ��� ��ȸ: GET `/users`
- ȸ�� ��� : POST `/users`
- ȸ�� ��ȸ : GET `/users/{userId}`
- ȸ�� ���� : PATCH `/users/{userId}`
- ȸ�� ���� : DELETE `/users/{userId}`

MappingClassController �����

---

### HTTP ��û - �⺻, ��� ��ȸ

�ֳ����̼� ����� ������ ��Ʈ�ѷ��� �پ��� �Ķ���͸� �����Ѵ�.<br>
�̹� �ð����� HTTP ��� ������ ��ȣ�ϴ� ����� �˾ƺ���.

RequestHeaderController �����

```java
@Slf4j
@RestController
public class RequestHeaderController {

    @RequestMapping("/headers")
    public String headers(HttpServletRequest request,
                          HttpServletResponse response,
                          HttpMethod httpMethod,
                          Locale locale,
                          @RequestHeader MultiValueMap<String, String> headerMap,
                          @RequestHeader("host") String host,
                          @CookieValue(value="myCookie", required = false) String cookie
                          ){
        log.info("request={}", request);
        log.info("response={}", response);
        log.info("httpMethod={}", httpMethod);
        log.info("locale={}", locale);
        log.info("headerMap={}", headerMap);
        log.info("header host={}", host);
        log.info("myCookie={}", cookie);

        return "ok";
    }

}

```
- `HttpServletRequest`
- `HttpServletResponse`
- `HttpMethod` : HTTP �޼��带 ��ȸ�Ѵ�. `org.spring.framework.http.HttpMethod`
- `Locale` : Locale ������ ��ȸ�Ѵ�.
- `@RequestHeader MultiValueMap<String, String> headerMap`
  - ��� HTTP ����� MultiValueMap �������� ��ȸ.
- `@RequestHeader("host") String host`
  - Ư�� HTTP ����� ��ȸ�Ѵ�.
  - �Ӽ�
    - �ʼ� �� ���� : `required`
    - �⺻ �� �Ӽ� : `defaultValue`
  - `@CookieValue(value="myCookie",required=false) String cookie`
    - Ư�� ��Ű�� ��ȸ.
    - �Ӽ�
      - �ʼ� �� ���� : `required`
      - �⺻ �� : `defaultValue`

`MultiValueMap`
- MAP�� �����ѵ�, �ϳ��� key�� ���� value�� ���� �� �ִ�.
- HTTP header, HTTP ���� �Ķ���Ϳ� ���� �ϳ��� key�� ���� value ���� ���� �� ���.
  - **keyA=value1&keyA=value2**
- �迭�� return ��
  - 
  
```java
MultiValueMap<String, String> map = new LinkedMultiValueMap();
map.add("keyA","value1");
map.add("keyA","value2");

//[value1,value2]
List<String> values = map.get("keyA");

```


> ����<br>
> `@Conroller` �� ��� ������ �Ķ���� ����� ���� ���� �޴��󿡼� Ȯ���� �� �ִ�.<br>
> https://docs.spring.io/spring-framework/docs/current/reference/html/web.html#mvc-annarguments
> ����<br>
> `@Conroller` �� ��� ������ ���� �� ����� ���� ���� �޴��󿡼� Ȯ���� �� �ִ�.<br>
> https://docs.spring.io/spring-framework/docs/current/reference/html/web.html#mvc-annreturn-types


---

### Http ��û �Ķ���� - ���� �Ķ����, HTML Form

#### HTTP ��û ������ ��ȸ - ����

**client���� server�� ��û �����͸� ������ ���� �ַ� ���� 3���� ��� ���.**
- **GET - ���� �Ķ����**
  - /url?**username=hello&age=20**
  - �޽��� �ٵ� ����, URL�� ���� �Ķ���Ϳ� �����͸� �����ؼ� ����
  - ex> �˻�, ����, ����¡��
- **POST - HTML Form**
  - content-type : application/x-www-form-urlencoded
  - �޽��� �ٵ� ���� �Ķ���� �������� ���� username=hello&age=20
  - ex> ȸ�� ����, ��ǰ �ֹ�, HTML Form ���
- **HTTP message body**�� �����͸� ���� ��Ƽ� ��û
  - HTTP API���� �ַ� ���, JSON, XML, TEXT
  - ������ ������ �ַ� JSON ���
  - POST, PUT, PATCH

#### ��û �Ķ���� - ���� �Ķ����, HTML Form

`HttpServletRequest`�� `request.getParameter()`�� ����ϸ� ���� 2���� ��û �Ķ���� ��ȸ ����.

**GET, ���� �Ķ���� ����**<BR>
����<BR>
`http://localhost:8080/request-param?username=hello&age=20`

**POST,HTML Form ����**<br>

GET ���� �Ķ���� ���� ����̵�, POST HTML Form ���� ����̵� �� �� ������ �����Ƿ� ���о��� ��ȸ ����.<br>
�̰��� ������ **��û �Ķ����(request parameter)��ȸ**�� �Ѵ�.

> **����**<br>
> `Jar`�� ����ϸ� `webapp`��θ� ����� �� ����. �������� ���� ���ҽ��� Ŭ���� ��ο� �Բ� �����ؾ� �Ѵ�.

---

### HTTP ��û �Ķ���� - @RequestParam

�������� �����ϴ� `@RequestParam`�� ����ϸ� ��û �Ķ���͸� �ſ� ���ϰ� ��� ����.

**requestParamV2**

```java
@ResponseBody
@RequestMapping("/request-param-v2")
public String requestParamV2(
        @RequestParam("username") String memberName,
        @RequestParam("age") int memberAge){

    log.info("username={}, age={}",memberName,memberAge);
    return "ok";
}
```
- `@RequestParam` : �Ķ���� �̸����� ���ε�
- `ResponseBody` : View ��ȸ�� �����ϰ�, HTTP message body�� ���� �ش� ���� �Է�

**@RequestParam**�� `name(value)` �Ӽ��� �Ķ���� �̸����� ���
- @RequestParam("**username**") String **memberName**
- -> request.getParameter("**username**")

**requestParamV4**

```java
@ResponseBody
@RequestMapping("/request-param-v4")
public String requestParamV4(String username, int age){
    log.info("username={}, age={}",username,age);
    return "ok";
}
```
- `String`, `int`, `Integer` ���� �ܼ� Ÿ���̸� `@RequestParam` �� ���� ����.

>**����**<br>
>�̷��� �ֳ����̼��� ������ �����ص� �ǳ� `@RequestParam`�� ������ ��Ȯ�ϰ� ��û �Ķ���Ϳ��� �����͸� �д� �ٴ� ���� ��������� �� �� ����.

**�Ķ���� �ʼ� ���� - requestParamRequired**

```java
@ResponseBody
@RequestMapping("/request-param-required")
public String requestParamRequired(
        @RequestParam(required = true) String username,
        @RequestParam(required = false) Integer age){
    //Integer�� ��ü�̹Ƿ� null�� �� �� ����
    log.info("username={}, age={}",username,age);
    return "ok";
}
```
- `@RequestParam.required`
  - �Ķ���� �ʼ� ����
  - �⺻���� �Ķ���� �ʼ�(`true`)�̴�.

- `/request-param` ��û
  - `username`�� �����Ƿ� 400 ���ܰ� �߻��Ѵ�.

**����! - �Ķ���� �̸��� ���**<br>
`/request-param?username=`<br>
�Ķ���� �̸��� �ְ� ���� ���� ��� -> ���ڷ� ���

**����! - �⺻��(primitive)�� null �Է�**<br>
- `/request-param` ��û
- `@RequestParam(required = false) int age`

`null`�� `int`�� �Է��ϴ� ���� �Ұ���(500 ����)<br>
���� `null`�� ���� �� �ִ� `Integer`�� �����ϰų�, �Ǵ� ������ ������ `defaultValue` ���


**�⺻ �� ���� - requestParamDefault**<br>
```java
@ResponseBody
@RequestMapping("/request-param-default")
public String requestParamDefault(
        @RequestParam(required = true, defaultValue = "guset") String username,
        @RequestParam(required = false, defaultValue = "-1") int age){
    //Integer�� ��ü�̹Ƿ� null�� �� �� ����
    log.info("username={}, age={}",username,age);
    return "ok";
}
```

�Ķ���Ϳ� ���� ���� ��� `defaultValue`�� ����ϸ� �⺻ �� ����.<Br>
�̹� �⺻ ���� �ֱ� ������ `required`�� �ǹ̰� ����.

`defaultValue`�� �� ������ ��쿡�� ������ �⺻ ���� ����ȴ�.<br>
`/request-param?username=`

**�Ķ���͸� Map���� ��ȸ�ϱ� - requestParamMap**
```java
@ResponseBody
@RequestMapping("/request-param-map")
public String requestParamMap(@RequestParam Map<String,Object> paramMap){
    log.info("username={}, age={}",paramMap.get("username"),paramMap.get("age"));
    return "ok";
}
```

�Ķ���͸� Map, MultiValueMap���� ��ȸ�� �� �ִ�<br>
- `@RequestParam Map`
  - `Map(key=value)`
- `@RequestParam MultiValueMap`
  - `MultiValueMap(key=[value1,value2,...] ex) (key=userId, value=[id1,id2])`

�Ķ������ ���� 1���� Ȯ���ϴٸ� `Map`�� ����ص� ������, �׷��� �ʴٸ� `MultiValueMap`�� �������.

---

### HTTp ��û �Ķ���� - @ModelAttribute

���� ������ �ϸ� ��û �Ķ���͸� �޾Ƽ� �ʿ��� ��ü�� ����� �� ��ü�� ���� �־��־�� �Ѵ�. ���� ������ ���� �ڵ带 �ۼ��� ���̴�.
```java
@RequestParam String username;
@RequestParam int age;

HelloData data = new HelloData();
data.setUsername(username);
data.setAge(age);
```

�������� �� ������ ������ �ڵ�ȭ���ִ� `@ModelAttribute` ����� ����.

���� ��û �Ķ���͸� ���ε� ���� ��ü�� ������.

**HelloData**
```java
package hello.springmvc.basic;

import lombok.Data;

@Data
public class HelloData {
    private String username;
    private int age;
}
```
- lombok�� `@Data`
  - `@Getter`, `@Setter`, `@ToString`, `@EqualsAndHashCode`, `@RequiredArgsConstructor` �� �ڵ����� �������ش�.

**@ModelAttribute ���� - modelAttributeV1**

```java
@ResponseBody
@RequestMapping("/model-attribute-v1")
public String modelAttributeV1(@ModelAttribute HelloData helloData){
    log.info("username={}, age={}",helloData.getUsername(),helloData.getAge());
    return "ok";
}
```
�˾Ƽ� `HelloData` ��ü�� �����ǰ�, ��û �Ķ������ ���� ����.

������MVC�� `@ModelAttribute`�� ������ ������ ����.
- `HelloData` ��ü ����
- ��û �Ķ������ �̸����� `HelloData` ��ü�� ������Ƽ�� ã�´�. �׸��� �ش� ������Ƽ�� setter�� ȣ���ؼ� �Ķ������ ���� �Է�(���ε�)�Ѵ�.
- ex> �Ķ���� �̸��� `username`�̸� `setUsername()` �޼��带 ã�Ƽ� ȣ���ϸ鼭 ���� �Է��Ѵ�.

**������Ƽ**<br>
��ü�� `getUsername()`, `setUsername()` �޼��尡 ������, �� ��ü�� `username`�̶�� ������Ƽ�� ������ �ִ�.<br>
`username`������Ƽ�� ���� �����ϸ�, `setUsername()`�� ȣ��ǰ�, ��ȸ�ϸ� `getUsername()`�� ȣ��ȴ�.
```java
class HelloData{
  getUsername();
  setUsername();
}
```

 **���ε� ����**<br>
 `age=abc`ó�� ���ڰ� ���� �� ���� ���ڸ� ������ `BindException`�� �߻�. �̷� ���ε� ������ ó���ϴ� ����� ���� �κп��� �ٷ��.

**@ModelAttribute ���� - modelAttributeV2**<br>
```java
@ResponseBody
@RequestMapping("/model-attribute-v2")
public String modelAttributeV2(HelloData helloData){
  log.info("username={}, age={}",helloData.getUsername(),helloData.getAge());
  return "ok";
}
```
`@ModelAttribute`�� ������ �� �ִ�.<br>
�׷��� `@RequestParam`�� ������ �� ������ ȥ�� �߻��� �� �ִ�.

�������� �ش� ������ ������ ���� ��Ģ ����.
- `String`, `int`, `Integer` ���� �ܼ� Ÿ�� = `@RequestParam`
- ������ = `@ModelAttribute`(argument resolver �� �����ص� Ÿ�� ��)

---

### HTTP ��û �޽��� - �ܼ� �ؽ�Ʈ

- **HTTP message body**�� �����͸� ���� ��Ƽ� ��û
  - HTTP API���� �ַ� ���, JSON, XML, TEXT
  - ������ ������ �ַ� JSON
  - POST,PUT,PATCH

��û �Ķ���Ϳ� �ٸ���, HTTP �޽��� �ٵ� ���� �����Ͱ� ���� �����Ͱ� �Ѿ���� ���� `@RequestParam`, `@ModelAttribute`�� ����� �� ����.(���� HTML Form �������� ���޵Ǵ� ���� ��û �Ķ���ͷ� �����ȴ�.)

- HTTP �޽��� �ٵ��� �����͸� `InputStream`�� ����ؼ� ���� ���� �� �ִ�.

**RequestBodyStringController**<br>
```java
@Slf4j
@Controller
public class RequestBodyStringController {

    @PostMapping("/request-body-string-v1")
    public void requestBodyString(HttpServletRequest request, HttpServletResponse response) throws IOException {
        ServletInputStream inputStream = request.getInputStream();
        String messageBody = StreamUtils.copyToString(inputStream, StandardCharsets.UTF_8);

        log.info("messageBody={}",messageBody);

        response.getWriter().write("ok");
    }
```

**Input, Output ��Ʈ��, Reader - requestBodyStringV2**
```java
@PostMapping("/request-body-string-v2")
public void requestBodyStringV2(InputStream inputStream, Writer responseWriter) throws IOException {
    String messageBody = StreamUtils.copyToString(inputStream, StandardCharsets.UTF_8);
    log.info("messageBody={}",messageBody);
    responseWriter.write("ok");
}
```

**������ MVC�� ���� �Ķ���͸� �����Ѵ�.**<br>
InputStream(Reader): HTTP ��û �޽��� �ٵ��� ������ ���� ��ȸ<br>
OutputStream(Writer): HTTP ���� �޽����� �ٵ� ���� ��� ���<br>

**HttpEntity - requestBodyStringV3**<br>

```java
@PostMapping("/request-body-string-v3")
public HttpEntity<String> requestBodyStringV3(HttpEntity<String> httpEntity) throws IOException {

    String messageBody = httpEntity.getBody();
    log.info("messageBody={}",messageBody);
    
    return new HttpEntity<>("ok");
}
```

**������ MVC�� ���� �Ķ���͸� �����Ѵ�.**<br>
- **HttpEntity**: HTTP header, body ������ ���ϰ� ��ȸ
  - �޽��� �ٵ� ������ ���� ��ȸ
  - ��û �Ķ���͸� ��ȸ�ϴ� ��ɰ� ���� ���� `@RequestParam` X, `@ModelAttribute` X
- **HttpEntity�� ���信�� ��� ����**
  - �޽��� �ٵ� ���� ���� ��ȯ
  - ��� ���� ���� ����
  - view ��ȸX

`HttpEntity` �� ��ӹ��� ���� ��ü�鵵 ���� ����� �����Ѵ�.
- **RequestEntity**
  - HttpMethod, url ������ �߰�, ��û���� ���
- **ResponseEntity**
  - HTTP ���� �ڵ� ���� ����, ���信�� ���
  - `return new ResponseEntity<String>("Hello World", responseHeaders,HttpStatus.CREATED)`

> **����**<br>
> ������MVC ���ο��� HTTP �޽��� �ٵ� �о ���ڳ� ��ü�� ��ȯ�ؼ� �������ִµ�, �̶� HTTP �޽��� ������(`HttpMessageConverter`)��� ����� ����Ѵ� �̰��� ���� �� HTTP �޽��� �����Ϳ��� �ڼ��� ����.

**@RequestBody - requestBodyStringV4**<br>
```java
@PostMapping("/request-body-string-v4")
public HttpEntity<String> requestBodyStringV4(@RequestBody String messageBody){
    log.info("messageBody={}",messageBody);
    return new HttpEntity<>("ok");
}
```

**@RequestBody**<br>
`@RequestBody`�� ����ϸ� HTTP �޽��� �ٵ� ������ ���ϰ� ��ȸ�� �� �ִ�. ����� ��� ������ �ʿ��ϴٸ� `HttpEntity`�� ����ϰų� `@RequestHeader`�� ����ϸ� �ȴ�.<br>
�̷��� �޽��� �ٵ� ���� ��ȸ�ϴ� ����� ��û �Ķ���͸� ��ȸ�ϴ� `@RequestParam`,`@ModelAttribute`�ʹ� ���� ���谡 ����.

**��û �Ķ���� vs HTTP �޽��� �ٵ�**<br>
- ��û �Ķ���͸� ��ȸ�ϴ� ��� : `@RequestParam`, `@ModelAttribute`
- HTTP �޽��� �ٵ� ���� ��ȸ�ϴ� ��� : `@RequestBody`

**@ResponseBody**<br>
`@ResponseBody`�� ����ϸ� ���� ����� HTTP �޽��� �ٵ� ���� ��Ƽ� ������ �� �ִ�.<BR>
���� �� ��쿡�� view�� ������� �ʴ´�.

---

### HTTP ��û �޽��� - JSON

HTTP API���� �ַ� ����ϴ� JSON ������ ���� ��ȸ.

**RequestBodyJsonControllerV3 - @RequestBody ��ü ��ȯ**
```java
@ResponseBody
@PostMapping("/request-body-json-v3")
public String requestBodyJsonV3(@RequestBody HelloData helloData){
    log.info("username={}, age={}",helloData.getUsername(),helloData.getAge());
    return "ok";
}
```

**@RequestBody ��ü �Ķ����**
- `@RequestBody HelloData data`
- `@RequestBody`�� ���� ���� ��ü�� ������ �� �ִ�.

`HttpEntity`, `@RequestBody`�� ����ϸ� HTTP �޽����� �����Ͱ� HTTP �޽��� �ٵ��� ������ �츮�� ���ϴ� ���ڳ� ��ü ������ ��ȯ���ش�.<BR>
HTTP �޽��� �����ʹ� ���� �� �ƴ϶�, JSON ��ü�� ��ȯ���ִµ�, �츮�� ��� V2���� �ߴ� �۾��� ��� ó�����ش�. �ڼ��� ������ �ڿ� HTTP �޽��� �����Ϳ��� �ٷ��.

**@RequestBody�� ���� �Ұ���**<br>
`@ModelAttribute`���� �н��� ���� ���ø���.

�������� `@ModelAttribute`, `@RequestParam` �ش� ���½� ������ ���� ��Ģ ����
- `String`, `int`, `Integer` ���� �ܼ� Ÿ�� = `@RequestParam`
- ������ = `@ModelAttribute`(argument resolver�� �����ص� Ÿ�� ��)

���� �� ��� HelloData�� `@RequestBody`�� �����ϸ� `@ModelAttribute`�� ����Ǿ������.<br>
`HelloData data` -> `@ModelAttribute HelloData data`<br>
���� �����ϸ� HTTP �޽��� �ٵ� �ƴ϶� ��û �Ķ���͸� ó���ϰ� �ȴ�.

**requestBodyJsonV5**<br>
```java
@ResponseBody
@PostMapping("/request-body-json-v5")
public HelloData requestBodyJsonV5(@RequestBody HelloData data){
    log.info("username={}, age={}",data.getUsername(),data.getAge());
    return data;
}
```

`@ResponseBody`<br>
������ ��쿡�� `@ResponseBody`�� ����ϸ� �ش� ��ü�� HTTP �޽��� �ٵ� ���� �־��� �� �ִ�.<BR>
���� �� ��쿡�� `HttpEntity`�� ����ص� �ȴ�.

- `@RequestBody` ��û
  - JSON ��û -> HTTP �޽��� ������ -> ��ü
- `@ResponseBody` ����
  - ��ü -> HTTP �޽��� ������ -> JSON ����

---

### ���� - ���� ���ҽ�, �� ���ø�

������(����)���� ���� �����͸� ����� ����� ũ�� 3����.
- ���� ���ҽ�
  - ex> �� �������� ������ HTML, css, js�� ������ ����, **���� ���ҽ�** ���.
- �� ���ø� ���
  - ex> �� �������� ������ HTML�� ������ ���� �� ���ø��� ���.
- HTTP �޽��� ���
  - HTTP API�� �����ϴ� ��쿡�� HTML�� �ƴ϶� �����͸� �����ؾ� �ϹǷ�, HTTP �޽��� �ٵ� JSON ���� �������� �����͸� �Ǿ� ������.

#### ���� ���ҽ�
������ ��Ʈ�� Ŭ�����н��� ���� ���丮�� �ִ� ���� ���ҽ��� ����.<br>
`/static`, `/public`,`resources`,`/META-INF/resources`

`src/main/resources`�� ���ҽ��� �����ϴ� ���̰�, �� Ŭ�����н��� ���� ����̴�.<br>
���� ���� ���丮�� ���ҽ��� �־�θ� ������ ��Ʈ�� ���� ���ҽ��� ���񽺸� �����Ѵ�.

**���� ���ҽ� ���**<br>
`src/main/resources/static`

���� ��ο� ������ ���������<br>
`src/main/resources/static/basic/hello-form.html`

�� ���������� ������ ���� �����ϸ��.<br>
`http://localhost:8080/basic/hello-form.html`

���� ���ҽ��� �ش� ������ ���� ���� �״�� �����ϴ� ��.

#### �� ���ø�
�� ���ø��� ���ļ� HTML�� �����ǰ�, �䰡 ������ ���� �����Ѵ�.<BR>
�Ϲ������� HTML�� �������� �����ϴ� �뵵�� ���������, �ٸ� �͵鵵 �����ϴ�. �� ���ø��� ���� �� �ִ� ���̶�� ������ �����ϴ�.

������ ��Ʈ�� �⺻ �� ���ø� ��θ� ������.

**�� ���ø� ���**<BR>
`src/main/resources/templates`

**�� ���ø� ����**<br>
`src/main/resources/templates/response/hello.html`

```java
@Controller
public class ResponseViewController {

  @RequestMapping("/response-view-v1")
  public ModelAndView responseViewV1(){
      ModelAndView mav = new ModelAndView("response/hello")
              .addObject("data","hello!");
      return mav;
  }

  @RequestMapping("/response-view-v2")
  public String responseViewV2(Model model){
      model.addAttribute("data","hello!");
      return "response/hello";
  }

  //���� x
  @RequestMapping("/response/hello")
  public void responseViewV3(Model model){
      model.addAttribute("data","hello!");
  }
}
```

**String�� ��ȯ�ϴ� ��� - View or HTTP �޽���**<BR>
`@ResponseBody`�� ������ `response/hello`�� �� �������� ����Ǿ �並 ã��, ������ �Ѵ�.<br>
`@ResponseBody`�� ������ �� �������� �������� �ʰ�, HTTP �޽��� �ٵ� ���� `response/hello`��� ���ڰ� �Էµȴ�.

���⼭ ���� �� �̸��� `response/hello`�� ��ȯ�ϸ� ���� ����� �� �������� ������ �Ǵ� ���� Ȯ���� �� �ִ�.
- ���� : `templates/response/hello.html`

**Void**�� ��ȯ�ϴ� ���(v3)<br>
- `@Controller`�� ����ϰ�, `HttpServletResponse`, `OutputStream(Wrtier)` ���� HTTP �޽��� �ٵ� ó���ϴ� �Ķ���Ͱ� ������ ��û URL�� �����ؼ� �� �� �̸����� ���
  - ��û URL : `/response/hello`
  - ���� : `templates/response/hello`
- **����� �� ����� ��ü��� �ʹ� �������� �̷��� �� �´� ��쵵 ���� ���, �������� �ʴ´�.**

**HTTP �޽���**<BR>
`@ResponseBody`,`HttpEntity`�� ����ϸ�, �� ���ø��� ����ϴ� ���� �ƴ϶�, HTTP �޽��� �ٵ� ���� ���� �����͸� ����� �� �ִ�.

---

### HTTP ���� - HTTP API, �޽��� �ٵ� ���� �Է�

> **����**<BR>
> HTML�̳� �� ���ø��� ����ص� HTTP ���� �޽��� �ٵ� HTML �����Ͱ� ��ܼ� ���޵ȴ�. ���⼭ �����ϴ� ������ ���� ���ҽ��� �� ���ø��� ��ġ�� �ʰ�, ���� HTTP ���� �޽����� �����ϴ� ��츦 ���Ѵ�.

**ResponseBodyController** 
```java
@Slf4j
//@Controller
//ResponseBody
@RestController
public class ResponseBodyController {

    @GetMapping("/response-body-string-v1")
    public void responseBodyV1(HttpServletResponse response) throws IOException {
        response.getWriter().write("ok");
    }

    @GetMapping("/response-body-string-v2")
    public ResponseEntity<String> responseBodyV2(){
        return new ResponseEntity<>("ok", HttpStatus.OK);
    }

    @ResponseBody
    @GetMapping("/response-body-string-v3")
    public String responseBodyV3(){
        return "ok";
    }

    @GetMapping("/response-body-json-v1")
    public ResponseEntity<HelloData> responseBodyJsonV1(){
        HelloData helloData = new HelloData();
        helloData.setUsername("userA");
        helloData.setAge(20);

        return new ResponseEntity<>(helloData, HttpStatus.OK);
    }

    @ResponseStatus(HttpStatus.OK)
    @ResponseBody
    @GetMapping("/response-body-json-v2")
    public HelloData responseBodyJsonV2(){
        HelloData helloData = new HelloData();
        helloData.setUsername("userA");
        helloData.setAge(20);
        return helloData;
    }
    
}
```

**@RestController**
- `@Controller` ��ſ� `@RestController` �ֳ����̼��� ����ϸ�, �ش� ��Ʈ�ѷ��� ��� `@ResponseBody`�� ����Ǵ� ȿ���� �ִ�. ���� �� ���ø��� ����ϴ� ���� �ƴ϶�, HTTP �޽��� �ٵ� ���� �����͸� �Է��Ѵ�. �̸� �״�� Rest API(HTTP API)�� ���� �� ����ϴ� ��Ʈ�ѷ��̴�.

����� `@ResponseBody`�� Ŭ���� ������ �θ� ��ü �޼��忡 ����Ǵµ�, `@RestController` �ֳ����̼� �ȿ� `@ResponseBody`�� ����Ǿ��ִ�.<br>
��, `@RestController` = `@Controller` + `ResponseBody`

