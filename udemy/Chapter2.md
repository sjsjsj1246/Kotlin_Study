# Chpater2 : 변수와 자료형, 연산자

## 2.1 코틀린 패키지

### 프로젝트와 모듈, 패키지, 파일의 관계

- 프로젝트와 패키지(자바와 비슷)  
![](img/프로젝트와패키지.png)
프로젝트 내부에는 여러 모듈이 있음, 모듈 내부는 여러 패키지가 있음, 패키지 내부에는 kt파일이 있음, kt파일에는 여러 class가 있음  
패키지명을 정하지 않으면 default 패키지 생성  
(패키지 이름을 그림과 같이 주소를 거꾸로 하는 형태로 짓는 이유는 다른 회사와 충돌하지 않게 하기 위해서)  

- 패키지 정의
    - 자바 프로젝트 처럼 디렉터리와 매치되어야 하지는 않는다.
    ```kotlin
    package con.example.edu
    class Person(val name: String, val age: Int)
    ```
    - 패키지를 지정하지 않으면 이름이 없는 기본(default) 패키지에 속한다.
    - import의 이름이 충돌하면 as 키워드로 로컬에서 사용할 이름을 변경해서 충돌을 피할 수 있다.
    ```kotlin
    import con.example.edu.Person
    import con,example.edu.Person as User // com.example.edu.Person을 User로 지정
    ```
    - import는 클래스 뿐만 아니라 다른 것도 임포트 할 수 있다.
        - 최상위 레벨 함수와 프로퍼티, 오브젝트 선언의 함수와 프로퍼티, 열거형 상수

(파일에 클래스가 하나 있고 그거스이 일므이 파일과 같다면 확장자가 생략됨)

- 기본 패키지(코틀린 표준 라이브러리)
    - kotlin-stdlib-source.jar  
    ![](img/코틀린표준라이브러리.png)

## 2.2 변수와 자료형

## 2.3 자료형 검사와 변환

## 2.4 코틀린 연산자