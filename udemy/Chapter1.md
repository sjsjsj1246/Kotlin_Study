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

## 1.2 실습환경 구축

## 1.3 코틀린 프로젝트 시작하기

- kotlin은 NullPointException을 방지하기 위해서 변수 선언 시 널 가능성에 대해 명시해야 한다.
- 세미콜론이 선택사항이며 public이 디폴트이고 함수 파라미터에 기본설정을 할 수 있는 등 간결함을 채택하고 있다.
- 코틀린 확장을 통해 boilerplate한 코드를 많이 줄일 수 있다.
- Kotlin은 함수형 프로그래밍과 OOP를 지원하며 Java와 호환되기 때문에 JVM상에서 실행할 수 있다.