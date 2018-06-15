# JSP 학습 저장소

## JSP(Java Server Page)
  - HTML 파일 내에 Java언어를 삽인한 문서
  - 동적 웹 어플리케이션 컴포넌트
  - .jsp 확장자
  - 클라이언트의 요청에 동적으로 작동하고, 응답은 html을 이용
  - jsp는 servlet으로 변환되어 실행
  - hello.jsp는 실행될 때 hello_jsp.java로 변환되고, hello_jsp.class로 컴파일된다.
    - 경로는 톰캣 - work - catalina - localhost - 프로젝트명 폴더
## Servlet(Server Applet)
  - Java 언어로 이루어진 웹 프로그래밍 문서
  - 동적 웹 어플리케이션 컴포넌트
  - .java 확장자
  - 클라이언트의 요청에 동적으로 동작하고, 응답은 html을 이용
## Context Path
  - WAS에서 웹어플리케이션을 구분하기 위한 path
  - 이클립스에서 프로젝트를 생성하면, 자동으로 servlet.xml에 추가된다.
## Servlet 작동 순서
  - 클라이언트에서 servlet 요청이 들어오면, 서버에서는 servlet 컨테이너를 만들고 요청이 있을 때마다 쓰레드가 생성된다.
  - 클라이언트 요청 -> 웹서버 -> WAS -> Servlet Container(쓰레드 생성, 서블릿객체 생성)
  - Servlet은 요청이 들어오면 JVM 안에서 쓰레드를 생성하므로 다른 CGI 언어들과 다르게 서버 부하가 적게 발생. (다른 CGI는 요청 있을때마다 객체 생성)
