### π‘ HTML νμ€νΈ μμ 

**(1)  a** : href μμ±μ νμ©νμ¬ λ€λ₯Έ URLλ‘ μ°κ²°νλ νμ΄νΌλ§ν¬ μμ±

```html
<!DOCTYPE html>
    <head>
        <title>html κΈ°μ΄</title>
    </head>
    <body>
      <a href="https://google.com">κ΅¬κΈ</ah>
    </body>
```



**(2) b** : κ΅΅μ κΈμ¨ μμ

```html
<p>The two most popular science courses offered by the school are <b class="term">chemistry</b> (the study of chemicals and the composition of substances) and <b class="term">physics</b> (the study of the nature and properties of matter and energy).</p>

<!--κ΅΅μ κΈμ¨ : chemistry, physics-->
```

![image-20220830023024693](WEB_HTML_CSS(2).assets/image-20220830023024693.png)



**(3) strong** : μ€μν κ°μ‘°νκ³ μ νλ μμ (λ³΄ν΅ κΈμ κΈμ¨λ‘ νν)

```html
<p>Before proceeding, <strong>make sure you put on your safety goggles</strong>.</p>
```

![image-20220830022817598](WEB_HTML_CSS(2).assets/image-20220830022817598.png)



**(4) i** :  κΈ°μΈμ κΈμ¨ μμ

* κΈ°μ  μ©μ΄, μΈκ΅­μ΄ κ΅¬μ , λ±μ₯μΈλ¬Όμ μκ° λ±
* css font-style λ‘ μμ± μ¬μ© κΆμ₯ 

```html
<p>I looked at it and thought <i>This can't be real!</i></p>
```

![image-20220830022224264](WEB_HTML_CSS(2).assets/image-20220830022224264.png)

|   **< em >**   | μμλ κ°μΈ                                |
| :------------: | :----------------------------------------- |
| **< strong >** | **μμλ λ³΄λ€ κ°ν κ°μ‘°**                  |
|  **< mark >**  | **μμλ κ΄λ ¨μ±**                          |
|  **< cite >**  | **μμλ μ±, κ³΅μ°, μμ λ± μ μλ¬Όμ μ΄λ¦** |
|  **< dfn >**   | **μμλ μ μ λμμΈ μ©μ΄**                |



**(5) em** : μ€μν κ°μ‘°νκ³ μ νλ μμ (λ³΄ν΅ κΈ°μΈμ κΈμ¨λ‘ νν)

```html
<p>
  κ³Όκ±°μ <em>block-level</em>μ΄λΌ λΆλ Έλ
  μ½νμΈ λ HTML 5λΆν° <em>flow</em> μ½νμΈ λΌκ³ 
  λ§ν©λλ€.
</p>
```

![image-20220830023237686](WEB_HTML_CSS(2).assets/image-20220830023237686.png)

![image-20220830023606282](WEB_HTML_CSS(2).assets/image-20220830023606282.png)



**(6) br** : νμ€νΈ λ΄μ μ€ λ°κΏ μμ± (μ£Όμλ μμ‘° λ± μ€μ κ΅¬λΆμ΄ μ€μν λ΄μ©μ μμ±ν  λ μ μ©)

: μ¬λ νκ·Έλ νμμλλ€. λ«λ νκ·Έλ μ‘΄μ¬ν΄μ  μλ©λλ€.

: < p >μμμ ν¨κ» CSS margin μμ± λ±μ μ‘°ν©ν΄ κ°κ²© μ‘°μ νκΈ° 

```html
Mozilla Foundation<br>
1981 Landings Drive<br>
Building K<br>
Mountain View, CA 94043-0801<br>
USA
```

![image-20220830023921939](WEB_HTML_CSS(2).assets/image-20220830023921939.png)

##### π  μ κ·Όμ± κ³ λ €μ¬ν­

`λ¬Έλ¨ κ΅¬λΆμ `< br >`λ‘ νλκ±΄ λμ μ¬λ‘μΌ λΏλ§ μλλΌ μ€ν¬λ¦° λ¦¬λλ₯Ό μ¬μ©ν΄ νμνλ μ¬μ©μμκ²λ λ¬Έμ κ° λ©λλ€. `

 `μ€ν¬λ¦° λ¦¬λκ° μμμ μ‘΄μ¬λ μλ €μ£Όκ² μ§λ§, `< br >`μλ μλ¬΄λ° λ΄μ©λ μκΈ° λλ¬Έμλλ€. λ°λΌμ μ¬μ©μλ λ΄μ©μ΄ μ΄λ¨λμ§ λͺ°λΌ νΌλμ λλ μ μμ΅λλ€.`



**(7) img** : src μμ±μ νμ©νμ¬ μ΄λ―Έμ§ νν, alt μμ±μ νμ©νμ¬ λμ²΄ νμ€νΈ

(λ§μΉ `inline-block`μ²λΌ λ³΄μλλ€. border / border-radius, padding / margin, width, height λ±μ μμ±μ μ΄λ―Έμ§μ μ§μ  κ°λ₯ )

```html
<img src="favicon144.png"
     alt="MDN logo">
```

![image-20220830024524302](WEB_HTML_CSS(2).assets/image-20220830024524302.png)



* **μ΄λ―Έμ§ λ§ν¬** 

> μ΄λ―Έμ§λ₯Ό λ§ν¬λ‘ λ°κΎΈλ λ°©λ²
>
>  <img> νκ·Έλ₯Ό <a> μμ λ£κΈ°λ§ νλ©΄ λλ€. 

```html
<a href="https://developer.mozilla.org">
     <img src="favicon144.png" alt="Visit the MDN site">
   </a>
```



* **srcset νΉμ± μ¬μ©νκΈ°** 

> srcset νΉμ±μ κ³ ν΄μλ λ²μ  λ‘κ³  μΆκ° (κ³ ν΄μλ μ΄λ―Έμ§ μ¬μ©)

```html
<img src="favicon72.png"
     alt="MDN logo"
     srcset="favicon144.png 2x">
```



##### π  μ κ·Όμ± κ³ λ €μ¬ν­

` alt νΉμ±μ κ°μ μ΄λ―Έμ§ μ½νμΈ λ₯Ό κ°λ¨νκ³  λͺλ£νκ² μ€λͺ ν΄μΌνλ€. `

`μ΄λ―Έμ§λ₯Ό νμ€νΈλ‘ μ€λͺν  λ°©λ²μ΄ μμ΄μ μλμ μΌλ‘ alt λ₯Ό μ§μ νμ§ μμ κ²½μ°, ν΄λΉ μ΄λ―Έμ§κ° λνλ΄λ €λ λ°λ₯Ό μλ €μ€ μ μλ λ€λ₯Έ λ°©λ²μ κ³ λ €νκΈ°.`

**π λΆμ μ ** 

```html
<img alt="μ΄λ―Έμ§" src="penguin.jpg">
```

**π μ μ **

```html
<img alt="ν΄λ³μ μμλ λ°μλ°κΈ°ν­κ·." src="penguin.jpg">
```



**(8) span** : μλ―Έ μλ μΈλΌμΈ μ»¨νμ΄λ 

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



### π‘ HTML κ·Έλ£Ή μ»¨νμΈ 

**(1) p** : νλμ λ¬Έλ¨ (paragraph)

```html
<p>μ²« λ²μ§Έ λ¬Έλ¨μλλ€.
  μ²« λ²μ§Έ λ¬Έλ¨μλλ€.
  μ²« λ²μ§Έ λ¬Έλ¨μλλ€.
  μ²« λ²μ§Έ λ¬Έλ¨μλλ€.</p>
<p>λ λ²μ§Έ λ¬Έλ¨μλλ€.
  λ λ²μ§Έ λ¬Έλ¨μλλ€.
  λ λ²μ§Έ λ¬Έλ¨μλλ€.
  λ λ²μ§Έ λ¬Έλ¨μλλ€.</p>
```

![image-20220830031417334](WEB_HTML_CSS(2).assets/image-20220830031417334.png)

##### π  νκ·Έ μλ΅

>  λΈλ‘ λ λ²¨ μμμ΄λ©°, μμ μ λ«λ νκ·Έ(`</p>`) μ΄μ μ λ€λ₯Έ λΈλ‘ λ λ²¨ νκ·Έκ° λΆμλλ©΄ μλμΌλ‘ λ«νλ€. 

> μμ νκ·Έλ νμμλλ€. λ«λ νκ·Έλ < p > μμμ λ°λ‘ λ€μ address, article, aside, blockquote, div, dl, fieldset, footer, form, h1, h2, h3, h4, h5, h6, header, hr, menu, nav, pre, section, table, ul, p μμκ° μμΉνλ κ²½μ°, λλ λΆλͺ¨ νκ·Έμ μ½νμΈ κ° λ μ‘΄μ¬νμ§ μκ³  λΆλͺ¨κ° a μμκ° μλ λ μλ΅ κ°λ₯



##### π  μ κ·Όμ± κ³ λ €μ¬ν­ 

`μ½νμΈ λ₯Ό λ¬Έλ¨μΌλ‘ λλλ©΄ νμ΄μ§μ μ κ·Όμ±μ λμΈλ€.`

`μ€ν¬λ¦° λ¦¬λ λ± λ³΄μ‘° κΈ°μ μ λ€μ λ¬Έλ¨μΌλ‘ λμ΄κ° μ μλ λ¨μΆν€ λ±μ μ κ³΅νλ―λ‘, μκ°μ  λ§€μ²΄μ μ¬λ°±μ΄ μ¬μ©μμ λΉ λ₯Έ μ½νμΈ  νμμ λλ κ²κ³Ό κ°μ ν¨κ³Όλ₯Ό μ»μ μ μλ€. μ€ν¬λ¦° λ¦¬λκ° λ¬Έλ¨μ μ‘΄μ¬λ μλ €μ£Όκ² μ§λ§, λ μ½μ λ΄μ©μ΄ μκΈ° λλ¬Έμ λ¬Έλ¨ μ¬μ΄μ μ¬λ°±μ μΆκ°νλ©΄ λΆμ μ μΈ κ²½νμ μ€ μ μλ€. λ°λΌμ μ¬μ©μκ° νΌλμ λλ μ μλ€. `



**(2) hr** : λ¬Έλ¨ λ λ²¨ μμμμμ μ£Όμ μ λΆλ¦¬λ₯Ό μλ―Ένλ©° μνμ μΌλ‘ ννλ¨ (A Horizontal Rule)

* μ΄μΌκΈ° μ₯λ©΄ μ ν, κ΅¬ν λ΄ μ£Όμ  λ³κ²½ λ±, λ¬Έλ¨ λ λ²¨ μμμμ μ£Όμ μ λΆλ¦¬λ₯Ό λνλΈλ€.
* μ¬λ νκ·Έλ νμμλλ€. λ«λ νκ·Έλ μ‘΄μ¬ν΄μ  μλ©λλ€. (λΉ μμ)

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



**(3) ol** : μμκ° μλ λ¦¬μ€νΈ (ordered)

* λ³΄ν΅ μ«μ λͺ©λ‘μΌλ‘ νν

* reversed : λͺ©λ‘μ μμ μ­μ  μ¬λΆ, λ΄λΆμ μ§μ ν ν­λͺ©μ΄ μ­μμΌλ‘ λ°°μ΄λ κ²μΈμ§ λνλ 
* start : ν­λͺ©μ μ λ μμν  μ, typeμ΄ λ‘λ§ μ«μλ μμ΄ λ¬ΈμμΈ κ²½μ°μλ μλΌλΉμ μ«μλ‘ λνλΈ μ μ(1, 2, 3...)λ§ κ°λ₯

```html
<p>Finishing places of contestants not in the winnersβ circle:</p>

<ol start="4">
  <li>Speedwalk Stu</li>
  <li>Saunterinβ Sam</li>
  <li>Slowpoke Rodriguez</li>
</ol>
```

![image-20220830032535810](WEB_HTML_CSS(2).assets/image-20220830032535810.png)

* type : ν­λͺ©μ μ λ μ¬μ©ν  μΉ΄μ΄ν° μ ν 

- `'a'`λ μλ¬Έμ μνλ²³, `'A'`λ λλ¬Έμ μνλ²³, `'i'`λ μλ¬Έμ λ‘λ§ μ«μ, `'I'`λ λλ¬Έμ λ‘λ§ μ«μ, `'1'` λ μ«μ(κΈ°λ³Έκ°)μ λνλλλ€.



**β λ¨κ³λ³ μλ¦¬λ², λ΄λΉκ²μ΄μ, μμμ λ³΄μμ λΉμ¨μ λ΄λ¦Όμ°¨μμΌλ‘ μ λ ¬ν μμ¬λ£ λͺ©λ‘** 



βΌ κ°λ¨ν μμ  

```html
<ol>
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ol>
```

βΌ λ‘λ§ μ«μλ‘ νκΈ° 

```html
<ol type="i">
  <li>Introduction</li>
  <li>List of Greivances</li>
  <li>Conclusion</li>
</ol> 
```

βΌ μ€μ²© λͺ©λ‘ 

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

βΌ μ λ ¬ λͺ©λ‘ μμ λΉμ λ ¬ λͺ©λ‘ 

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



**(4) ul** : μμκ° μλ λ¦¬μ€νΈ (unordered)

* μμκ° μ€μνμ§ μλ€. 

βΌ κ°λ¨ν μμ  

```html
<ul>
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ul>
```

βΌ μ€μ²© λͺ©λ‘ 

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

βΌ λΉμ λ ¬ λͺ©λ‘ μμ μ λ ¬ λͺ©λ‘ 

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



**(5) pre** : HTMLμ μμ±ν λ΄μ©μ κ·Έλλ‘ νν, λ³΄ν΅ κ³ μ ν­ κΈκΌ΄μ΄ μ¬μ©λκ³  κ³΅λ°±λ¬Έμλ₯Ό μ μ§

```html
<p>CSSλ‘ κΈμ μμ λ°κΎΈλκ±΄ μ½μ΅λλ€.</p>
<pre>
body {
  color:red;
}
</pre>
```

![image-20220830033453886](WEB_HTML_CSS(2).assets/image-20220830033453886.png)

##### π  μ κ·Όμ± κ³ λ €μ¬ν­ 

`μλ ₯μ΄ λ?μ μ¬μ©μκ° μ€ν¬λ¦° λ¦¬λμ κ°μ λ³΄μ‘° κΈ°μ μ μ¬μ© μ€μ΄λΌλ©΄, λ―Έλ¦¬ μμ μ μ©ν νμ€νΈμ λ¬Έμλ₯Ό μ°¨λ‘λλ‘ μ½μ΄μλ μ΄κ² λ¬΄μμ μλ―Ένλμ§ μ΄ν΄νμ§ λͺ»ν  μ μμ΅λλ€.`



**(6) blockquote** : νμ€νΈκ° κΈ΄ μΈμ©λ¬Έ μ£Όλ‘ λ€μ¬μ°κΈ°λ₯Ό ν κ²μΌλ‘ ννλ¨

* μ§§μ μΈμ©λ¬Έμ μ¬μ©ν  κ²½μ° < q > μ¬μ©νκΈ° 
* cite : μΈμ©λ¬Έμ μΆμ² λ¬Έμλ λ©μμ§λ₯Ό κ°λ¦¬ν€λ URL. μΈμ©λ¬Έμ λ§₯λ½ νΉμ μΆμ² μ λ³΄λ₯Ό κ°λ¦¬ν¬ μ©λ

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



**(7) div** : μλ―Έ μλ λΈλ‘ λ λ²¨ μ»¨νμ΄λ

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



## **CSS (Cascading )**_ μ€νμ΄μ μ§μ νκΈ° μν μΈμ΄ 

**β­ μμμ μλλ‘ νλ₯΄λ μμ λλ μ’μνλ μλ―Έλ₯Ό κ°κ³  μλ€.** 

**β­ μ€νμΌμ μ§μ νκΈ° μν μΈμ΄, μ ννκ³  μ€νμΌμ μ§μ νλ€. (μμ μ νμ΄ ν΅μ¬)**

![image-20220830034626692](WEB_HTML_CSS(2).assets/image-20220830034626692.png)

* CSS κ΅¬λ¬Έμ μ νμλ₯Ό ν΅ν΄ μ€νμΌμ μ§μ ν  HTML μμλ₯Ό μ ν
* μ€κ΄νΈ μμμλ μμκ³Ό κ°, νλμ μμΌλ‘ μ΄λ£¨μ΄μ§ μ μΈμ μ§ν 
* κ° μμ μ νν μμμ μμ±, μμ±μ λΆμ¬ν  κ°μ μλ―Έ 
  * **μμ± : μ΄λ€ μ€νμΌ κΈ°λ₯μ λ³κ²½ν μ§ κ²°μ **
  * **κ° : μ΄λ»κ² μ€νμΌ κΈ°λ₯μ λ³κ²½ν μ§ κ²°μ **



```html
<!DOCTYPE html>
<html>
  <head>
    <title>μ λͺ©</title>
    <style>
      h1 {
        color: orchid;
        font-size: 15px;
      }
    </style>
  </head>
  <body>
    <h1>μλνμΈμ! HTML CSS</h1>
  </body>
</html>
```

![image-20220830035215568](WEB_HTML_CSS(2).assets/image-20220830035215568.png)



π  **CSS μ μ λ°©λ² μ€ μΈλΌμΈ λ°©λ² μ¬μ©μνκΈ° _ κ°λμ±μ΄ λ¨μ΄μ§** 



---



### π‘ CSS κΈ°μ΄ μ νμ 

* μμ μ νμ 
  * HTML νκ·Έλ₯Ό μ§μ  μ ν 
* ν΄λμ€(class) μ νμ 
  * λ§μΉ¨ν λ¬Έμλ‘ μμνλ©°, ν΄λΉ ν΄λμ€κ° μ μ©λ ν­λͺ©μ μ ν 
* μμ΄λ(id) μ νμ 
  * #λ¬Έμλ‘ μμνλ©°, ν΄λΉ μμ΄λκ° μ μ©λ ν­λͺ©μ μ ν 
  * μΌλ°μ μΌλ‘ νλμ λ¬Έμμ 1λ²λ§ μ¬μ©
  * μ¬λ¬ λ² μ¬μ©ν΄λ λμνμ§λ§, λ¨μΌ idλ₯Ό μ¬μ©νλ κ²μ κΆμ₯ 

