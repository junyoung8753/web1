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

- data type

* 숫자number(1,2,3...)
* 문자(a,b,c...#,\$...)
* 문자열string(hello,ohmygod,...)

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

Javascript select tag by css selector

---- 이해 다 안됨. 일단 넘어감------

# WEB2 JavaScript - 13.프로그램,프로그래밍,프로그래머

PROGRAM 은 순서라는 의미가 들어있다
순서를 만드는것을 PROGRAMMING 이라하고
순서를 만드는 사람을 PROGRAMMER 라고 한다.

순서에 '패턴'이 발생한다면 굳이, 계속, 일일이 반복할 이유가 사라진다. 실증난다.
그래서 프로그램을 짜고 그에 걸맞는 언어를 만들어냈다.

HTML은 웹페이지를 묘사하는 목적의 언어이기에 시간의 순서에 따라 진행되지 않는다.
JavaScript는 시간의 순서에 따라 실행되기에 프로그래밍 언어라 볼수 있다.
