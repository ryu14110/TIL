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
```
연산자     반환  	      부수효과    
a++	   값그대로	        1 증가   
++a 	 1증가한값           1 증가    
a--	   값그대로 	       1 감소  
--a	   1감소한값	       1 감소  
+a	   값 그대로	       없음  
-a	  양음을 반전한값	   없음  
```
- 연산자
```
1. Truthy
console.log(
  1.23 ? true : false,
  -999 ? true: false,
  '0' ? true : false,
  ' ' ? true : false,
  Infinity ? true : false,
  -Infinity ? true : false,
  {} ? true : false,
  [] ? true : false,
);
//true true true true true true true true

2. Falsy
console.log(
  0 ? true : false,
  -0 ? true : false,
  '' ? true : false,
  null ? true : false,
  undefined ? true : false,
  NaN ? true : false,
);
//false false false false false false
```
## 2022년 12월 28일 (수)
- Math 객체
```
// 0 반환
console.log(
  Math.abs(0),
  Math.abs(''),
  Math.abs(null),
  Math.abs([]),
);
//0 0 0 0
// NaN 반환
console.log(
  Math.abs('abc'),
  Math.abs(undefined),
  Math.abs({a: 1}),
  Math.abs([1, 2, 3]),
  Math.abs()
);
//NaN NaN NaN NaN NaN
```
- 배열의 기본 메서드
- Join
```
const arr1 = ['a', 'b', 'c', 'd', 'e'];
const arr2 = [
  1, true, null, undefined, '가나다', { x: 0 }, [1, 2, 3]
];
console.log(
  arr1.join() // 인자가 없다면 쉼표`,`로
);
//a,b,c,d,e
console.log(
  arr1.join('')
);
//abcde
console.log(
  arr1.join(' ')
);
//a b c d e
console.log(
  arr2.join(':')
);
//1:true:::가나다:[object Object]:1,2,3
```
- splice
```
const arr = [1, 2, 3, 4, 5, 6, 7];

// 2번 인덱스부터 2개 요소 제거
arr.splice(2, 2);

console.log(arr);
// [1, 2, 5, 6, 7]

// 3번 인덱스부터 요소 제거 없이 'a' 추가
arr.splice(3, 0, 'a');

console.log(arr);
//[1, 2, 5, 'a', 6, 7]
// 1번 인덱스부터 3개 요소 제거 후 '가', '나', '다' 추가
arr.splice(1, 3, '가', '나', '다');

console.log(arr);
//[1, '가', '나', '다', 6, 7]
```
- fill
 ```
// 중간의 빈 값도 채움
const arr1 = [1, 2, , , 4, 5];
arr1.fill(7);

console.log('1.', arr1);
//1. (6) [7, 7, 7, 7, 7, 7]

// 💡 특정 값으로 채운 배열 생성시 유용
const arr2 = new Array(10);
arr2.fill(1);

console.log('2.', arr2);
//2. (10) [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]

// 인자가 둘일 때: (채울 값, ~부터)
arr2.fill(2, 3);

console.log('3.', arr2);
//3. (10) [1, 1, 1, 2, 2, 2, 2, 2, 2, 2]

// 인자가 셋일 때: (채울 값, ~부터, ~ 전까지)
arr2.fill(3, 6, 9);

console.log('4.', arr2);
//4. (10) [1, 1, 1, 2, 2, 2, 3, 3, 3, 2]
```
## 2023년 1월 1일
정수 배열 array가 매개변수로 주어질 때, 최빈값을 return 하도록 solution 함수를 완성해보세요
```
function solution(array) {
                           // array의 길이가 1일 경우 갯수가 하나이기에
                           // 그 값을 반환해준다.
  if (array.length === 1) return array[0];

  const obj = {};
  const answer = [];

                           // array를 forEach() 반복문을 돌려
                           // obj에 값이 없으면 값을 만들고 1을 넣어주고
                           // obj에 값이 있으면 기존 값 +1을 해준다.
  array.forEach((n) => {
    obj[n] = ++obj[n] || 1;
  });

                            // 값과 그 값의 갯수를 정의해 둔 obj를 array에 넣어준다.
                            // ex) [[1, 1], [2, 1], [3, 3], [4, 1]]
  for (let key in obj) {
    answer.push([key, obj[key]]);
  }

                                   // answer 배열을 갯수 기준으로 내림차순 정렬을 해준다.
                                   // ex) [[3, 3], [4, 1], [2, 1], [1, 1]]
  answer.sort((a, b) => b[1] - a[1]);

                                     // 최빈값이 여러 개면 -1을 반환해야 하기 때문에 확인한다.
  if (answer[0][1] === answer[1][1]) return -1;

                                      // 여러개가 아니라면 정렬한 처음 값을 반환한다.
  return Number(answer[0][0]);
}

console.log(solution([1, 2, 3, 3, 3, 4]));
```
### I studied for **6** hours today.(Coding Test Practice all) 
## 2023년 1월 2일
- 코딩 테스트 연습, 입문과정 풀기 
  "입문 과정 (10/100)"
### I studied for **5** hours today. (Coding Test Practice all)
## 2023년 1월 3일
- 코딩 테스트 연습, 입문 풀기 
  "입문 과정 (20/100)"
### I studied for **7** hours today. (Coding Test 5h, Html 2h)
## 2023년 1월 7일
- 코딩 테스트 연습, 입문과정 풀기 (30/100)
## 2023년 1월 8일
- Hello, JavaScript: 자바스크립트 입문 강의(무료) <김용록> 수강
## 2023년 1월 9일
- 코딩테스트 광탈방지 Ato Z 강의(10만원) <이선협> 수강중
## 2023년 1월 11일
- 코딩테스트 입문 문제풀이 
## 2023년 1월 12일
- Do it! HTML + CSS + 자바스크립트 웹 표준정석(이지스퍼블리싱) 수강중
## 2023년 1월 13일
- 코딩테스트 입문 문제 (2시간)
- 이지스퍼블리싱 수강
## 2023년 1월 15일
- 디지털 시계 만들기(바닐라 자바스트립트)
## 2023년 1월 19일
- 연습게임 만들기 : Flying Saucer
## 2023년 1월 25일
- 프로젝트 만들기 : Register Validator
## 2023년 1월 27일
- 프로젝트 만들기 : Expanding Cards
## 2023년 1월 28일
- 프로젝트 만들기 : Movie Seat Booking
## 2023년 1월 29일
- 프로젝트 만들기 : Progress Step
## 2023년 1월 30일
- 프로젝트 만들기 : Rotating Navigation
## 2023년 1월 31일
- 프로젝트 만들기 : Hidden Search
## 2023년 2월 1일
- 프로젝트 만들기 : Blurry Loading
## 2023년 2월 2일
- 프로젝트 만들기 : Split Landing Page, ScrollAnimation
## 2023년 2월 4일
- 프로젝트 만들기 : Dad Joker
## 2023년 2월 5일
- 프로젝트 만들기 : Event Key Codes
## 2023년 2월 6일
- 프로젝트 만들기 : Animation Navigation, Increment Counter
## 2023년 2월 7일
- 프로젝트 만들기 : Button Ripple Effect, Theme Clock
## 2023년 2월 8일
- 프로젝트 만들기 : Drag N Drop, Drawing App
## 2023년 2월 9일(목요일)
- 프로젝트 만들기 : Kinetic CSS Loader, Sticky Navbar
## 2023년 2월 10일(금요일)
- 프로젝트 만들기 : Double Vertical Slider, Toast Notification
## 2023년 2월 11일(토요일)
- 프로젝트 만들기 : Double Heart Click. Auto Text Effect
## 2023년 2월 12일(일요일)
- 프로젝트 만들기 : Password Generator
## 2023년 2월 13일(월요일)
- 프로젝트 만들기 : Good Cheap Fast Checkboxes
## 2023년 2월 14일(화요일)
- 프로젝트 만들기 : Image Carousel,Animated Countdown
## 2023년 2월 15일(수요일)
- 프로젝트 만들기 : Hover board, Pokedex
## 2023년 2월 16일(목요일)
- 프로젝트 만들기 : Mobile Tab Navigation,Password Strength Background
## 2023년 2월 17일(금요일)
- 프로젝트 만들기 : 3D Background Boxes, Verify Account UI
## 2023년 2월 18일(토요일)
- 프로젝트 만들기 : Live User Filter, Feedback UI Design
## 2023년 2월 19일(일요일)
- 프로젝트 만들기 : Custom Range Slider, Netflix Nabigation
## 2023년 2월 20일(월요일)
- 프로젝트 만들기 : Quiz App, Testimonial Box Switcher
## 2023년 2월 21일(화요일)
- 프로젝트 만들기 : Form Validato
## 2023년 2월 22일(수요일)
- 프로젝트 만들기 : Movie Seat Booking
## 2023년 2월 23일(목요일)
- 프로젝트 만들기 : Custom Video Player
## 2023년 2월 24일(금요일)
- 프로젝트 만들기 : Dom Array Methods
## 2023년 2월 25일(토요일)
- 프로젝트 만들기 : Modal Menu Slider
## 2023년 2월 26일(일요일)
- 프로젝트 만들기 : Hangman Game
## 2023년 2월 27일(월요일)
- nico 프로젝트 만들기 : Random Number Game
## 2023년 3월 2일(목요일)
- nico 프로젝트 만들기 : Time Until Chrismas Eve
## 2023년 3월 3일(금요일)
- nico 프로젝트 만들기 : GradientButton
## 2023년 3월 4일(토요일)
- nico 프로젝트 만들기 : ToDoListSite
## 2023년 3월 5일(일요일)
- 코누 프로젝트 만들기 : Google 검색창 만들기
## 2023년 3월 8일(수요일)
- 프로젝트 만들기 : Spotify 만들기
## 2023년 3월 9일(목요일)
- 프로젝트 만들기 : Number Guess Game
