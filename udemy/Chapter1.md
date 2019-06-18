# Chapter1 : 코틀린 시작하기

## 강의 개요

### Education Environment

- Host PC
    - OS : Windows7 or 8~10 64bit (4GB~Memory) or MAC OS is possble
- Development Environments
    - inteliJ IDEA Conmmunity
    - Android Studio 3.x
    - SOurce Tree (git)
    - Virtual Machine for Android
- Target Board
    - Android bassed machine 또는 Smartphone

### Objects

- 코틀린 프로그래밍 기본 개념
    - 탄생 배경, 언어의 특징, 실습 환경 구축
- 기본 프로그래밍 문법 습득
    - 변수와 타입, 함수, 제어, 배열과 문자열, 파일 입출력
- 코틀린의 추가된 기법과 활용
    - 추가된 클래스 기법, 람다, 코루틴, 널 처리
- 안드로이드에서 코틀린 확장 및 사용
    - 코틀린 확장, Anko 확장
- 간단한 프로젝트를 통한 코틀린 이해

## 1.1 코틀린의 탄생 배경

- 목표
    - 풀스택 웹 개발, Android와 IOS앱, 그리고 임베디드, IOT등 모든 개발을 다양한 플랫폼에서 개발할 수 있도록 하는 것.
- 특징
    - IDE(Android Studio의 모체)로 유멸한 JetBrains에서 개발하고 보급 코드가 간결하고 다재다능하며 호환성이 높다.
    - 문장 끝에 세미콜론은 옵션이다.
    Android Studio에서 안드로이드 공식 언어로 추가
    - 변수는 Nullable(널 값 사용 가능)과 NotNull로 나뉘는 데, 변수 선언시 '?'를 붙여 Nullable로 만들 수 있다.

### 다양한 플랫폼

- 사용 가능한 플랫폼
    - Kotlin/JVM - 자바 가상 머신 상에서 동작하는 앱을 만들 수 있다.
    - Kotlin/JS - 자바스크립트에 의해 브라우저에서 동작하는 앱을 만들 수 있다.
    - Kotlin/Native - LLVM기반의 네이티브 컴파일을 지원해 여러 타깃의 앱을 만들 수 있다.

- Kotlin/Native에서의 타깃
    - IOS (arm32, arm64, emulator x86_64)
    - MacOS (x86_64)
    - Android (arm43, arm64)
    - Windows (mingw x86_64)
    - Linux (x86_64, arm32, MIPS, MIPS little endian)
    - WebAssembly (wasm32)

### 코틀린의 장점

- 자료형에 대한 오류를 미리 잡을 수 있는 정적 언어
- 널 포인터로 인한 프로그램의 중단을 예방할 수 있다.
    - 보통 개발자들은 코틀린의 이런 특징을 NPE에서 자류롭다고 한다
    - NPE는 Null Pointer Exception
- 아주 간결하고 효율적
- 함수형 프로그래밍과 객체 지향 프로그래밍이 모두 가능
- 세미콜론을 생략할 수 있다.

### 안드로이드의 공식 언어

- 자바와 안드로이드 그리고 코틀린
    - 제임스 고슬링 - 자바언어의 제작자
    - 선 마이크로 시스템즈 -> 오라클 이후 자바의 부분 유료 정책 고수

- 자바 언어와 Oracle JDK
    - 자바 언어 자체는 무료지만 SDK인 Oracle JDK는 특정 기능을 위해 라이선스비 지불

- OpenJDK
    - 오픈소스화된 SDK로 Oracle JDK와 거의 동일하나 몇 가지 상용기능이 빠진 형태로 제공한다.

## 1.2 실습환경 구축

### 자바 JDK 설치하기

- JDK 설치는 왜?
    - 코틀린은ㄹ JVM에서 실행하기 위해
    - 기존 자바와 상호작용할 수 있고 자바 라이브러리를 이용할 수 있다.

- Oracle JDK vs Open JDK
    - Oracle JDK : 보안 업데이트를 지속적으로 받으려면 구독 방식으로 라이선스 구매 필요
    - Open JDK : 제한 없이 사용 가능. 단 보안 서비스의 의무가 없어 유지보수 어려움

- Azul의 zulu
    - TCK 인증을 통과한 OpenJDK를 묶어서 배포하는 제 3의 벤더

### JDK 배포판의 선택

    - 원하는 배포판 선택



## 1.3 코틀린 프로젝트 시작하기

- kotlin은 NullPointException을 방지하기 위해서 변수 선언 시 널 가능성에 대해 명시해야 한다.
- 세미콜론이 선택사항이며 public이 디폴트이고 함수 파라미터에 기본설정을 할 수 있는 등 간결함을 채택하고 있다.
- 코틀린 확장을 통해 boilerplate한 코드를 많이 줄일 수 있다.
- Kotlin은 함수형 프로그래밍과 OOP를 지원하며 Java와 호환되기 때문에 JVM상에서 실행할 수 있다.