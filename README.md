# Javascript0920
소스명 : exercise8.html
다음에서 제시된 기능들을 자바스크립트로 구현하시오.

(1) 다음 사양의 함수를 2개 구현한다.

   printH1(content) : content에 전달된 내용을 <h1> 태그와 함께 도큐먼트 영역에 출력한다.
   printH4(content) : content에 전달된 내용을 <h4> 태그와 함께 도큐먼트 영역에 출력한다.

(2) 다음 기능을 처리하는 함수 apply() 를 구현한다.

   - 매개변수 2개
   - 첫 번째 아규먼트로 배열을 두 번째 아규먼트로 함수를 전달받는다.
     아규먼트로는 순서대로 배열과 함수를 전달 받아야 한다.
     아규먼트가 전달되지 않거나 다른 종류의 아규먼트 종류가 전달되면 브라우저에서 제공하는 자바스크립트 콘솔 창에
     "아규먼트 오류"라고 출력하고 false 를 리턴한다.
   - 첫 번째 매개변수에 전달된 배열의 원소값들을 두 번째 매개변수에 전달된 함수를 호출하여 

	도큐먼트 영역에 출력하고(배열의 원소 갯수만큼 호출한다.) true를 리턴한다.

(3) 전역 코드 영역

   - 비어있는 배열을 하나 만든다.
   - window.prompt()를 사용하여 데이터를(숫자, 문자열 관계없다) 입력받고 
     입력된 데이터를 배열에 저장한다. 이 작업은 취소 버튼이 클릭 될 때까지 계속 진행한다.
   - 입력이 끝나면  1~10 사이의 랜덤값을 추출하여
     1, 4, 6 이면  생성된 배열과 printH1을 
     아규먼트로 전달하면서 apply()를 호출한다.

     3, 5, 7 이면 생성된 배열과 printH4를 아규먼트로 전달하면서 apply()를 호출한다.

     8, 9 이면  "ㅋㅋ"라는 문자열과 printH1을 아규먼트로 전달하면서 apply()를 호출한다.

     그 외의 모든 값이면 이면 생성된 배열만 아규먼트로 전달하면서 apply()를 호출한다.

     이 때 추출되는 난수는 자바스크립트 콘솔창에 출력한다.

   - apply()의 호출 후에 리턴되는 값이 true 이면 "처리 성공" 이라는 메시지를 window.alert() 로 출력한다.
     리턴되는 값이 false 이면 "처리 실패" 라는 메시지를 window.alert() 로  출력한다.

소스명 : exercise9.html
다음에서 제시된 기능들을 자바스크립트로 구현하시오.

(1) 구현 함수

     printObject(p)
   
     - 매개변수에 객체타입이 왔는지 채크하고 Object 타입이 아니면 그냥 리턴한다.
     - 아규먼트로 전달된 객체에서 tag 속성값, color 속성값 그리고 
       msg 속성값을 추출하여 추출된 태그와 칼라 그리고 메시지를
       적용하여 도큐먼트 영역에 출력한다.

(2) 전역 코드 영역
     - printObject(p) 함수를 다섯번 호출하는 기능을 구현한다.
     - 호출할 때마다 다른 내용의 객체를 생성해서 전달한다.
     - 객체 생성시에는 객체 리터럴 방식으로 하며
        tag 속성 ---> HTML 태그명 저장
        color 속성  ---> 칼라값 저장(칼라명 또는 # 시작하는 rgb 값)
        msg 속성  ---> 출력 메시지 저장
        으로 구성되는 자바스크립트 객체를 생성하며 각 속성들의 값은 임의로 정한다.


소스명 : exercise10.html
다음에서 제시된 기능들을 자바스크립트로 구현하시오.

생성자 함수 이름 : DayInfo

(1) 객체 생성시 이름, 년, 월, 일을 아규먼트로 받는다. 
(2) 이름, 년, 월, 일을 객체의 속성이 되게 초기화 한다.
(3) 다음에 제시된 기능을 지원하는 getTotalDates(), getKorDay() 메서드를 생성하여 
     DayInfo 라는 생성자 함수의 prototype 영역에 저장한다.

     getTotalDates() : "XX님은 태어난지 XXX일 되었어요."를 리턴
     getKorDay() :  "XX님은 X요일에 태어났어요."를 리턴

(4) DayInfo 객체를 3개 정도 생성하여 변수에 담고 각각의 getTotalDates(), getKorDay() 메서드의 	
     호출결과를 <h3> 태그와 함께 각각의 칼라로 도큐먼트 영역에 출력한다.


소스명 : exercise11.html
다음에서 제시된 기능들을 자바스크립트로 구현하시오.

1부터 3까지의 랜덤값을 추출하여 
   	1이면 다음으로
  	2이면 네이버로
  	3이면 구글로 이동하는 기능을 구현해 본다.

  단, 무조건 이동하는 것이 아니며 사용자에게 확인 받는 서브 윈도우를 출력하여 
  확인 버튼을 클릭하면 이동하고 취소 버튼이 클릭되면 first.html로  이동한다.

소스명 : exercise12_1.html, exercise12_2.html, exercise12_3.html
다음에서 제시된 기능들을 자바스크립트로 구현하시오.
(1) HTML 파일은 제공된 것을 사용한다.
(2) 페이지 랜더링시 <h2> 태그의 컨텐트로 “오늘은 xx월 xx일입니다” 를 출력한다.
(3) 각 버튼이 클릭되면 출력되는 날짜 메시지를 버튼의 칼라로 변경하는 이벤트 핸들러를
 구현하는데 파일에 따라서 이벤트 모델을 다르게 적용한다.
 exercise12_1.html – 인라인 이벤트 모델
exercise12_2.html – 고전 이벤트 모델
exercise12_3.html – 표준 이벤트 모델
오늘은 xx월 xx일입니다
각각의 파일마다
이벤트 모델-인라인
이벤트 모델-고전
이벤트 모델-표준
으로 제목 정의

소스명 : exercise13.html
다음에서 제시된 기능들을 자바스크립트로 구현하시오.
(1) 다음과 같이 구구단이라는 제목과 버튼 9를 출력한다.(별은 출력하는 것 아님)
 칼라, 웹 폰트 등 스타일은 임의로 정한다.
(2) 버튼 클릭시 해당 버튼의 구구단을 별 위치에 세로로 출력한다.
(3) 구구단이라는 제목을 클릭하면 다음 사이트로 이동하게 자바스크립트로 구현한다.
https://ko.wikipedia.org/wiki/구구단
(4) 구현 시 사용하는 이벤트 모델의 종류는 임의로 정한다.
