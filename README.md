# JS-scientific-calculator

JavaScript를 이용해 구현한 간단한 공학용 계산기

2021년 12월 17일 작업 내용 :  
- 모든 함수 기능 구현  
- 버튼에서 쓰일 모든 함수의 기능들을 모두 구현  
- eval() 함수를 사용해 문자열 수식을 만든 뒤 JavaScript의 기본 연산과 Math 내장 객체를 이용해 수식 연산  
- +추가
- eval() 함수를 대신해 함수를 생성하고 수식 문자열을 return하도록 해, eval()함수 제거

2021년 12월 20일 작업 내용 :
- 정규표현식을 이용해 수식을 수정하는 기능의 함수 분리
- 버블링을 이용해 event handler 간소화
- exp() 함수명 변경 및 정규식 수정을 통해 자연상수와 exp() 구분
- 닫히지 않은 괄호 자동 처리 기능 추가
- 기능별 함수 분리
- html 코드 간소화 -> 태그의 value속성 제거 후 javascript를 통해 속성 추가 및 제어


## 오류 및 수정해야 할 내용
1. 자연상수 e와 exp()함수의 e를 구분하지 못해 오류 발생 -> exp()함수명을 변경하거나 정규표현식 수정 필요
2. 괄호가 닫히지 않은 함수의 연산이 자동으로 실행되지 않음 -> 문자열 순회 후 소괄호가 열린 뒤 닫히지 않은 함수 발견시 자동으로 닫는 기능 추가 예정
3. 수식이 표출될 때 제곱을 표현하는 방식이 아직 x^y와 같은 상황 -> innerHtml을 이용해 <sup>태그 추가 예정
4. 키보드를 이용한 버튼 제어 기능 추가 예정