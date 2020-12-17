생활코딩 web2 CSS (html+css)

---

# CSS-3.CSS의 등장

CSS의 특징

- html 이 정보에 전념하게 하기 위해서, html로부터 디자인의 기능을 빼온 것
- html을 통해서 디자인을 하는 것보다 훨씬더 효율 적이기 때문에
  (중복제거, 가독성 좋아짐, 수정하기 편함)

핵심내용

- html*정보. css*디자인
- <style>로 이제 부터 CSS언어 문법에 맞게 처리하자

<!--
<style>
a {color : red;}
</style>
-->

---

# CSS-4.CSS의 기본 문법

HTML에 CSS를 적용하는 방법

1. style 속성 사용
   <a href="2.html" style="color:red;text-decoration:underline">CSS</a>
   style은 a 태그의 속성으로 사용됐다. 속성으로 사용되면 선택자가 필요없다.

2. style 태그 사용
<style>
    a {
      color: black;
      text-decoration: none;
    }
</style>

3. 용어

<style>
- div {color: red; padding:5px;}

  </style> : style태그

div : 선택자 div태그
{ } : 선언블록
color:red; : 선언,효과(declaration)
color : 속성
red : 속성값

- ( ; 는 description 구분하기위해 사용)
- 선택자(selector)는 { 가 나오기 전 전부를 선택자라 부른다.

---

# CSS-6.CSS 속성을 스스로 알아내기

속성(property)을 스스로 알아내는 방법, 그리고 기계가 알려주는 자동완성을 활용하자!
구글에서 css text center, css text size property 등을 검색
font-size: 00px;
text-align(정렬): center;

---

# CSS-7.CSS 선택자의 기본

선택자에는 위계관계에 따른 우선 적용 순위가 존재한다.
id(#grid) > class(.saw) > element(div)
구체적 > 중간 > 포괄적 순서이다
id 는 문서에서 딱 한 번만 등장하는 유일무이한 선택자.

태그 이름이 saw 일때는 saw{ }이지만 class="saw"일때는 .saw 라고 쓰기로 약속되있다.

-예시 코드

<head>
  <style>
    div {
      color:black;
    }
    #grid {
      color: red;
    }
    .saw {
      color: gray
    }
  </style>
</head>
<body>
    <div href="1.html" class="saw">HTML</div>
    <div href="2.html" class="saw" id="grid">CSS</div>
</body>

---

# CSS-8.박스모델

# CSS-9.박스 모델 써먹기

- CSS박스모델: border, padding, margin, width, height
- 브라우저에서 우클릭 -> inspect(검사) 하여 CSS 박스모델이 어떻게 사용됐는지 파악할 수 있다.
- 용어 헷갈리면 구글 이미지검색등에 CSS box model 등을 치면 나온다.

  block: block level element (주변화면 전체를 사용)
  inline: 부피만큼만 사용한다
  none: 없는것으로 간주
  hidden:화면에서 감춰짐

- <예시 코드>
  <>
  h1{
  font-size: 45px;
  text-align: center;
  border:5px solid red; /border으로 묶어 중복 제거/
  padding-bottom: 20px;  
   margin:20px;
  display:block; /inline, block 등 으로 변경할 수 있다./
  width:100px  
   }
  </>

---

# CSS-10.그리드 소개

# CSS-11.그리드 써먹기

grid: 화면 크기에 맞추어 비율을 자동으로 조절되게 해주는 기술
div: 어떤 의미도 존재하지 않는 block level element tag (주변전체사용)
span: 어떤 의미도 존재하지 않는 inline element tag (부피만큼사용)
caniuse.com 을 통해 사용가능한 코드들을 확인할 수 있다.

- grid의 사용

  width: 800px;
  display:grid;
  grid-template-columns: 300px 10% 1fr 1fr;
  /이면, 300px 80px 210px 210px 가 된다.즉, 800에서 -300, -10%, 남은것 1:1비율/

- grid 사용 예시

  <head>
    <>
      #grid{
          display:grid;
          grid-template-columns: 2fr 1fr 1fr (2:1:1비율)
          }
    </>
  </head>

  <body>
      <div id="grid">
  <body>

.은 class에, #은 id 에 붙이며
.tag 와 <div class="tag">안녕</div> 혹은 #tag 와 <div id="tag"> 로 사용하고

style
.tag or #tag
display:grid;
grid-template-columns: 10px 1fr
/style
과 같이 사용한다.

---

# CSS-12.미디어 쿼리 소개

- 미디어 쿼리: @media(min-width:800px) { }
  최소 또는 최대 폭부터 { } 가 작동하게 해주는 태그

- 예시
  @media(min-width:800px) {div {display:none;}}

800px 보다 크다면 { } 를 동작시킨다
{ } 안에 div{} 가 있으므로 800px보다 클때 화면을 안보이게 만든다.
min: 최소~~부터
max: 최대~~까지
최대100까지는 0~100 까지.

---

# CSS-13.미디어 쿼리 써먹기

@media(max-width:800px){
#grid {
display: block;
}
ol {
border-right: none;
}
h1 {
border-bottom: none;
}
}
창을 800px보다 작게 줄이면 보더(선) 을 안보이게 하는동시에 #grid{display:block;}을 주어 두번째 블록인 P 태그를 아래로 내려오게 한다.

---

# CSS-14.CSS 코드의 재사용

- link 태그 사용으로 여러페이지에 CSS 동시적용

* 적용할 여러 페이지의 <head></head> 사이에 link 태그를 넣어주고
  <style></style> 태그를 새 파일에 넣어버린다

- 링크태그
<link rel="stylesheet" href="style.css"> 
(style.css 는 style 코드만 빼놓은 새파일 이름)
