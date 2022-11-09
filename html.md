## HTML 
- Hyper Text Markup Language
- Created in **1993**


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

#### Heading ELement Exmples
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
##### Output
<p>This is paragraph</p>

---

### Comments in HTML
- Comments in HTML start with ```<!--``` and end with a ```-->```
- Commenting is a way to leave comments for other developers
- Commenting is the convinent way to make code inactive without having to delete it entirely

```html
<h1>This is main Heading</h1>
<h2>This is Sub Heading</h2>
<p>This is paragraph</p>
<!-- This is comment
<h2>This is Second Sub Heading</h2>
-->
<p>This is second paragraph</p>
```
##### Output
<h1>This is main Heading</h1>
<h2>This is Sub Heading</h2>
<p>This is paragraph</p>
<!-- This is comment
<h2>This is Second Sub Heading</h2>
-->
<p>This is second paragraph</p>

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

| Element | Attributes |
| --- | --- |
|```img```|  ```src``` , ```alt```, ```loding```|         



- Images can be added using ```img``` element
- ```src``` attribute is used to point a specific image's URL or image's path
- ```alt``` attribute must be included in ```img``` elements
  - The text inside an ```alt``` attribute is used for screen readers to improve accessibility and is displayed if the image fails to load
  - If the image is purely decorative, using an empty ```alt``` is best practice 
  - Ideally the ```alt``` attribute should not contain special characters unless needed
- Hack to behave image responsive use ```width``` attribute with value ```100%```
- Images can be borrowed online or some online storage
- Base64 can also be used to render the images source
```html
<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.techradar.com%2Fbest%2Ffree-stock-photos&psig=AOvVaw0x6Cr2lmeGbRJGbuYziftM&ust=1668060896024000&source=images&cd=vfe&ved=0CA0QjRxqFwoTCLCCj7O5oPsCFQAAAAAdAAAAABAI" width="100%" alt="A woman taking photos">
```
##### output
<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.techradar.com%2Fbest%2Ffree-stock-photos&psig=AOvVaw0x6Cr2lmeGbRJGbuYziftM&ust=1668060896024000&source=images&cd=vfe&ved=0CA0QjRxqFwoTCLCCj7O5oPsCFQAAAAAdAAAAABAI" width="100%" alt="A woman taking photos">


---


### Self-closing Tag
- A tag without closing tag is known as self-closing tag

|Self-Closing Tags| Purpose |
|---|---|
|```<img/>```| Adding Images |
|```<hr/>```||
|```<br/>```||
|```<link/>```||
|```<input/>```||


---
### Linking to external pages and internal sections in a webpage

```mermaid

graph LR

A[Anchor element]-->B[External Pages]
A[Anchor element]-->C[Internal Sections]

```

| Element | Attributes |
| --- | --- |
|```a```|  ```href``` , ```target="_blank"```,|



- ```a``` *(anchor)* element is used to link external pages and internal sections in a webpage
- ```href``` attribute is used to put the address of the linking page or section 
- ```target``` attribute with value ```_blank``` is used to open the page in new tab
- Anchor text is added in opening and closing tags of an *(anchor)* element 
- The browser displays that text as a link that is clickable
- ```#``` is used with id value to link internal sections in a webpage
- *(anchor)* element can be used within text
```html
<p>This is a paragraph in which <a target="_blank" href="https://github.com/khurramshahzadlali">anchor element</a> is nested</p> 
```
##### Output
<p>This is a paragraph in which <a target="_blank" href="https://github.com/khurramshahzadlali">anchor element</a> is nested</p> 

---

### Scrimba Challenge Example

```html
<h1>Humans have reached Mars</h1>
<img src="https://media-cldnry.s-nbcnews.com/image/upload/t_focal-760x428,f_auto,q_auto:best/mpx/2704722219/2021_10/MarsAFP_9PG3DY-n3pk3j.jpg" width="100%">
<h3>The Starship rocket successfully landed on the red planet this morning.</h3>
<p>After a 115 days long journey, the crew of 12 finally arrived at their destination. This is the first time humans have set foot on a planet other than Earth.</p>
<img src="https://www.universetoday.com/wp-content/uploads/2010/10/manned-mission-mars-illustration.jpg" width="100%">
```
##### Output
<h1>Humans have reached Mars</h1>
<img src="https://media-cldnry.s-nbcnews.com/image/upload/t_focal-760x428,f_auto,q_auto:best/mpx/2704722219/2021_10/MarsAFP_9PG3DY-n3pk3j.jpg" width="100%">
<h3>The Starship rocket successfully landed on the red planet this morning.</h3>
<p>After a 115 days long journey, the crew of 12 finally arrived at their destination. This is the first time humans have set foot on a planet other than Earth.</p>
<img src="https://www.universetoday.com/wp-content/uploads/2010/10/manned-mission-mars-illustration.jpg" width="50%">

---
### Nesting

```html
<div>
  <h1>Humans have reached Mars</h1>
  <img src="https://media-cldnry.s-nbcnews.com/image/upload/t_focal-760x428,f_auto,q_auto:best/mpx/2704722219/2021_10/MarsAFP_9PG3DY-n3pk3j.jpg" width="100%">
  <h3>The Starship rocket successfully landed on the red planet this morning.</h3>
  <p>After a 115 days long journey, the crew of 12 finally arrived at their destination. This is the first time humans have set foot on a planet other than Earth.</p>
  <img src="https://www.universetoday.com/wp-content/uploads/2010/10/manned-mission-mars-illustration.jpg" width="100%">
</div>  
  
```
#### HTML document tree
```mermaid
graph TD

A("&lt;div&gt;")-->B("&lt;div&gt;")
A("&lt;div&gt;")-->C("&lt;div&gt;")
B("&lt;div&gt;")-->D("&lt;img&gt;")
B("&lt;div&gt;")-->E("&lt;h3&gt;")
C("&lt;div&gt;")-->F("&lt;div&gt;")
C("&lt;div&gt;")-->G("&lt;p&gt;")
C("&lt;div&gt;")-->H("&lt;p&gt;")
C("&lt;div&gt;")-->I("&lt;h2&gt;")
H("&lt;p&gt;")-->j("&lt;a&gt;")
```
---

### Intractive Elements 

- ```button```
- ```Input```

```mermaid

graph TD

A[input] --> B(Attribute)
B(Attribute) ----> C[type]
B(Attribute) --> D[placeholder]
C[type] --- E(text)
C[type] --- F(password)
C[type] --- G(date)
C[type] --- H(time)
C[type] --- I(color)
C[type] --- J(file)

```

### Scrimba Challenge Example

```html
<h1>Welcome</h1>
<p>You have been granted access to the platform. 
Please create an account.</p>
<input type="text" placeholder="Enter username">
<input type="password" placeholder="Enter password">
<input type="file">
<button>Sign Up!</button>

```







