# Browser Rendering

Browser rendering refers to the process by which a web browser converts web page resources, such as HTML, CSS, and JavaScript, into a visual representation that users can see and interact with. Rendering involves parsing and interpreting the web page content, computing the layout and styles, and painting the pixels on the screen.

![here is the icons of HTML,CSS,JS](https://blog.logrocket.com/wp-content/uploads/2021/06/how-browser-rendering-works.png)

## Basic Scenario

you visiting a website for suppose www.google.com now you expect to show up on the screen but what is exactly happend in behind scenes, well the website is stored on the some server when you serach this return back because in the end your browser is an interpretor gets back certain source code to return come back in the second and it can displays on the screen.

## How does the server know.

![screen shot how does the server know](https://digitalmarketingdeal.com/blog/wp-content/uploads/2019/12/What-is-a-server-and-how-does-it-work.jpg)

The server is a computer program or a hardware device that provides services and resources to other computers or clients on a network. In the context of web applications, a server typically refers to a computer program running on a remote machine that handles requests from clients (such as web browsers) and provides responses back.

Here's a simplified overview of how a server works:

### Accepting Connections: 
The server program listens for incoming network connections on a specific port, such as port 80 for HTTP or port 443 for HTTPS. It waits for client requests to establish a connection.

### Handling Requests: 
When a client (e.g., a web browser) sends a request to the server, the server receives the request and processes it. The request typically includes information like the requested resource (e.g., a specific web page URL) and any additional data or parameters.

### Processing Logic: 
The server executes its specific logic to handle the request. This may involve retrieving data from a database, processing the request parameters, performing calculations, or generating a dynamic response.

### Generating a Response: 
Based on the request and the server's processing logic, the server generates an appropriate response. This response typically includes an HTTP status code, headers, and the requested content (e.g., HTML, JSON, images, or files).

### Sending the Response: 
The server sends the response back to the client over the established network connection. It may include the requested content, along with any additional instructions or headers.

### Closing the Connection: 
After sending the response, the server closes the network connection with the client. This frees up server resources and allows it to handle subsequent requests from other clients.

---

*When a browser renders a web page, it goes through several steps to process and display the HTML, CSS, and JavaScript content. The process can be summarized as follows:*

**Parsing HTML**:
The browser starts by parsing the HTML markup of the web page using the HTML parser. It reads the HTML tags and constructs a Document Object Model (DOM) tree, which represents the structure and content of the web page.

**Building the DOM**:As the HTML parser encounters HTML elements, it creates corresponding DOM nodes and organizes them into a tree structure. Each element, attribute, and text node becomes a part of the DOM tree.

**Parsing CSS**: Once the browser has built the initial DOM tree, it starts parsing the CSS stylesheets linked to the page. The CSS parser reads the styles and computes how they affect the elements in the DOM tree, determining their layout, appearance, and positioning.


![html and css snapshot](https://limpet.net/mbrubeck/images/2014/pipeline.svg)



**Layout(or Reflow)**: The browser performs a layout process to determine the position and size of each element on the page. It calculates the dimensions of elements based on the styles, content, and other factors. This step is also known as "reflow" or "layout."

**Painting**: The browser takes the Render Tree and paints the actual pixels on the screen according to the layout and styling information. It creates the visual representation of the web page by painting each element in the appropriate order, applying colors, images, borders, and other visual effects.

**JavaScript Execution**: During the rendering process, if the browser encounters JavaScript code, it can pause rendering and execute the JavaScript. JavaScript can manipulate the DOM, modify styles, handle events, and perform other dynamic actions that may further affect the rendering of the page.

![javascript snapshot from google](https://geekflare.com/wp-content/uploads/2022/01/CLIENT-SIDE-RENDERING.png)


## conclusion:
It's important to note that modern browsers may employ various optimizations, such as incremental rendering, caching, or just-in-time compilation, to improve the overall rendering performance and user experience.

Overall, this step-by-step process of parsing HTML, computing CSS, building the DOM, creating the Render Tree, performing layout, painting, and executing JavaScript allows the browser to render web pages and present them visually to the user.

**For References**:

[youtube link for browser rendering](https://youtu.be/hJHvdBlSxug)

[google link for browser rendering](https://blog.logrocket.com/how-browser-rendering-works-behind-scenes/)