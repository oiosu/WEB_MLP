### 💡 HTML 텍스트 요소 

**(1)  a** : href 속성을 활용하여 다른 URL로 연결하는 하이퍼링크 생성

```html
<!DOCTYPE html>
    <head>
        <title>html 기초</title>
    </head>
    <body>
      <a href="https://google.com">구글</ah>
    </body>
```



**(2) b** : 굵은 글씨 요소

```html
<p>The two most popular science courses offered by the school are <b class="term">chemistry</b> (the study of chemicals and the composition of substances) and <b class="term">physics</b> (the study of the nature and properties of matter and energy).</p>

<!--굵은 글씨 : chemistry, physics-->
```

![image-20220830023024693](WEB_HTML_CSS(2).assets/image-20220830023024693.png)



**(3) strong** : 중요한 강조하고자 하는 요소 (보통 긁은 글씨로 표현)

```html
<p>Before proceeding, <strong>make sure you put on your safety goggles</strong>.</p>
```

![image-20220830022817598](WEB_HTML_CSS(2).assets/image-20220830022817598.png)



**(4) i** :  기울임 글씨 요소

* 기술 용어, 외국어 구절, 등장인물의 생각 등
* css font-style 로 속성 사용 권장 

```html
<p>I looked at it and thought <i>This can't be real!</i></p>
```

![image-20220830022224264](WEB_HTML_CSS(2).assets/image-20220830022224264.png)

|   **< em >**   | 요소는 강세                                |
| :------------: | :----------------------------------------- |
| **< strong >** | **요소는 보다 강한 강조**                  |
|  **< mark >**  | **요소는 관련성**                          |
|  **< cite >**  | **요소는 책, 공연, 음악 등 저작물의 이름** |
|  **< dfn >**   | **요소는 정의 대상인 용어**                |



**(5) em** : 중요한 강조하고자 하는 요소 (보통 기울임 글씨로 표현)

```html
<p>
  과거에 <em>block-level</em>이라 불렸던
  콘텐츠는 HTML 5부터 <em>flow</em> 콘텐츠라고
  말합니다.
</p>
```

![image-20220830023237686](WEB_HTML_CSS(2).assets/image-20220830023237686.png)

![image-20220830023606282](WEB_HTML_CSS(2).assets/image-20220830023606282.png)



**(6) br** : 텍스트 내에 줄 바꿈 생성 (주소나 시조 등 줄의 구분이 중요한 내용을 작성할 때 유용)

: 여는 태그는 필수입니다. 닫는 태그는 존재해선 안됩니다.

: < p >요소와 함께 CSS margin 속성 등을 조합해 간격 조절하기 

```html
Mozilla Foundation<br>
1981 Landings Drive<br>
Building K<br>
Mountain View, CA 94043-0801<br>
USA
```

![image-20220830023921939](WEB_HTML_CSS(2).assets/image-20220830023921939.png)

##### 🛠 접근성 고려사항

`문단 구분을 `< br >`로 하는건 나쁜 사례일 뿐만 아니라 스크린 리더를 사용해 탐색하는 사용자에게도 문제가 됩니다. `

 `스크린 리더가 요소의 존재는 알려주겠지만, `< br >`에는 아무런 내용도 없기 때문입니다. 따라서 사용자는 내용이 어딨는지 몰라 혼란을 느낄 수 있습니다.`



**(7) img** : src 속성을 활용하여 이미지 표현, alt 속성을 활용하여 대체 텍스트

(마치 `inline-block`처럼 보입니다. border / border-radius, padding / margin, width, height 등의 속성을 이미지에 지정 가능 )

```html
<img src="favicon144.png"
     alt="MDN logo">
```

![image-20220830024524302](WEB_HTML_CSS(2).assets/image-20220830024524302.png)



* **이미지 링크** 

> 이미지를 링크로 바꾸는 방법
>
>  <img> 태그를 <a> 안에 넣기만 하면 된다. 

```html
<a href="https://developer.mozilla.org">
     <img src="favicon144.png" alt="Visit the MDN site">
   </a>
```



* **srcset 특성 사용하기** 

> srcset 특성에 고해상도 버전 로고 추가 (고해상도 이미지 사용)

```html
<img src="favicon72.png"
     alt="MDN logo"
     srcset="favicon144.png 2x">
```



##### 🛠 접근성 고려사항

` alt 특성의 값은 이미지 콘텐츠를 간단하고 명료하게 설명 해야한다. `

`이미지를 텍스트로 설명할 방법이 없어서 의도적으로 alt 를 지정하지 않은 경우, 해당 이미지가 나타내려는 바를 알려줄 수 있는 다른 방법을 고려하기.`

**👉 부적절** 

```html
<img alt="이미지" src="penguin.jpg">
```

**👉 적절**

```html
<img alt="해변에 서있는 바위뛰기펭귄." src="penguin.jpg">
```



**(8) span** : 의미 없는 인라인 컨테이너 

```html
<li><span>
    <a href="portfolio.html" target="_blank">See my portfolio</a>
</span></li>
```

```css
li span {
  background: gold;
 }
```

![image-20220830031015066](WEB_HTML_CSS(2).assets/image-20220830031015066.png)

---



### 💡 HTML 그룹 컨텐츠

**(1) p** : 하나의 문단 (paragraph)

```html
<p>첫 번째 문단입니다.
  첫 번째 문단입니다.
  첫 번째 문단입니다.
  첫 번째 문단입니다.</p>
<p>두 번째 문단입니다.
  두 번째 문단입니다.
  두 번째 문단입니다.
  두 번째 문단입니다.</p>
```

![image-20220830031417334](WEB_HTML_CSS(2).assets/image-20220830031417334.png)

##### 🛠 태그 생략

>  블록 레벨 요소이며, 자신의 닫는 태그(`</p>`) 이전에 다른 블록 레벨 태그가 분석되면 자동으로 닫힌다. 

> 시작 태그는 필수입니다. 닫는 태그는 < p > 요소의 바로 뒤에 address, article, aside, blockquote, div, dl, fieldset, footer, form, h1, h2, h3, h4, h5, h6, header, hr, menu, nav, pre, section, table, ul, p 요소가 위치하는 경우, 또는 부모 태그의 콘텐츠가 더 존재하지 않고 부모가 a 요소가 아닐 때 생략 가능



##### 🛠 접근성 고려사항 

`콘텐츠를 문단으로 나누면 페이지의 접근성을 높인다.`

`스크린 리더 등 보조 기술은 다음 문단으로 넘어갈 수 있는 단축키 등을 제공하므로, 시각적 매체의 여백이 사용자의 빠른 콘텐츠 탐색을 돕는 것과 같은 효과를 얻을 수 있다. 스크린 리더가 문단의 존재는 알려주겠지만, 더 읽을 내용이 없기 때문에 문단 사이에 여백을 추가하면 부정적인 경험을 줄 수 있다. 따라서 사용자가 혼란을 느낄 수 있다. `



**(2) hr** : 문단 레벨 요소에서의 주제의 분리를 의미하며 수평선으로 표현됨 (A Horizontal Rule)

* 이야기 장면 전환, 구획 내 주제 변경 등, 문단 레벨 요소에서 주제의 분리를 나타낸다.
* 여는 태그는 필수입니다. 닫는 태그는 존재해선 안됩니다. (빈 요소)

```html
<p>
This is the first paragraph of text.
This is the first paragraph of text.
This is the first paragraph of text.
This is the first paragraph of text.
</p>

<hr>

<p>
This is second paragraph of text.
This is second paragraph of text.
This is second paragraph of text.
This is second paragraph of text.
</p>
```



![image-20220830032230874](WEB_HTML_CSS(2).assets/image-20220830032230874.png)



**(3) ol** : 순서가 있는 리스트 (ordered)

* 보통 숫자 목록으로 표현

* reversed : 목록의 순서 역전 여부, 내부의 지정한 항목이 역순으로 배열된 것인지 나타냄 
* start : 항목을 셀 때 시작할 수, type이 로마 숫자나 영어 문자인 경우에도 아라비아 숫자로 나타낸 정수(1, 2, 3...)만 가능

```html
<p>Finishing places of contestants not in the winners’ circle:</p>

<ol start="4">
  <li>Speedwalk Stu</li>
  <li>Saunterin’ Sam</li>
  <li>Slowpoke Rodriguez</li>
</ol>
```

![image-20220830032535810](WEB_HTML_CSS(2).assets/image-20220830032535810.png)

* type : 항목을 셀 때 사용할 카운터 유형 

- `'a'`는 소문자 알파벳, `'A'`는 대문자 알파벳, `'i'`는 소문자 로마 숫자, `'I'`는 대문자 로마 숫자, `'1'` 는 숫자(기본값)을 나타냅니다.



**✔ 단계별 요리법, 내비게이션, 영양정보에서 비율의 내림차순으로 정렬한 원재료 목록** 



◼ 간단한 예제 

```html
<ol>
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ol>
```

◼ 로마 숫자로 표기 

```html
<ol type="i">
  <li>Introduction</li>
  <li>List of Greivances</li>
  <li>Conclusion</li>
</ol> 
```

◼ 중첩 목록 

```html
<ol>
  <li>first item</li>
  <li>second item  <!-- closing </li> tag not here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
  </li>            <!-- Here's the closing </li> tag -->
  <li>third item</li>
</ol>
```

◼ 정렬 목록 안의 비정렬 목록 

```html
<ol>
  <li>first item</li>
  <li>second item      <!-- Look, the closing </li> tag is not placed here! -->
    <ul>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ul>
  </li>                <!-- Here is the closing </li> tag -->
  <li>third item</li>
</ol>
```



**(4) ul** : 순서가 없는 리스트 (unordered)

* 순서가 중요하지 않다. 

◼ 간단한 예제 

```html
<ul>
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ul>
```

◼ 중첩 목록 

```html
<ul>
  <li>first item</li>
  <li>second item
  <!-- Look, the closing </li> tag is not placed here! -->
    <ul>
      <li>second item first subitem</li>
      <li>second item second subitem
      <!-- Same for the second nested unordered list! -->
        <ul>
          <li>second item second subitem first sub-subitem</li>
          <li>second item second subitem second sub-subitem</li>
          <li>second item second subitem third sub-subitem</li>
        </ul>
      </li> <!-- Closing </li> tag for the li that
                  contains the third unordered list -->
      <li>second item third subitem</li>
    </ul>
  <!-- Here is the closing </li> tag -->
  </li>
  <li>third item</li>
</ul>
```

◼ 비정렬 목록 안의 정렬 목록 

```html
<ul>
  <li>first item</li>
  <li>second item
  <!-- Look, the closing </li> tag is not placed here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
  <!-- Here is the closing </li> tag -->
  </li>
  <li>third item</li>
</ul>
```



**(5) pre** : HTML에 작성한 내용을 그대로 표현, 보통 고정폭 글꼴이 사용되고 공백문자를 유지

```html
<p>CSS로 글자 색을 바꾸는건 쉽습니다.</p>
<pre>
body {
  color:red;
}
</pre>
```

![image-20220830033453886](WEB_HTML_CSS(2).assets/image-20220830033453886.png)

##### 🛠 접근성 고려사항 

`시력이 낮은 사용자가 스크린 리더와 같은 보조 기술을 사용 중이라면, 미리 서식 적용한 텍스트의 문자를 차례대로 읽어서는 이게 무엇을 의미하는지 이해하지 못할 수 있습니다.`



**(6) blockquote** : 텍스트가 긴 인용문 주로 들여쓰기를 한 것으로 표현됨

* 짧은 인용문을 사용할 경우 < q > 사용하기 
* cite : 인용문의 출처 문서나 메시지를 가리키는 URL. 인용문의 맥락 혹은 출처 정보를 가리킬 용도

```html
<blockquote cite="https://tools.ietf.org/html/rfc1149">
  <p>Avian carriers can provide high delay, low
  throughput, and low altitude service.  The
  connection topology is limited to a single
  point-to-point path for each carrier, used with
  standard carriers, but many carriers can be used
  without significant interference with each other,
  outside of early spring.  This is because of the 3D
  ether space available to the carriers, in contrast
  to the 1D ether used by IEEE802.3.  The carriers
  have an intrinsic collision avoidance system, which
  increases availability.</p>
</blockquote>
```

![image-20220830033813040](WEB_HTML_CSS(2).assets/image-20220830033813040.png)



**(7) div** : 의미 없는 블록 레벨 컨테이너

```html
<div class="shadowbox">
  <p>Here's a very interesting note displayed in a
  lovely shadowed box.</p>
</div>
```

```css
.shadowbox {
  width: 15em;
  border: 1px solid #333;
  box-shadow: 8px 8px 5px #444;
  padding: 8px 12px;
  background-image: linear-gradient(180deg, #fff, #ddd 40%, #ccc);
}
```

![image-20220830034022779](WEB_HTML_CSS(2).assets/image-20220830034022779.png)





---



## **CSS (Cascading )**_ 스타이을 지정하기 위한 언어 

**⭐ 위에서 아래로 흐르는 상속 또는 종속하는 의미를 갖고 있다.** 

**⭐ 스타일을 지정하기 위한 언어, 선택하고 스타일을 지정한다. (요소 선택이 핵심)**

![image-20220830034626692](WEB_HTML_CSS(2).assets/image-20220830034626692.png)

* CSS 구문은 선택자를 통해 스타일을 지정할 HTML 요소를 선택
* 중괄호 안에서는 속상과 값, 하나의 쌍으로 이루어진 선언을 진행 
* 각 쌍은 선택한 요소의 속성, 속성에 부여할 값을 의미 
  * **속성 : 어떤 스타일 기능을 변경할지 결정**
  * **값 : 어떻게 스타일 기능을 변경할지 결정**



```html
<!DOCTYPE html>
<html>
  <head>
    <title>제목</title>
    <style>
      h1 {
        color: orchid;
        font-size: 15px;
      }
    </style>
  </head>
  <body>
    <h1>안녕하세요! HTML CSS</h1>
  </body>
</html>
```

![image-20220830035215568](WEB_HTML_CSS(2).assets/image-20220830035215568.png)



🛠 **CSS 정의 방법 중 인라인 방법 사용안하기 _ 가독성이 떨어짐** 



---



### 💡 CSS 기초 선택자 

* 요소 선택자 
  * HTML 태그를 직접 선택 
* 클래스(class) 선택자 
  * 마침표 문자로 시작하며, 해당 클래스가 적용된 항목을 선택 
* 아이디(id) 선택자 
  * #문자로 시작하며, 해당 아이디가 적용된 항목을 선택 
  * 일반적으로 하나의 문서에 1번만 사용
  * 여러 번 사용해도 동작하지만, 단일 id를 사용하는 것을 권장 

