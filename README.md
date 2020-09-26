생활코딩 web2 CSS (html+css)

강의: WEB2 CSS-4.CSS의 기본 문법



배운내용: 

HTML에 CSS를 적용하는 방법
1. style 속성 사용
<a href="2.html" style="color:red;text-decoration:underline">CSS</a>
style은 href 태그의 속성으로 사용됐다. 속성으로 사용되면 선택자가 필요없다.

2. style 태그 사용
<style>
    a {
      color:black;
      text-decoration: none;
    }
</style>  

3. 용어
선언,효과(declaration) : color:black; text-decoration:none; 
;은 description 구분하기위해 사용
a{선언} : 선택자(selector) 















CSS의 특징
1. html 이 정보에 전념하게 하기 위해서, html로부터 디자인의 기능을 빼온 것
2. html을 통해서 디자인을 하는 것보다 훨씬더 효율 적이기 때문에
 (중복제거, 가독성 좋아짐, 수정하기 편함)

핵심내용
1. html_정보. css_디자인
2. style{ }로 이제 부터 CSS언어 문법에 맞게 처리하자

<!--
<style>
a {color : red;}
</style>
-->
