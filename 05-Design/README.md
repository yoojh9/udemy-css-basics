# Web Design Rules and Framework

## 1) Overview of Web Design and Website Personalities

### (1) Web Design Ingredients

- Typography
- Colors
- Images/Illustrations
- Icons
- Shadows
- Border-radius
- Whitespace
- Visual Hierarchy
- User Experience
- Components/Layout

<br><br>

## 2) WEB DESIGN RULES #1: TYPOGRAPHY

### (1) SERIF vs SANS-SERIF

- **serif**

  - serif는 좀 더 전통적인 형태라서 전통적이거나 고전적인 느낌을 줄 수 있음
  - Creates a traditional / classic look and feel
  - Conveys trustworthiness
  - Good for long text

- **sans-serif**
  - sans-serif는 좀 더 깔끔해 보인다.
  - Modern look and feel
  - Clean and simple
  - Easier to choose for beginner designer

<br>

### (2) Use Good Font Size and Weights

- Use only good and popular typefaces and play it safe
- It's okay to use just one typeface per page! If you want more, limit to 2 typefaces.
- Choose the right typeface according to our website personality
- When choosing font-sizes, limit choices! Use a **"type scale"** tool or other pre-defined range
- Use a font size between 16px and 32px for "normal" text
- For long text (like a blog post), try a size of 20px or even bigger
- For **headlines**, you can go really big(50px+) and bold(600+), depending on personality
- For any text, don't use a font weight under 400 (regular)

<br>

### (3) Create a Good Reading Experience

- Under less than 75 characters per line
- For normal-sized text, use a line height between 1.5 and 2. For big text, go below 1.5
- Decrease letter spacing in headlines, if it looks unnatural(this will come from experience)
- Experiment with all caps for short titles. Make them small and bold and increase letter-spacing
- Don't center long text blocks. Small blocks are fine

<br>

### (4) Tools

- google fonts: https://fonts.google.com/
- Type Scale: https://typescale.com/

<br>

### (5) Implementing Typography

- https://github.com/yoojh9/udemy-css-basics/tree/main/05-Design

<br><br>

## 3) WEB DESIGN RULES #2: COLORS

### (1) Choose the Right Color

- Make the main color match your website's personality: colors convey meaning!
- Use a good color tone! Don't choose a random tone or CSS named colors
- You need at least two types of colors in your color palette: a **main color** and a **grey color**
- With more experience, you can add more colors: **accent(secondary) colors** (use a tool)
- For diversity, create ligher and darker "versions" **(tint and shades)**

<br>

### (2) When and How to use Colors

- Use your main color to draw attention to the most important elements on the page
- Use colors to add interesting accents or make entire components or sections stand out
- You can try to use your colors strategically in images and illustrations

<br>

### (3) Colors and Typography

- On dark colored backgrounds, try to use a tint of the background("light version") for text
- Text should usually not be completely black. Lighten if up it looks heavy and uninviting.
- **Don't make text too light!** Use a tool(ex.Coolors) to check contrast between text and background colors
  - Contrast ratio need to be at least **4.5:1 for normal text** and **3:1 for large text**(18px+)

<br>

### (4) Tools

- Open Color: https://yeun.github.io/open-color/
- Tailwind CSS: https://tailwindcss.com/docs/customizing-colors
- Flat UI Colors 2: https://flatuicolors.com/
- Tint & Shade Generator: https://maketintsandshades.com/
- Paletton: https://paletton.com
- Coolors: https://coolors.co/

<br>

### (5) Implementing Colors

- Coolors로 Color Contrast를 체크할 수 있다 (https://coolors.co/contrast-checker)
- https://github.com/yoojh9/udemy-css-basics/commit/ff20407b47699cd436eef4546ae957c28d251686

<br><br>

## 4) WEB DESIGN RULES #3: Images and Illustrations

### (1) Use Good Images

- Different types of images: product photos, storytelling photos, illustrations, patterns
- Use images to support your website's message and story. So only use relevant images!
- Prefer original images. If not possible, use original-looking stock images(not generic ones!)

<br>

### (2) Use Images Well

- Try to show real people to trigger user's emotions
- if necessary, crop images to fit your message
- Experiment combining photos, illustrations and patterns

<br>

### (3) Handling Text On Images

- Method #1: Darker or brighten image (completely or partially, using a gradient)
- Method #2: Position text into neutral image area
- Method #3: Put text in a box

<br>

### (4) Some Technical Details

- To account for high-res screens, make image dimensions 2x as big as their displayed size
  - **scale factor**: Actual pixels the screen contains / Pixels represented on screen
  - On high-res screens, scale factor is 2x or even 3x, on "normal" screens it's just 1x (1 physical pixel = 1 design pixel)
- 고해상도 스크린을 위해 이미지는 300 x 300px로 보여진다 하더라도 이미지 원본은 600 x 600px의 이미지를 사용해야 한다.
- Compress image for a lower file size and better performance (squoosh를 이용해 96%까지 이미지를 줄일 수 있다)
- When using multiple images side-by-side, make sure they have the **exact same dimensions** (이미지 가로, 세로 길이가 같은지 최소한 가로 세로 비율이 같은지 확인 필요)

<br>

### (5) Tools

- Use images from (for free)
  - Unsplash: https://unsplash.com/ko
  - Pexels: https://www.pexels.com/ko-kr/
  - DrawKit: https://www.drawkit.com/
  - UnDraw: https://undraw.co/
  - Squoosh: https://squoosh.app/

<br><br>

## 5) WEB DESIGN RULES #4: Icons

### (1) Use Good Icons

- Use a good icon pack, there are tons of free and paid icons packs
- Use only one icon pack. Don't mix icons from diffrent icon packs.
- Use SVG icons or icon fonts. Don't use bitmap image formats (.jps and .png)
  - Vector-based: SVG images and icon fonts. Scale indefinitely!
  - Bitmap: Regular images (JPG, PNG, GIF), Do not scale, become unsharp!
- Adjust to website personality! Roundeness, weight and filled/outlined depend on typography

<br>

### (2) When to use Icons

- Use icons to provide visual assistance to text
- Use icons for product feature blocks
- Use icons associated with actions, and label them
- Use icons as bullet points

<br>

### (3) Use Icons Well

- To keep icons neutral, **use same color as text**. To draw more attention, use different color
- Don't confuse your users: icons need to make sense and fit the text or action!
- Don't make icons larger than what they were designed for. if needed, enclose them in a shpace.

<br>

### (4) Tools

- Phosphor icons: https://phosphoricons.com/
- ionicons: https://ionic.io/ionicons
- Icons8: https://icons8.com/
