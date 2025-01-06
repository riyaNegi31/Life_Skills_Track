# Topic: Browser Rendering	

How does a browser render HTML, CSS, JS to DOM? What is the mechanism behind it?

### 1. Browser Reads HTML:
- When you open a webpage, the browser starts by reading the HTML file. 
- This is like the skeleton of the page – it tells the browser what elements (like headings, paragraphs, images) are there.

### 2. Browser Reads CSS:
- Next, it reads the CSS (the style file). 
- CSS is like clothing and makeup – it decides how everything should look: colors, fonts, sizes, spacing, etc.

### 3. Creates a DOM and CSSOM:

- The browser builds a DOM (Document Object Model) from the HTML. 
- Think of it as a family tree of all the elements on the page.
- At the same time, it creates a CSSOM (CSS Object Model) from the CSS to figure out the styles for those elements.

### 4. Combines DOM and CSSOM:
- Now, the browser puts the DOM and CSSOM together to create a Render Tree. 
- This is like a visual map of what should be shown on the screen and how it should look.

### 5. Lays Everything Out:
- The browser figures out where everything goes on the page – for example, "This image goes here, this text goes next to it." 
- This step is called Layout.

### 6. Paints the Screen:
- Once the layout is ready, the browser starts painting – it fills in the colors, draws the text, images, shadows, etc. 
- It’s like colouring in the sketch.

### 7. Final Touch (Compositing):
- For complex pages with layers (like animations or overlapping elements), the browser organizes them into layers and combines them to display the final picture on your screen.

### Why Some Pages Load Slowly:
If JavaScript is in the middle, the browser pauses and waits to execute it. This can delay things.
CSS has to finish loading before the page can be styled, so incomplete CSS can hold up rendering.

#### In short:
### HTML → Structure → Style → Layout → Paint → Display.

It’s like building a house: you start with the structure, decorate it, decide where the furniture goes, and finally, you move in and enjoy it! 🏡

### References
#### Online Articles and Resources:
- [Browser Rendering by Medium](https://engineering.teknasyon.com/what-is-the-dom-how-does-html-rendering-happen-in-browsers-cbeb12bdfea6)
- [Renders the Pages with DOM CSSOM by xenonstack](https://www.xenonstack.com/blog/web-browser-renders)
