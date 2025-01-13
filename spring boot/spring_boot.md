## 스프링 부트란 ?

-   **제품 수준 이상의 스프링 기반의 애플리케이션을 만들 때 빠르고 쉽게 만들 수 있게 하는 것**

-   사용자가 일일히 모든 설정을 직접 하지 않도록 많이 쓰이는 설정을 제공
    -   필요시 설정을 바꿀 수 있음
-   code generation이 없고 XML이 사용하지 않음

<br/>

### 의존성 관리

-   스프링 부트가 관리해주는 의존성은 pom.xml에서 version을 명시하지 않아도 스프링 부트가 자동으로 설정
    -   pom.xml에 version 없이 dependency만 추가해주면 알아서 version을 관리
-   스프링 부트가 관리해주는 의존성이 아닌 의존성을 사용하고 싶다면 dependency에 version과 함께 정의 해주면 됌
-   스프링 부트가 관리해주는 의존성의 버전을 임의로 바꾸고 싶다면, pom.xml에 안에 의존성의 버전을 명시

<br/>

### 자동 설정

**메인 클래스에 있는 @SpringBootApplication은 크게 3가지가 합쳐진 것**

1. @SpringBootConfiguration
2. @ComponentScan
3. @EnableAutoConfiguration

-   스프링부트 어플리케이션은 Bean을 2번 등록
-   @ComponentScan으로 등록 후, EnableAutoConfiguration으로 추가적인 Bean을 읽어 등록

> **스프링 빈(Bean)이란 ?**

-   빈(Bean)은 스프링 컨테이너에 의해 관리되는 **재사용 가능한 소프트웨어 컴포넌트**
    -   스프링 컨테이너가 관리하는 자바 객체
    -   하나 이상의 Bean을 관리

> 왜 사용하는가 ?

-   스프링 간의 객체가 의존 관계를 관리하도록 하는 것
-   객체가 의존관계를 등록할 때, 스프링 컨테이너에서 해당하는 빈을 찾고, 그 빈의 의존성을 만듬
