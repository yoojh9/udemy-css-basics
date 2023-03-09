# Components and Layout Pattern

## 1) Elements and Components

### (1) From elements to Webpage

- Element -> Components -> Layouts -> Webpage
- Use common elements and components to convey your website's information
- Combine components into layouts using **common layout patterns**
- Assemble diffrent layout areas into a complete, final page

<br>

### (2) Elements

- Text
- Button
- Images
- Input elements
- Tags

<br>

### (3) Components

- Breadcrumbs (ex. Development > Web Development > Javascript)
- Pagination
- Alert and Status bar
- Statistics
- Gallery
- Feature box
- Preview and Profile card
- Accordion
- Tabs
- Carousel
- Customer Testimonials
- Customer Logos
- Steps
- Forms
- Tables
- Pricing Tables
- Modal Windows

<br><br>

## 2) Building an Accordion component

### (1) Switching Flex-Direction to Column

- Main Axis가 가로 방향에서 세로 방향으로 변함.
- with flex-direction set to **COLUMN :**
  - align-items aligns items **horizontally**, no longer vertically
  - justify-content aligns items **vertically**, no longer horizontally
  - gap acts like **margin-bottom**, no longer like margin-right

<br>

```css
.accordion {
  display: flex;
  gap: 24px;
  flex-direction: column;
}
```

<br>

- https://github.com/yoojh9/udemy-css-basics/commit/10c858f7ba4e884e4e69b23ff8a7cfbea04d9d39
