# html 세팅

<!doctype html>
  <html></html>
    <head></head>
      <title>제목</title>
      <meta charset="utf-8(문자타입)">
    </head>
    <body>
      본문
    </body>
    </html>

- charset: character set 문자 규칙</p>

# htlml 태그

<h1></h1> ~ <h6></h6> 
heading tag.
H1 is biggest and H6 is smallest size of heading.

<b></b>
bold tag

<strong></strong>
similar to bold text.

<p></p>
Paragraph tag
uses fron and end of paragraph to know mark where is start and end of the paragraph.

<br></br>
breaking line
use when need to start in new line.

<u></u>
underline

# 이미지 삽입

1. 이미지를 작업폴더에 넣기
2. 편집기에 자동 생성됨.
3. 이미지 넣기를 원하는 부분에 <img src="파일이름".jpg" width="크기">

- width can be any number and %. for ex, 200 or 50%. and it call 속성

# 부모태그

ol: ordered list(부모태그)
ul: unordered list(부모태그)
li: list(자식태그)
부모태그<ol>, <ul> 다음은 자식태그<li></li>가 반드시 와야한다

<ol>
  <li>1번목록</li>
  <li>2번목록</li>
</ol>

# HyperLink(하이퍼링크) 삽입

<a href="https://www.w3.org/TR/html52/" target="_blank" title="html5 specification">눌리게만들고싶은글</a>

- a : anchor 닻(글자 눌리게만들때)
- target: 누르면 열리는 방법(\_blank, \_parent, \_self, \_top, frame name)
- title : 설명
