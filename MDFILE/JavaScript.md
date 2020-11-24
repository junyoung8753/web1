JavaScript

2.수업의 목적

3.HTML과 JS의 만남 : script 태그
4.HTML과 JS의 만남 : 이벤트
5.HTML과 JS의 만남 (콘솔)

6.데이터타입 - 문자열과 숫자

7.변수와 대입 연산자

8.웹브라우저 제어

9.CSS 기초 : style 속성
10.CSS 기초 : style 태그
11.CSS 기초 : 선택자

12.제어할 태그 선택하기

13.프로그램,프로그래밍,프로그래머

14.조건문 예고 15.비교 연산자와 블리언 16.조건문 17.조건문의 활용

18.리팩토링 중복의 제거

19.반복문 예고 20.배열 21.반복문 22.배열과 반복문 23.배열과 반복문의 활용

24.함수예고 25.함수 26.함수 : 매개변수와 인자 27.함수 (리턴) 28.함수의 활용

29.객체 예고 30.객체 쓰기와 읽기 31.객체와 반복문 32.객체프로퍼티와 메소드 33.객체의 활용

34.파일로 쪼개서 정리 정돈하기 35.라이브러리와 프레임워크
36.UI vs API 37.수업을 마치며

# WEB2 JavaScript - 1.수업소개

# WEB2 JavaScript - 2.수업의 목적

- JavaScript 란

* 자바스크립트는 사용자와 상호작용하는 언어이다.
* html을 제어하는 언어다.
* web을 다이나믹하게 만들어주는 역할을 한다.

# WEB2 JavaScript - 3.HTML과 JS의 만남 : script 태그

<body></body> 사이에 넣으며

<script>
document.write(1 + 1);
</script>

와 같이 사용한다/

# WEB2 JavaScript - 4.HTML과 JS의 만남 : 이벤트

JavaScript는 웹에서 사용자와 상호작용하는 기능을 만드는것.
사건(event)을 통해 사용자와 상호작용 가능한 웹을 만들 수 있다..

- 이벤트 속성(attribute)

onclick : 버튼 이벤트
onchange : 텍스트내용 바뀌었을 때 이벤트
onkeydown : 텍스트에서 키를 눌렀을 때
alert('내용') : 경고창

자주 사용하는 event에는 10~20개 정도가 있는데 on click/onchange/onkeydown 등이 있다.

자바스크립트 이벤트 기본 형태 :
<input="button/text" onchange/onclick/onkeydown="alert('아무말')">

# WEB2 JavaScript - 5.HTML과 JS의 만남 (콘솔)

console은 꼭 파일을 통째로 실행시키는 경우가 아닐 때 자주 사용한다.

작업하는 중간마다 결과를 확인하는 데도 유용하다. 코드를 한 번에 쳐서 완성하는 사람은 없으니까.

1. <script> 태그를 이용하거나
2. 특정사건 event 에 대해서 on~ attribute를 추가해서 실행시키거나,
3. 웹페이지-검사에서 웹페이지의 콘솔 JavaScript를 사용하여 간단히 원하는 문제를 해결할 수 있다.

# WEB2 JavaScript - 6.데이터타입 - 문자열과 숫자

데이터 처리하기위해 데이터를 분류하는 일이 필요하고 중요해서 문자와 숫자 문자열을 나누고,
JavaScript 프로퍼티를 이용하여 다양한 편의성기능을 사용한다.

- data type (데이터 타입)

* 숫자number(1,2,3...)
* 문자(a,b,c...#,\$...)
* 문자열string(hello,ohmygod,...)
* 불리언(boolean)

- javascript string(문자열) 프로퍼티

* string.toUpperCase() 대문자로 바꿔줌
* string.indexOf('A') 몇번째에 찾는 문자(A)가 있는지 알려줌
* string.trim() 공백 없애줌
* string.length 문자수 (str.XXX는 string.xxx. 즉 문자열이란뜻)

"1" 은 문자, 1 은 숫자. 즉 "" '' 는 문자로 만들어준다.
1+1 은 2, "1"+"1" 은 11이다
그러나, html 에서는 타이핑한 문자가 그대로 나온다.

# WEB2 JavaScript - 7.변수와 대입 연산자

- 상수(constant): 항상"상" 인 수. 바뀌지 않는것 (ex: 1=1)
- 변수(variable): 변할수 있는 수. 바뀔수 있는것 (ex: var name = 'junyoung')

backgroundColor='black';
backgroundColor(변수) =(대입연산자) 'black';(변수의 값)

- 변수(variable)활용 예

var name = 'junyoung'; (shift + Enter 누르면 검사를 유보하고 다음칸으로감)
alert("Web browsers receive "+name+" HTML documents from a web server or from local storage and render the documents into multimedia web page aasdfafs "+name+" fsd sdfa "+name+"8753 HTMLdescribes the structure of a web page semantically and o "+name+" riginally included cues for the appearance of the document.")

var name = 'junyoung'; 를 사용하면 "+name+" 에 junyoung을 쉽게 넣을수 있다.

# WEB2 JavaScript - 8.웹브라우저 제어

<body style="background-color:black;color:white;">는 "HTML"의 body에 "CSS" style태그를 넣어 사용한것이다.
HTML은 한번 수정하면 바뀌지 않는 정적인 언어이고 CSS는 디자인의 역활을한다.
이제 JavaScript를 사용하여 내 행동에 따라 반응하게 만들 수 있는 방법중 하나인 웹브라우저 제어에 대하여 배운다.

# WEB2 JavaScript - 9. CSS 기초 : style 속성

CSS 복습.

<h2 style="background-color:coral;color:powderblue">JavaScript</h2>

html에 CSS의 style태그라는 문법을 적용.
color, background-color은 CSS의 속성(property)

# WEB2 JavaScript - 10.CSS 기초 (style 태그)

<style></style>는 태그 사이에 들어있는 것이 CSS라는것을 알려주는 구분자.

div(<>) > class(.) > id(#)  
div가 제일 포괄적. 동시에 class와 id가 같이 쓰였을때 id가 더 구체적이기에 우선적용됨.

<style>
    div {
    }
    .apple{
    }
    #banana{
    }
</style>
<body>
<div class="apple" id="banana">hello</div>
</body>

# WEB2 JavaScript - 11.CSS 기초 : 선택자

div(<>) class(.) id(#) 는 선택자.
div가 먼저 적용되고 class를 적용한후 id를 적용한다. 즉 id가 마지막에 적용됨으로
동시에 사용되었을때 id의 속성값이 적용된다.

# WEB2 JavaScript - 12.제어할 태그 선택하기

<input type="button" value="night" onclick="
document.querySelector('body').style.backgroundColor = 'black';
document.querySelector('body').style.color = 'white';
">
<input type="button" value="day" onclick="
document.querySelector('body').style.backgroundColor = 'white';
document.querySelector('body').style.color = 'black';
">

구글검색 Javascript select tag by css selector

---- 이해 다 안됨. 일단 넘어감------

# WEB2 JavaScript - 13.프로그램,프로그래밍,프로그래머

PROGRAM 은 순서라는 의미가 들어있다
순서를 만드는것을 PROGRAMMING 이라하고
순서를 만드는 사람을 PROGRAMMER 라고 한다.

순서에 '패턴'이 발생한다면 굳이, 계속, 일일이 반복할 이유가 사라진다. 실증난다.
그래서 프로그램을 짜고 그에 걸맞는 언어를 만들어냈다.

HTML은 웹페이지를 묘사하는 목적의 언어이기에 시간의 순서에 따라 진행되지 않는다.
JavaScript는 시간의 순서에 따라 실행되기에 프로그래밍 언어라 볼수 있다.

# WEB2 JavaScript - 14. 조건문 예고

toggle, if 기능 예고.

# WEB2 JavaScript - 15. 비교 연산자와 블리언

comparison operators & Boolean

비교연산자: === + - x % 등등..
=== 는 true or false를 만들어내고 이것을 boolean이라부르며 비교연산자에 들어간다.
이항연산자
대입연산자

- 데이터타입
  number
  string
  boolean 단 두개의 데이터 타입 true & false
  [ < ] : &lt;
  [ > ] : &gt;

# WEB2 JavaScript - 16.조건문

if()에는 boolean data type인 true or false가 온다.

- IF-true 일때 예제
  <script>
  document.write("1");
  if(true){
  document.write("2");
  } else {
  document.write("3");
  }
  document.write("4");
  </script>

  - 결과: 1 2 4
    if true이면 다음줄 코드가 온다

- IF-false 일때 예제
  <script>
      document.write("1");
      if(false){
        document.write("2");
      } else {
        document.write("3");
      }
      document.write("4");
  </script>
  - 결과: 1 3 4
    if false면 else가 온다

# WEB2 JavaScript - 17.조건문의 활용

<input id="night_day" type="button" value="night" onclick="       //value값은 버튼의 기본 글씨값
if(document.querySelector('#night_day').value === 'night'){      //#night_day값이(버튼글씨) night이면
document.querySelector('body').style.backgroundColor = 'black'; //배경 검은색
document.querySelector('body').style.color = 'white';          //글씨 흰색
document.querySelector('#night_day').value = 'day'            //#night_day값을 day로 해라
} else {                                                     //if가 거짓이면
document.querySelector('body').style.backgroundColor = 'white'; //배경 흰
document.querySelector('body').style.color = 'black';          //글씨 검
document.querySelector('#night_day').value = 'night';         //#night_day값을 night로 해라
}
">

# WEB2 JavaScript - 18.리팩토링 중복의 제거

리펙토링: 공장으로 다시보내 개선한다

<input type="button" value="night" onclick="// this를 사용해서 id태그가 필요없어짐.
var target = document.querySelector('body');//document.querySelector('body')를 target으로 하겟다 선언
if(this.value === 'night'){               //document.querySelector('#night_day')를 this로 대체
target.style.backgroundColor = 'black'; //이하 아래로 전부 중복 전부 제거 
target.style.color = 'white';
this.value = 'day'
} else {
target.style.backgroundColor = 'white';
target.style.color = 'black';
this.value = 'night';
}
">

# WEB2 JavaScript - 19.반복문 예고

예고

# WEB2 JavaScript - 20.배열

Array : 정렬
Syntax : 구문

<script>
      var cowerkers = ["egoing", "leezche"];
</script>
  <h2>get</h2>
    <script>
      document.write(cowerkers[0]);  //0부터 시작. egoing이 맨앞이라 0
      document.write(cowerkers[1]);  //lezche가 두번째라 1
    </script>

  <h2>add</h2>
    <script>
      cowerkers.push('duru');      //밀어넣기
      cowerkers.push('taeho');    // "
    </script>

  <h2>count</h2>
    <script>
        document.write(cowerkers.length);  //갯수세기(4개)
    </script>

    javascript array [add,get,count...] 으로 검색해서 활용.

# WEB2 JavaScript - 21.반복문

예제) false가 될때까지 반복

<ul>
  <script>
    document.write("<li>1</li>");
    var i = 0;   // i= 0 이라고 알려줌
    while (i < 3) {  // i < 3 일때까지
      document.write("<li>2</li>");  //반복
      document.write("<li>3</li>");  //1회 반복마다 1씩 증가된다
      i = i + 1;
    }
    document.write("<li>4</li>");//반복이 끝난후.
  </script>
</ul>
값: 1 2 3 2 3 2 3 4

# WEB2 JavaScript - 22.배열과 반복문

배열: 정보를 담는 그릇이면서 정보를 순서대로 담는 특징이 있다.
객채: 이름이 있는 정리정돈 상자. ex) BodySetColor , NightDayHandler 같은걸 객체라 한다
배열은 대가로[] 객체는 중가로{}

<script>
  var coworkers = ["egoing", "leezhe", "duru", "taeho"];
</script>

<ul>  //unordered list
  <script>
    var i = 0;
    while (i < coworkers.length) { //i는 coworkers의 갯수
      document.write(
        '<li><a href="https://www.youtube.com/results?search_query='+coworkers[i]+'">'
         +coworkers[i]+
          '</a></li>'
      );
      i = i + 1;
    }
  </script>
</ul>

# WEB2 JavaScript - 23.배열과 반복문의 활용

var alist = document.querySelectorAll('a');
var i= 0;
while(i < alist.length){
alist[i].style.color='powderblue';
i=i+1;
}

# WEB2 JavaScript - 24.함수예고

# WEB2 JavaScript - 25.함수

<script>
    function two(){
    document.write('<li>2-1</li>')
    document.write('<li>2-2</li>')
    }
    document.write('<li>1</li>')
    two();
    document.write('<li>3</li>')
    two();
</script>

two를 fuction해라 알려주고 원하는곳에 넣음.

# WEB2 JavaScript - 26.함수 : 매개변수와 인자

함수 function
매개변수 parameter
인자 Argument
출력 Return

<script>
    function OnePlusOne(){
   document.write(1+1+'<br>');
    }

    OnePlusOne();

    function sum(left, right){
        document.write(left+right+'<br>');
    }
    sum(2,3); // 5
    sum(3,4); // 7
</script>

# WEB2 JavaScript - 27.함수 (리턴)

Return함수 사용예시

<script>
    function sum2(left, right) {
            return left+right
    }
    sum2(2,3)
    document.write(sum2(2,3)+'<br>');
    document.write('<div style="color:red">'+sum2(2,3)+'</div>');
    document.write('<div style="font-size:3rem";>'+sum2(2,3)+'</div>');
</script>

document.write대신 return함수를 쓰는이유

<script>
    function sum(left, right){
      document.write(left+right+'<br>');
}
    document.write(sum(2,3));
</script>

위의 sum(2,3)는 document.write(2+3+'<br>') 이다.
document.write(sum(2,3));는 document.write(document.write(2+3+'<br>'));이다.
이럴때 return 함수를 사용함으로서
document.write('<div style="color:red">'+sum2(2,3)+'</div>'); 와 같은 식을 사용할 수 있게된다.
즉 다양한 맥락에서 활용할수 있는 자유도가 생긴다.

# WEB2 JavaScript - 28.함수의 활용

이해부족 넘어감.

# WEB2 JavaScript - 29.객체 예고

객체: 수납상자와 비슷. 정보를 담는그릇에 나중에 꺼낼수 있게 순서는 상관없이 이름을 붙여서 담는다.
즉, 이름이 있는 정리정돈 상자. ex) BodySetColor , NightDayHandler 같은걸 객체라 한다.

- 배열은 대가로[] 객체는 중가로{}

<script>
function BodySetColor(color) {    // function,만든이름,담을기능의 
  document.querySelector("body").style.color = color; // 쿼리셀렉터, 위치, 
}
function BodySetBackgroundColor(color) {
  document.querySelector("body").style.backgroundColor= color; 
}
function nightDayHandler(self) {
  var target = document.querySelector("body");
  if (self.value === "night") {
    Body.setBackgroundColor("black")
    Body.setColor("white");
    self.value = "day";
    LinksSetColor("powderblue");
  } else {
    Body.setBackgroundColor("white");
    Body.setColor("black");
    self.value = "night";
    LinksSetColor("blue");
  }
}
</script>

- 객체에 속해있는 함수는 메소드라고한다.
- function에 이름과 기능을 담은후 기능이 필요할때 이름만 써서 사용하기 편하게 만든것이 함수.

# WEB2 JavaScript - 30.객체 쓰기와 읽기

31.객체와 반복문 에 포함.

# WEB2 JavaScript - 31.객체와 반복문

객체: Object

<script>
  var coworkers = {
    //coworkers 라는 변수 객체에
    programmer: "egoing", // egoing이란 정보를 programmer이란 key에 저장한다는 뜻
    designer: "leezche",
    };

  document.write("programmer: " + coworkers.programmer + "<br>");
  document.write("designer : " + coworkers.designer + "<br>");
  coworkers.bookkeeper = "duru";// coworkers객체에 bookkeeper 이란 정보를 나중에 추가 하고싶을때 
  document.write("bookkeeper : " + coworkers.bookkeeper + "<br>");
  coworkers["data scientist"] = "taeho";
  document.write("data scientist : " + coworkers["data scientist"] + "<br>");
  // data scientist에 띄어쓰기가 있어서 []를 사용해 동일효과 구현.(배열은[]대가로)
  // ex) coworkers.programmer = coworkers[programmer]

 //반복문 for(var key in 내object)를 사용했다.
    for(var key in coworkers) {    //coworkers안에 있는 변수 key를 사용하여,
        document.write(key+'<br>'); // 작성하라, (key)를.
    }
    for(var key in coworkers) {
        document.write(coworkers[key]+'<br>');
    }
    for(var key in coworkers) {
        document.write(key +':'+ coworkers[key]+'<br>');
    }
</script>

# WEB2 JavaScript - 32.객체프로퍼티와 메소드

- 객체에 소속된 함수 : method
- 객체에 소속된 변수: property ex) programmer : "egoing" (둘다 변수.즉 property)
<script>
        var showAll = function(){ };  // 이것과
        function showAll(){ };  //       이것은 똑같은 표현이다.
</script>

<script>
   coworkers.showAll = function () {
     for (var key in this) {
       document.write(key + " : " + this[key] + "<br>");
     }
   }
   coworkers.showAll();
    객체       함수            객체에 소속된 함수이기에 shoAlll은 method이다.
</script>

# WEB2 JavaScript - 33.객체의 활용

함수는 코드가 많아지면 사용하는 정리정돈 도구.
객체는 함수와 변수가 많아지면 그룹핑해서 사용하는 정리정돈 도구.
객체가 많아지면 ....
코드<함수<객체<......

# WEB2 JavaScript - 34.파일로 쪼개서 정리 정돈하기

<head>
    <link rel="stylesheet" href="style.css" />  //css태그를 style.css파일에 담음
    <script src="colors.js"></script>   //script 태그를 colors.js파일에 담음.
</head>
<body>
  <h1><a href="index.html">WEB</a></h1>
  <input type="button"value="night"onclick="
  nightDayHandler(this);"/>  // nightDayHandler는 버튼을 클릭했을때를 위해 만든 만든 객체.
</body>

# WEB2 JavaScript - 35.라이브러리와 프레임워크

라이브러리는 작은것들을 가져다 쓰는느낌
프레임워크는 뼈대 큰것을 세우고 하는 느낌

jquery사용하는법.
cdn, download 등으로 사용할수있는다.

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>등과같은

jquery를 복사해와서 html파일에 넣고 사용법을 보고 필요부분에 코드를 넣는다.

ex) \$("a").css('color',color);

# WEB2 JavaScript - 36.UI vs API

인터페이스 : 두 시스템간의 상호작용 형식
UI : 유저 인터페이스, 사용자와 컴퓨터와의 상호작용 형식
API : 응용프로그램 인터페이스, 응용프로그램과 컴퓨터,운영체제와의 상호작용 형식

"UI는 사용자가 시스템을 제어하기 위해 사용하는 조작 장치이고,
그 조작 장치를 만들려면 API를 가져와서 만들 수 있다"

# WEB2 JavaScript - 37.수업을 마치며
