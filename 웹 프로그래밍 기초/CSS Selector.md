## 3-2) CSS Selector

<br/>


학습 목표
   - 기본적인 Selector 문법을 이해한다.

### Selector

   - 트리구조로 되어있는 selector를 속성과 테그이름으로 빠르게 찾는 방법

###CSS Selector의 다양한 활용

   - id, class 요소 선택자와 함께 활용  


~~~
#myid { color : red }
div.myclassname { color : red }
~~~

   - 그룹 선택 (여러 개 셀렉터에 같은 style을 적용해야 한다면)
~~~
h1, span, div { color : red }
h1, span, div#id { color : red }
h1.span, div.classname { color : red }
~~~
   - 요소 선택 (공백) : 자손요소
   - 아래 모든 span태그에 red색상이 적용됨
~~~
<div id="jisu">
  <div>
    <span> span tag </span>
  </div>
  <span> span tag 2 </span>
</div>
~~~

~~~
#jisu span { color : red }
~~~

   - 자식 선택 (>) : 자식은 바로 하위엘리먼트를 가리킵니다.
   - 아래는 span tag 2만 red 색상이 적용됩니다.
~~~
<div id="jisu">
  <div>
    <span> span tag </span>
  </div>
  <span> span tag 2 </span>
</div>
~~~

~~~
#jisu > span { color : red }
~~~
 

   - n번째 자식요소를 선택합니다. (nth-child)
   - 첫번째 단락에 red 색상이 적용됩니다.

~~~
<div id="jisu">
  <h2>단락 선택</h2>
  <p>첫번째 단락입니다</p>
  <p>두번째 단락입니다</p>
  <p>세번째 단락입니다</p>
  <p>네번째 단락입니다</p>
</div>
~~~

~~~
#jisu > p:nth-child(2) { color : red }
~~~


-참고자료-
부스트코스 - 웹프로그래밍









  
































