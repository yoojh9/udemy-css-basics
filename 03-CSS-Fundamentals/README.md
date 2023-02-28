# CSS Fundamentals

## 1) WHAT IS CSS?

- Cascading Style Sheets
- CSS describes the visual style and presentation of the content writter in HTML
- CSS consists of countless properties that developers use to format the content: properties about font, text, spacing, layout, etc.

<br><br>

## 2) Inline, Internal, and External CSS

### (1) Inline Style

- 인라인 스타일은 절대 사용하지 않는다.

<br>

```javascript
<h1 style="color: blue">📘 The Code Magazine</h1>
```

<br>

### (2) Internal Style

- 좋은 방법이 아니다.

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

- css 파일에 css 코드를 넣어서 분리한다.

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

- font-size
- font-family
- text-transform
- font-style
- line-height: 1.5 -> 높이가 글꼴의 1.5배가 된다는 의미

- \<h1\>이 제일 주요한 제목이라고 해도 \<h2\>보다 커야 한다는 것은 아니다.
