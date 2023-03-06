# Layouts: Floats, FlexBox and CSS Grid Fundamentals

## 1) THE 3 WAYS OF BUILDING LAYOUTS

### (1) What Does "Layout" Mean ?

-   Layout is the way text, image, and other content is placed and arranged on a webpage
-   Layout gives the page a visual structure, into which we place our content.
-   **Buliding a layout**: arranging page elements into a visual structure, instead of simply having them placed one after another (normal flow)

<br>

### (2) The 3 Ways of Building Layouts With CSS

-   **FLOAT LAYOUTS** : The old way of building layouts of all size, using the float css property. still used, but getting outdated fast.
-   **FLEXBOX**: Modern way of laying out elements in a 1-dimensional row without using floats. Perfect for component layouts.
-   **CSS GRID**: For laying out element in a fully-fledged 2-dimensional grid. Perfect for page layouts and complex components.

<br><br>

---

# 1. Float

## 1) Using Floats

-   아래 header 영역은 child에 float 속성을 주게 되면 기존에 자식 요소만큼 차지하고 있던 높이에서 height: 0으로 바뀐다. (Collapsing Height 발생)
-   float 속성을 사용하여 parent 하위에 child 요소가 없는 것으로 판단하기 떄문이다.

<br>

```html
<header class="main-header">
    <h1>📘 The Code Magazine</h1>

    <nav>
        <!-- <strong>This is the navigation</strong> -->
        <a href="blog.html">Blog</a>
        <a href="#">Challenges</a>
        <a href="#">Flexbox</a>
        <a href="#">CSS Grid</a>
    </nav>
</header>
```

```css
.main-header {
    background-color: #f7f7f7;
    padding: 20px 40px;
    margin-bottom: 60px;
}

h1 {
    float: left;
}

nav {
    float: right;
}
```

<br>

### (1) Floats

-   Element is removed from the normal flow: "out of flow"
-   Text and inline elements will wrap around the floated element.
-   The container will not adjust its height to the element.
-   udemy 강의 css pdf 파일 64 페이지 참고!

<br>

```css
float: left;
float: right;
```

<br><br>

## 2) Clearing Floats

### (1) empty div를 만든다.

<br>

```html
<header class="main-header">
    <h1>📘 The Code Magazine</h1>

    <nav>
        <!-- <strong>This is the navigation</strong> -->
        <a href="blog.html">Blog</a>
        <a href="#">Challenges</a>
        <a href="#">Flexbox</a>
        <a href="#">CSS Grid</a>
    </nav>

    <div class="clear"></div>
</header>
```

```css
.clear {
    clear: both;
}
```

<br>

### (2) clearfix Hack을 이용한다

<br>

```html
<header class="main-header clearfix">
    <h1>📘 The Code Magazine</h1>

    <nav>
        <!-- <strong>This is the navigation</strong> -->
        <a href="blog.html">Blog</a>
        <a href="#">Challenges</a>
        <a href="#">Flexbox</a>
        <a href="#">CSS Grid</a>
    </nav>
</header>
```

```css
.clearfix::after {
    clear: both;
    content: "";
    display: block;
}
```

<br>

### (3) Building a Simple Float Layout

-   https://github.com/yoojh9/udemy-css-basics/tree/main/04-CSS-Layouts

<br><br>

## 3) BOX-SIZING: BORDER-BOX

-   slide 67p 참고

<br>

```css
box-sizing: border-box;
```

### (1) box-sizing: border-box 적용 전

```
Final element width = right border + right padding + width + left padding + left border

Final element height = top border + top padding + height + bottom padding + bottom border
```

### (2) box-sizing: border-box 적용 후

```
Final element width = width

Final element height = height
```

<br>

-   box-sizing: border-box 속성은 universal selector에 넣어서 모든 요소에 적용되도록 한다.

<br>

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

<br><br>

---

# 2. FlexBox

## 1) What is FlexBox?

-   Flexbox is a set of related **CSS properties** for **building 1-dimensional layouts**
-   The main idea behind flexbox is that empty space inside a container element can be automatically divided by its child elements
-   Flexbox makes it easy to automatically align items to one another inside a parent container, both horizontally and vertically
-   Flexbox solves common problems such as **vertical certering** and creating **equal-height columns**
-   Flexbox is perfect for replacing floats, allowing us to write fewer and cleaner HTML and CSS code.

<br><br>

## 2) Spacing and Aligning flex items

-   **justify-content**: To align items along main axis (horizontally, by default)
-   **align-items**: To align items along cross axis (vertically, by default)
-   **align-self**: To overwrite align-items for individual flex items
-   https://github.com/yoojh9/udemy-css-basics/commit/b5fd333a4a5d392ee00f68b91e85b99739c1dd65

<br><br>

## 3) The Flex Property

-   **flex-basis**: To define an item’s width, instead of the width property. flex-basis 값 기준으로 브라우저에서 자동으로 크기를 줄일 수 있다. (flex-shrink가 default로 1이기 때문) container에 크기가 충분하지 않으면 flex-basis: 200px;으로 설정하더라도 그보다 적은 너비를 가질 수 있다.

-   **flex-shrink**: To allow an element to shrink (0 means no, 1+ means yes)

-   **flex-grow**: To allow an element to grow (0 means no, 1+ means yes). container 영역에서 차지할 수 있는 만큼 늘어남.

-   **flex**: Recommended shorthand for flex-grow, -shrink, -basis. (ex. flex: 0 1 auto)

-   flex 속성을 사용하는 것을 권장!

<br>

```css
/* DEFAULTS */
flex-grow: 0;
flex-shrink: 1;
flex-basis: auto;
```

<br><br>

## 4) Building a Simple Flexbox Layout

-   https://github.com/yoojh9/udemy-css-basics/commit/2c5c5d5f4ab16ef44618a620ed4c8dde602eceb8

<br><br>

---

# 3. CSS GRID

## 1) Introduction CSS
