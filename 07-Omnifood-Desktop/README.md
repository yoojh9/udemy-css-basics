# OMNIFOOD - Desktop

## 1) The Process behind building a website

### (1) DEFINE the project

- Define **WHO the website is for.** Is it for yourself? For a client of your agency or your freelancing business?
- Define **WHAT the website is for.** In other words, **define business and user goals** of your website project
- Define a **target audience.** Be really specific if possible and if it makes sense for your website (this can come from your client)

<br>

### (2) PLAN the project

- Plan and gather **website content**: copy(text), images, videos etc
- Content is usually **provided by the client,** but you also can help them produce and fine some content
- For bigger sites, plan out the **sitemap:** what pages the site needs, and how they are related to one another
- Based on the content, plan what sections each page needs in order to convey the content's message, and in which order
- Define the **website personality**

<br>

### (3) SKETCH

- Think about what components you need, and how you can use them in layout patterns
- Get ideas out of your head: sketch them with pen and paper or with some design software(e.g. Figma)
- This is an **iterative process**: experient with different components and layouts, until you arrive at a first good solution
- You don't need to sketch everythig, and don't make it perfect. At some point, you're ready to jump into HTML and CSS

<br>

### (4) DESIGN

- Use dicisions, content and sketches from Steps 1, 2, and 3 to design and build the website with HTML and CSS
- Create the design based on selected website personality, the design guidelines
- Use the **client's branding** (if it exists already) for design decisions whenever possible: colors, typography, icons, etc

<br>

### (5) TEST and OPTIMIZE

- Make sure webdsite works well in all major browsers
- Test the website on actual mobile devices, not just in DevTools
- Optimize all images, in terms of dimensions and file size
- Fix simple accessibility problems (e.g. color contrast issues)
- Run the **Lighthouse** performance test in Chrome DevTools and try to fix reported issues
- Think about Search Engine Optimization (SEO)

<br>

### (6) LAUNCH

- Upload your website files to a **hosting platform**. There are countless platform, we will use one with a free plan(Netlify)
- Choose and buy a great domain name, one that represents the brand well, is memorable and easy to write

<br>

### (7) MAINTAIN and UPDATE

- Launching is not the end..
- Keep the website content updated over tieme. If you're working with a client, you can create a montly maintenance contract
- Install **analytics software** (e.g. Google Analytics or Fathom) to get statics about website users. This may inform future changes in the site structure and content.
- A blog that is updated regularly is a good way to keep users coming back, and is also good for SEO.

<br><br>

## 2) RESPONSIVE DESIGN

### (1) What is Reponsive Design?

- Design technique to make a webpace adjust its layout and visual stype to **any possible screen size** (window or viewport size)
- In practice, this means that responsive design makes websites usable on all devices, such as **desktop computers, tablets, and mobile phones.**
- It's a set of practices, not a seperate technology. It's all just CSS!

<br>

### (2) Responsive Design Ingredients

- Fluid Layouts

  - To allow webpage to adapt to the **current viewport** width (or even height)
  - Use % (or vh / vw) unit instead of px for elements that should adapt to viewport (usually layout)
  - Use max-width instead of width

- Resposive Units

  - Use rem unit instead of px for most lengths
  - To make it easy to **scale the entire layout down**(or up) automatically
  - **Helpful trickL** setting 1rem to 10px for easy calculations

- Flexible images

  - By default, images don't scale automatically as we change the viewport. so we need to fix that
  - Always use % for image dimensions, together with the max-width property

- Media Queries

  - Bring resposive sites to life!
  - To change CSS styles on **certain viewport widths**(called breakpoints)

<br><br>
