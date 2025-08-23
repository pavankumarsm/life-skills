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
This is the first step in the rendering process. The browser received the HTML document, and it resolves the HTML code to create a tree-like structure called DOM.

### 2) Parsing CSS
The browser takes the css code asscoiate with the page and create a separate tree like structure known as CSS object model(CSSOM). it contains all the rules and styles of css

### 3) Constructing the Rendering Tree 
combines DOM and CSSOM create the rendering tree. it representing the elements on the page and styles and also involves only visible elemnets.

  example->  p { color: blue; }
  span { display: none; }  //span remove from rendering tree
             

### 4) Layout
In this step browser calculuate exact position and size of the all elements on the page and also give based on the margins, padding and borders in screen

### 5) Painting 
After complete the layout steps next it moves to the painting step in that step it gives color and creating the text and images for each elements  

### 6) Compositing
The browser combines the all the steps into a final image in the screen this complete the rendering process


### Diagram 
    HTML → DOM
    CSS  → CSSOM
    DOM + CSSOM → Render Tree
    Render Tree → Layout → Paint → Composite → Screen


## Common issues 
1) Conflicting style rules can cause unexpected layouts 
2) It breake the rendering because of invalid structure in HTML and CSS
3) Large image it takes some time to paint


## Optimization Strategies
1) Use efficient CSS selectors 
2) Compress the image 
3) Use dvelopers tools to enhanace the perfromance
4) Write clean and vaild HTML code

## References
* [The Anatomy of Browser Rendering: How Web Pages Come to Life](https://medium.com/@regondaakhil/the-anatomy-of-browser-rendering-how-web-pages-come-to-life-6fa9e801a3f)

* [Understanding Browser Rendering: The Critical Rendering Path](https://www.linkedin.com/pulse/understanding-browser-rendering-critical-path-divyansh-singh)

