# InnoRules User's Guide of Rule Builder

## 제 1장. 룰 문법

이 장에서는 InnoRules 룰 문법을 구성하는 기본 사항과, 룰 내용 작성에 필요한 룰 표현식 기술 문법에 대해 설명한다.

- 룰을 구성하는 룰 식별자, 룰 템플릿, 룰 버전, 룰 리턴, 룰 표현식 등
- 룰 표현식의 구성 요소
- 룰 표현식의 구성 요소와 룰 표현식의 실행 결과가 가지는 데이터 타입과 데이터 형식
- 룰과 룰 표현식의 작성 규칙

## 1. 기본 사항

업무 분석을 통해 도출된 하나의 비즈니스 룰은, 문법 규칙이나 재활용, 성능, 유지보수 효율성 등을 고려하여, InnoRules 룰 시스템(이하 InnoRules 또는 룰 시스템)에서의 최소 정의 단위인 룰로 분해되고, 이들 룰 간 일련의 호출 및 결과 참조, 연산 등을 통해 구현된다.

![image](https://github.com/syheo10/syheo10.github.io/blob/develop/images/image1.png?raw=true)

![그림 1 . 룰 호출 및 결과 참조 관계도](https://github.com/rundocs/jekyll-rtd-theme/workflows/CI/badge.svg?branch=develop)


기본적으로 하나의 룰은, 하나 이상의 (룰) 버전을 가지며 룰과 버전 각각에 대한 정보(정의 사항)와 룰 내용 기술을 통해 구현된다.

|구분           | 주요 구성/정의 사항        |
| ------------- | -------------------- |
| `룰 정보`      | 룰 식별자, 룰 템플릿 유형, 부가 정보 등 룰 관련 정의 사항 |
| `룰 정보`      | 리턴 정보(리턴 형식, 리턴 항목, 리턴 항목의 데이터 타입   |
| `버전 정보`    | 버전 일자, 실행 모드 등 버전 관련 정의 사항              |
| `룰 내용`      | 룰 템플릿에 기술한 룰 표현식들                          |

                 [표1. 룰의 구성]
