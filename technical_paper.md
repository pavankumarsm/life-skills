# Browser Rendering 

When you access a webpage in your browser, the process starts. It includes servers that convert the page's code into a visual display on your screen is known as Browser Rendering are also called as Critical Rendering.

The steps invloved are:
1. Parsing HTML 
2. Parsing CSS
3. Constructing the rendering tree
4. layout
5. Painting
6. Compositing 

### 1) Parsing HTML 
This is the first step in the rendering process. The browser received the HTML document, and it resolves the HTML code to create a tree-like structure called DOM..

### 2) Parsing CSS
The browser takes the CSS code associated with the page and creates a separate tree-like structure known as CSS Object Model (CSSOM). It contains all the rules and styles of CSS.

### 3) Constructing the Rendering Tree 
Combines DOM and CSSOM create the rendering tree. It representing the elements on the page and styles and also involves only visible elements.

  example->  p { color: blue; }
  span { display: none; }  //span remove from the rendering tree
             

### 4) Layout
In this step browser calculates exact position and size of all elements on the page and also give based on the margins, padding and borders in screen.

### 5) Painting 
After completing the layout steps next it moves to the painting step in that step it gives color and creating the text and images for each element. 

### 6) Compositing
The browser combines all the steps into a final image in the screen this completes the rendering process.


### Diagram 
    HTML → DOM
    CSS  → CSSOM
    DOM + CSSOM → Render Tree
    Render Tree → Layout → Paint → Composite → Screen


## Common issues 
1) Conflicting style rules can cause unexpected layouts
2) It breaks the rendering because of invalid structure in HTML and CSS
3) Large image it takes some time to paint


## Optimization Strategies
1) Use efficient CSS selectors 
2) Compress the image 
3) Use developers tools to enhance the performance
4) Write clean and valid HTML code

## References
* [The Anatomy of Browser Rendering: How Web Pages Come to Life](https://medium.com/@regondaakhil/the-anatomy-of-browser-rendering-how-web-pages-come-to-life-6fa9e801a3f)

* [Understanding Browser Rendering: The Critical Rendering Path](https://www.linkedin.com/pulse/understanding-browser-rendering-critical-path-divyansh-singh)

