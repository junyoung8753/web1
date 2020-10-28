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

* 문자(a,b,c...#,\$...)
* 숫자(1,2,3...)
* 문자열(hello,ohmygod,...)

- javascript string(문자열) 프로퍼티

* .toUpperCase 대문자로 바꿔줌
* .indexOf 몇번째에 찾는 문자가 있는지 알려줌
* .trim() 공백 없애줌

"1" 은 문자, 1 은 숫자
1+1 은 2, "1"+"1" 은 11이다
그러나, html 에서는 타이핑한 문자가 그대로 나온다.

# WEB2 JavaScript - 7.변수와 대입 연산자
