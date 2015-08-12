# Introduction to HTML & CSS
Let's build a website.

## Setting up tools
- [GitHub](https://github.com/)

  Create a free personal account and download the desktop app for your computer. ([Windows](https://windows.github.com/) or [Mac OS X](https://mac.github.com/))

- [Atom](https://atom.io/)

  Download and install this text editor to be able to edit source code files.

## Fork this repository
On the GitHub page of the [cbas/html-css-intro](https://github.com/cbas/html-css-intro) repository, press the **Fork** button.

![Fork button](https://i.imgur.com/jkmFr8q.png)

Forking creates your own copy of this code to set up your own website.

The fork will be available at: <https://github.com/YOUR_GITHUB_USERNAME/html-css-intro>

Any changes you make to your copy will not affect anyone else's not the original repository.

*Note: Forking is specific to the GitHub service and not part of the underlying Git source code manager. Git itself has a concept of branching which is similar but branches exist only within a copy of the repository.*

## Hack the code
Use Atom to edit the HTML and CSS files. In the GitHub app, right click on the repository bookmark, and choose "Open in Atom."

![Open in Atom](https://i.imgur.com/8Q5mOR0.png)

### Content authoring
The file `index.html` contains the page content in HTML format. Text, links, images, navigation, videos, widgets, etc.

*Tip: Start by writing the content as plain text. You can even use [Markdown](https://help.github.com/articles/github-flavored-markdown/), just like this file.*

### Structuring the document
Use semantic HTML tags to describe the content semantically, that is, using tags that capture the meaning of the content.

Semantic markup matter helps browsers and bots (i.e. search engines, social media) understand the site. It also makes it easier to style the page.

Reference: https://developer.mozilla.org/en/docs/Web/HTML/Element

### Design and layout
With a CSS the page content can be styled. A stylesheet is a set of rules, which consist of a selector and a declaration of properties with values.

```css
h1 {
  font-size: 36pt;
  font-weight: bold;
  color: purple;
}
```

Use your browser's developer tools to inspect any website. This is a great way to learn how interesting effects can be achieved. Remember, great artists steal.

![Inspect Element](https://i.imgur.com/nGLXgh0.png)

#### Selectors
Use selectors to precisely target the content that needs to be styled. The most specific selector overrides lesser ones.

To keep your CSS code clean, try to avoid overly generic selectors that affect many elements.

Use one or more classes or a single ID on elements to make them easier to target using CSS selectors.

Reference: https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_started/Selectors

```html
<p>This should be blue.</p>
<p class="sidenote">This should be red.<p>
<p class="sidenote" id="summary">This should be green.</p>
```

```css
p          { color: blue; }  /* applies to all p tags */
p.sidenote { color: red; }   /* overrides the second and third */
p#summary  { color: green; } /* overrides only the third */
p:hover    { color: gold; }  /* overrides on mouse over */
```

#### Properties
Control the visual design of elements using their many properties.

Reference: https://developer.mozilla.org/en-US/docs/Web/CSS/Reference

```css
color
background-image
font-family
width
height
padding
margin
...
```

#### Values
Depending on the property, values can be specified in different units. E.g. lengths, time, angles, colours, strings, URLs, etc.

```css
12px
500ms
url('cat.jpg')
...
```

## Publish your website
Commit & Push your changes to GitHub. Because they are on the `gh-pages` branch they will automatically be published on GitHub Pages.

Visit your page at: <https://YOUR_GITHUB_USERNAME.github.io/html-css-intro>

## Next Steps

### Change the URL path of your website
By renaming the repository or registering a unique domain name you can [publish the website at a custom URL](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages/).

### Split the page into multiple files
Splitting a growing code base into multiple smaller files is a great way to manage medium and larger sized projects.
- **HTML:** Use the *anchor* tag to link from one page to another.
  ```html
  <a href="about.html">About Us</a>
  ```
- **CSS:** Use the `@import` at-rule to reference other files.
  ```css
  @import url('widgets.css')
  ```

### Explore the Jekyll static site generator
GitHub Pages has a powerful content management system (CMS) called [Jekyll](http://jekyllrb.com/). Use it to create more complex pages with auto-generated content, templates, themes, etc.

### Add interactive behaviour to the page
Using a programming language called JavaScript we can add rich functionality to the document, even turning it into a full fledged single page application.

### Learn more with General Assembly
Sign up for the [Programming for Non Programmers (PFNP)](https://generalassemb.ly/education/programming-for-non-programmers/singapore) course at General Assembly Singapore.

### Ask me a question about this class
Create, browse, or comment on the [GitHub issues for this repository](https://github.com/cbas/html-css-intro/issues).

### Join our awesome local web developers community
- Free and open meetups

  https://webuild.sg/

- Chat room

  https://gitter.im/SingaporeJS/discussions

- Communities

  http://www.zell-weekeat.com/devfest/dist/community.html
