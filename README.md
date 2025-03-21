# 🦅 [코드 채점용] Swift Grammar Master CLI

**SwiftGrammerMaster_CLI**는 Swift의 심화 개념을 학습하고 CLI 환경에서 문제를 해결하는 프로젝트입니다.  

<br>

## 📖 프로젝트 개요
- **주제:** Swift 심화 문법 학습 및 CLI 기반 실습 프로젝트
- **학습 개념:** 객체지향 프로그래밍(OOP), 프로토콜, 에러 처리, 제네릭, 클로저
- **실행 환경:** MacOS 

<br>

## 🚀 실행 
### 1. 프로젝트 클론
```sh
$ git clone https://github.com/amazingDove367/SpartaCamp-iOS.git
$ cd SpartaCamp-iOS/[Week2] SwiftGrammerMaster_CLI
```

### 2. 실행하기
```sh
$ swift main.swift
```

<br>

## 📂 폴더 구조
```
[Week2] SwiftGrammerMaster_CLI
│── Problems
│   ├── Problem1.swift            # 문제 1
│   ├── Problem2.swift            # 문제 2
│   ├── Problem3.swift            # 문제 3
│   ├── AdvancedProblem
│   │   ├── Car.swift                 # 기본 자동차 클래스
│   │   ├── ElectricCar.swift         # 전기차 클래스 (Car 상속)
│   │   ├── HybridCar.swift           # 하이브리드 자동차 클래스 (Car 상속)
│   │   ├── Models
│   │   │   ├── CarError.swift        # 자동차 관련 에러 처리
│   │   │   ├── Engine.swift          # 엔진 모델
│── IOHelper.swift                    # 입출력 도우미 함수
│── main.swift                        # 실행 파일 (프로그램 시작점)
│── README.md
```
📌 **폴더 및 파일 설명**
- `Problems/` → **기본 문제 풀이 코드 (`Problem1`, `Problem2`, `Problem3`)**
- `AdvancedProblem/Models/` → **자동차 관련 클래스 및 모델 정의**
- `IOHelper.swift` → **CLI에서 입출력 처리**
- `main.swift` → **프로그램 실행 진입점**



<br>

## 🛠 트러블슈팅 (Troubleshooting)
### 1.제네릭의 잘못된 사용
- **원인**:
  1. 제네릭 함수를 사용하는 컨셉 자체를 잘못 이해함
  2. 명시적 매개변수를 넣어주지 않고, 프롬프트 입력을 받아 Any 타입으로 넘어가면서 컴파일 오류
    
- **상태**: **제네릭 함수 사용 컨벤션  재숙지후 리팩토링 완료**
- **해결 방법**:
  1. 제네릭 타입의 매개변수를 readLine() 으로 받지않고, 명시적인 매개변수를 넣어줬음
  2. 제네릭 함수 매개변수 타입을 String → 제네릭 타입으로 변경


### 2. type(of: ), is 잘못된 사용
- **원인**: type(of: ) 와 is 의 쓰임과 사용방법을 정확히 알지 못해, 혼용하여 사용
- **상태**: **type(of: ), is 개념 재숙지후 리팩토링 완료**
- **해결 방법**: 문제 해결 목적에 맞는, 프로토콜 준수 확인용 is 키워드만 사용

<br>

## vlog 회고 / 자세한 트러블 슈팅
https://hortenssiaa.tistory.com/88
