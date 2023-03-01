# CSS Fundamentals

## 1) WHAT IS CSS?

-   Cascading Style Sheets
-   CSS describes the visual style and presentation of the content writter in HTML
-   CSS consists of countless properties that developers use to format the content: properties about font, text, spacing, layout, etc.

<br><br>

## 2) Inline, Internal, and External CSS

### (1) Inline Style

-   인라인 스타일은 절대 사용하지 않는다.

<br>

```javascript
<h1 style="color: blue">📘 The Code Magazine</h1>
```

<br>

### (2) Internal Style

-   좋은 방법이 아니다.

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>The Basic Language of the Web: HTML</title>

        <style>
            h1 {
                color: blue;
            }
        </style>
    </head>
</html>
```

<br>

### (3) External Style

-   css 파일에 css 코드를 넣어서 분리한다.

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>The Basic Language of the Web: HTML</title>
        <link rel="stylesheet" href="style.css" />
    </head>
</html>
```

<br><bR>

## 3) Style Text

-   font-size
-   font-family
-   text-transform
-   font-style
-   line-height: 1.5 -> 높이가 글꼴의 1.5배가 된다는 의미

-   \<h1\>이 제일 주요한 제목이라고 해도 \<h2\>보다 커야 한다는 것은 아니다.

<br><br>

## 4) Combining Selectors

-   footer 태그 하위에 있는 모든 p 태그를 선택

<br>

```css
footer p {
}
```

<br><br>

## 5) Class and Id Selectors

-   id selector는 중복해서 사용할 수 없다. 하나의 요소에 하나의 id만 사용해야 함

<br>

```css
#author {
    font-style: italic;
    font-size: 18px;
}

#copyright {
    font-size: 16px;
}
```

<br>

-   따라서 이름을 재사용해야 한다면 클래스를 사용한다.
-   보통은 확장성을 위해 id를 사용하지 않고 항상 클래스를 사용한다.

<br>

```css
.related-author {
    font-size: 18px;
    font-weight: bold;
}

.related {
    list-style: none;
}
```

<br><br>

## 6) Working with Colors

### (1) RGB

-   Every color can be represented by a combination of RED, GREEN, and BLUE
-   Each of the 3 bas colors can take a value between 0 and 255, which leads to 16.8 million different colors

<br>

### (2) Defining Colors in CSS

-   RGB / RGBA Notation

    -   Regular RGB Model: rgb(0, 255, 255), rgb(244, 179, 63)
    -   RGB with transparency ("alpha"): rgba(0, 255, 255, 0.3), rgba(244, 179, 63, 0.7)

-   HEXADECIMAL Notation
    -   Instead of using a scale from 0 to 255, we go from 0 to ff (255 in hexadecimal numbers)
    -   #00ffff, #0ff
    -   In practice, we mostly use **hexadecimal** colors, and **rgba** when we need transparency

<br>
