## TIL
## 2022년 12월 19일 (월)
- TIL 시작

## 2022년 12월 20일 (화)
## 마음가짐 
- 서둘지마라.  
- 실패-시도-실패-수정-시도.  
- 기록/수정.  
- 기본기 중요.  
- 즐겁게 하자.  
- 호기심.  
- 꾸준히 평생
## 의식적인 연습 방법
- 약간 어려운 도전과제를 반복 할 것. 
- 시행착오에 좌절하지 말것. 
- 설명 할 수 없으면 모르는 것.
## 부족한 점
- 배경지식, CS 기본상식, 용어 이해
- 문제 해결 능력

## 자바스크립트 Deep Dive Study
- 이응모 블로그 https://poiemaweb.com/
- 100page/1day + Typing Practice(en)

## 2022년 12월 21일 (수)
## 얄팍한 코딩사전의 ( "제대로 파는 JavaScript" YouTube 강의 시청  )
- 섹션 1. 자바스크립트의 기본적인 사용
1. 콘솔 활용하기
2. 주석과 세미콜론
3. 변수와 상수 - 데이터를 담는 주머니

## 2022년 12월 22일 (목)
- 섹션 2. 자료형과 연산자
1. 자료형 - 데이터의 종류
2. 자료형과 정적, 동적 타입
3. 문자열(string) - 텍스트 데이터
4. 문자열에 사용되는 연산자
## 2022년 12월 23일 (금)
5. 숫자(Number)와 관련 연산자
6. 부동 소수점과 실수계산 오차
7. 불리언(boolean)과 관련 연산자
8. 연산자 마무리
9. 객체와 배열 미리보기
10. 원시 타입 VS 참조타입
## 2022년 12월 24일 (토)
- 섹션 3. 제어문
1. 블록문과 스코프
2. if/else
3. switch
4. for 루프
5. while 과 do while
## 2022년 12월 25일 (일)
- 섹션 4. 함수
1. 함수의 의미와 사용법
2. 일급 객체
3. 매개변수
. 함수 더 알아보기
- 섹션 5. 객체와 클래스
1. 객체의 기본 사용법들
2. 생성자 함수
3. 클래스
4. 접근자 프로퍼티와 은닉
5. 상속
6. 객체의 스프레드와 디스트럭쳐링
- 섹션 6. 주요 빌트인 객체
1. 전역 객체와 표준 빌트인 객체
2. 빌트인 전역 프로퍼티와 함수
3. String 객체
4. Number 객체
5. Math 객체
6. Date 객체
- 섹션 7. 배열
1. 자바스크립트 배열의 특징과 생성
2. 배열의 기본 메서드들
3. 고차함수 메서드들
4. 배열의 스프레드와 디스트럭쳐링

## 2022년 12월 26일 (월)
- 백틱 - ` ~ `
⭐️ 문자열 안에 탭과 줄바꿈 그대로 사용 가능!
템플릿 리터럴
👉 MDN 문서 보기
```
const NAME = '홍길동';
let age = 20;
let married = false;

console.log(
`제 이름은 ${NAME}, 나이는 ${age}세구요, \
${married ? '기혼' : '미혼'}입니다.`
);
// 제 이름은 홍길동, 나이는 20세구요, 미혼입니다.
${}안에 상수나 변수, 표현식 등을 삽입 가능
```
다른 자료형도 사용할 수 있음
- 숫자 자료형   
isNaN	: 숫자가 아니다 싶으면 무조건 true 반환   
Number.isNaN	: 숫자 자료형인 주제에 숫자가 아니어야만 true 반환  
- 단항 산술 연산자  
`연산자  	반환  	     부수효과`    
`a++	  값그대로	      1 증가`   
`++a 	 1증가한값    	  1 증가`    
`a--	  값그대로 	      1 감소`  
`--a	  1감소한값	      1 감소`  
`+a	   값 그대로	       없음`  
`-a	  양음을 반전한값	   없음`  
