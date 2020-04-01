# CSS_Master

Cloning some Webpages

### 2019 1. 2. 3.

..

CSS Master (Flexbox, Grid, PostCSS, CSSNext)

### CSS Flex

[] CSS Flex Basics
[] Main Axis and Cross Axis
[] Flex Direction
[] Flex Wrap
[] Align Self

### CSS Grid

[] CSS Grid Basics ( Row, columns and gaps)
[] Auto columns, auto rows
[] Template Areas
[] fr unit, repeat
[] minmax, max-content, min-content
[] auto-fill, auto-fit
[] Justify Content, Align Content and Place Content
[] Justify Items, Align Items and Place Items

justify, Align content는 box 자체를 움직인다.
justify, Align items는 box 안에 있는 content를 움직인다.
place content: (justify) (Align)
place items: (justify) (Align)

[] Grid Column, Column Start and End
[] Line Naming

[] Grid Row, Row Start and End

---

.box:first-child {
grid-row: 1 / 5
}
box 안 첫번째 자식에게 1부터 5까지 가져가라고 명령하는 것이다.

span을 써서 더 편하게 사용할 수 있다.
.box:first-child {
grid-row: span 5
}
라고 쓰면은 5개 너가 써 라고 컴퓨터에게 말하는 것과 같다.

[] Grid Area

---

grid-area: 2 / 1 / 4 / -1;
row start / column start / row end / column end 이다.
만약 2개를 적을 경우
grid-area: span4 span4

span 4 / span 4
row span4, column span4가 적용됩니다.

[] Justify, Align, Place Self

---

하나의 box에 대한 align이나 justify 값을 바꿀 때 사용한다.
justify-self: center;
align-self: center;
place-self: (justify) (align);

### Using CSS4

[] Installing Parcel
[] Configuring PostCSS
[] Testing

### CSS4 Awesomeness

[] :matches , :not

---

matches, not는 마치 if와 else와 같다.
matches 다음에 해당되는 속성을 기입해주면 해당라인에 적용된다.
not은 해당속성을 제외하고 적용된다.
.target을 해주면, index.html에서 target으로 지정한 라인에도 적용된다.

[] CSS Variables
[] @custom-selector

---

:root{
// 변수를 선언하고 값을 넣어준다. 변수앞에는 항상 --가 붙는다.
--awesomeColor: 2px solid #2980b9
}
이후 해당 엘리멘트에 var 키워드와 해당 변수를 사용해서 속성(color, border 등)에 저장할 수 있다.
이유는 자주 바뀔 수 있는 속성값을 편하게 제어하기 위해서이다.
@custom-selector는 property가 아니고 selection of element라고 한다.

[] @custom-media
[] Media Query Ranges
[] color-mod, gray(), system-ui
[] Nesting Rules

---

nesting rule을 사용하면 셀렉터를 더 줄일 수 있다.

& 를 사용해 HTML 내부 태그처럼 CSS또한 트리구조로 정리 가능
nesting selector는 매우 강력해서 덮어쓰기가 되지 않는다.
(CSS에서는 더 자세할수록, 더 깊을수록 강력한 우선순위 code가 된다.)
기존 CSS에서도 명확한 선택자가 우위를 선점했던 것가 같은 원리이다.

Conclusions
[] CSS Grid Kiss
[] Practice Flexbox
[] Practice Grid
