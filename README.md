## 1. HTML

- 웹페이지를 만들기 위한 언어
- 웹페이지 구조를 잡을 수 있다.
- 이미지, 텍스트, 비디오, 버튼 등 웹사이트 보여줄 내용 구성 가능.

<br>

## 2. Browser

1. html파일을 가지고 어떻게 화면에 출력되는지 파악한 후에 웹페이지를 생성한다.
2. Chorme, Safari, Firefox,IE 등 다양한 브라우저가 존재.

<br>

## 3. Tag

1. 태그의 기본 개념
2. html에서 image나 text를 그려주려면 그에 맞는 태그가 필요.
3. 대부분의 태그는 시작 태그와 끝 태그로 구성되어 있다.
4. 예외로 img, br, input등의 태그들은 끝 태그 없이 사용 가능하다.

<br>

## 4. Element (요소)

<br>

<center>
<img src="https://user-images.githubusercontent.com/67410919/99141294-61eb8000-268d-11eb-8468-3b11a09d1763.png" width="300" height="200">
</center>

<br>

## 5. Attribute(속성)

1. 속성은 시작 태그에 위치하며 한 태그에 여러 속성을 지정할 수 있다.
2. div, a, img는 Tag이고 class, href, src, alt는 Attribute이다.

```html
ex1)
<div class="title">제목</div>
ex2) <a href="www.google.com"> </a>
```

<br>

## 6. HTML 파일의 기본 구조

1. DOCTYPE

   1. HTML파일이라면 제일 첫줄에 위치해야하는 선언문
   2. 태그와 비슷하지만 HTML태그는 아니다.
   3. 해당 HTML파일이 무슨 버전을 사용했는지 브라우저에 알리는 역할이다.

2. Html Tag
   1. html elements 들은 html태그로 감싸져 있다.
   2. 브라우저가 html태그를 만나면, html이 시작된것으로 인지하고 요소를 그릴 준비를 한다.
3. head Tag

   1. html태그 다음에는 항상 head태그가 위치한다.
   2. body태그와 다르게 웹브라우저에 보이지 않는 부분이다.
   3. 사이트의 제목, 설명, 부가정보, 기술적 내용이 들어간다.
   4. 한글, 일본어, 중국어가 포함된 페이지라면 meta charset="utf-8"값으로 문자 인코딩을 추가해주어야 한다.
   5. 모바일에서 웹사이트를 사용하는 유저들을 위해 추가해야 하는 정보로 이 정보를 추가하지 않으면 데스크탑 버전의 웹페이지가 축소되어 보이는 현상이 나타난다. > meta name="viewport" content="width-device-width" 이 코드는 디바이스와 웹페이지의 가로 길이가 같다는 의미이다.
   6. title 태그는 브라우저 탭에 보여지는 페이지의 이름이다.

4. body Tag

   1. body 태그는 항상 head 태그 다음에 위치한다.
   2. 화면에 보여져야할 레이아웃대로 각종 태그들이 존재한다.

5. span & div Tag

   1. span태그에는 주로 텍스트를 넣어준다.
   2. span태그는 line brake가 되지 않고 한줄에 이어서 나오게된다. 이러한 요소를 inline-element라고 한다.
   3. div태그는 웹사이트에서 섹션을 나눌 때 사용하며 특별한 기능은 없다.
   4. 그럼에도 div태그를 사용하는 이유는 비슷한 부분끼리 그룹화하거나 디자인에 맞게 레이아웃을 분리하고 각 div태그에 class나 id attribute를 부여하고 css스타일을 입혀줄 수 있기 때문이다.

6. h# & p & a Tag
   1. h1 ~ h5 태그는 제목과 같은 텍스트를 보여줄 떄 사용한다. 숫자가 올라갈수록 글자 크기가 점점 작아진다.
   2. p태그는 paragraph의 줄임말로, 텍스트를 주로 넣어준다. 주로 문단을 통로에 넣을때 많이 사용.
   3. 한 줄에 이어서 나오지 않고 단락이 나뉘는 요소인 block-element 속성이다.
   4. a태그는 링크를 걸어줄때 사용되며 href 속성에 이동해야 하는 주소를 써준다. 많은 속성들을 가지고 있다.
