### HTML Element
```mermaid

graph TD 

A[HTML Element]--> |look like this| B["&lt;h1&gt;Hello World&lt;/h1&gt;"]
B["&lt;h1&gt;Hello World&lt;/h1&gt;"]-.->|"&lt;h1&gt; is"| C(Opening Tag)
B["&lt;h1&gt;Hello World&lt;/h1&gt;"]-.->|"Hello World is"| D(Opening Tag)
B["&lt;h1&gt;Hello World&lt;/h1&gt;"]-.->|"&lt;/h1&gt; is"| E(Closing Tag)
```
> Note: As a convention, all HTML tags are written in lowercase, for example ```<h1></h1>``` and not ```<H1></H1>```.

---
### Heading Elements

|Heading Type| Heading Element |
|---|---|
|Main Heading| ```h1```|
|Sub Headings|```h2```,```h3```,```h4```,```h5```,```h6```|
>*Note: Higher the Number lower the importance of Heading*
---
### Heading ELement Exmples
|Heading Element| Result |
|---|---|
|```<h1>Hello World</h1>```|<h1>Hello World</h1>|
|```<h2>Hello World</h2>```|<h2>Hello World</h2>|
|```<h3>Hello World</h3>```|<h3>Hello World</h3>|
|```<h4>Hello World</h4>```|<h4>Hello World</h4>|
|```<h5>Hello World</h5>```|<h5>Hello World</h5>|
|```<h6>Hello World</h6>```|<h6>Hello World</h6>|

---
### Paragraph Element 
```p``` element is used for paragraph text on websites, It looks like this:
```html
<p>This is paragraph</p>
```
---
### Comments in HTML
- Comments in HTML start with ```<!--``` and end with a ```-->```
- Commenting is a way to leave comments for other developers
- Commenting is the convinent way to make code inactive without having to delete it entirely
---
### HTML5 Elements 
- HTML5 introduced descriptive elements
- These give descriptive sturcture to HTML 
- These elements help Search Engine Optimiztion(SEO) and accessibility

```mermaid 

graph LR

A(HTML5) ---> B(main)
A(HTML5) ---> C(header)
A(HTML5) ---> D(footer)
A(HTML5) ---> E(nav)
A(HTML5) ---> F(vedio)
A(HTML5) ---> G(article)
A(HTML5) ---> H(section)
A(HTML5) ---> I(other)
```
---
### Adding Images to website 
- Images can be added using ```img``` element
- ```src``` attribute is used to point a specific image's URL or image's path
- ```alt``` attribute must be included in ```img``` elements
  - The text inside an ```alt``` attribute is used for screen readers to improve accessibility and is displayed if the image fails to load
  - If the image is purely decorative, using an empty ```alt``` is best practice 
  - Ideally the ```alt``` attribute should not contain special characters unless needed
---
### Linking to external pages to a website and internal sections in a webpage
- ```a``` *(anchor)* element is used to link external pages to a website and internal sections in a webpage
- ```href``` attribute is used to put the address of the linking page or section 
- Anchor text is added in opening and closing tags of an *(anchor)* element 
- The browser displays that text as a link that is clickable
