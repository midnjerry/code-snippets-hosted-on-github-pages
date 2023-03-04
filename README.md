# code-snippets-hosted-on-github-pages
This project can be used as a reference project when writing your own tutorials, blogs, or code snippets that you would like to host (for free) on GitHub Pages.

## How to Deploy

1. After creating repo - click on Settings
2. Go to Pages (left side)
3. Deploy from branch - Select `main` - select `root`
4. Click save
5. GitHub pages will attempt to build the page based on the content located at the root of the repostiory. It will look for `index.htm` and any corresponding .js and .css files to host.  The hosted link will be located at: `{https://{{username}}.github.io/{{repository-name}}/`
6. Anytime you commit to your `main` branch, GitHub Actions will automatically attempt to build and deploy your site!

## How to use Prism.js

Prism.js is an excellent library that will allow you to display source code stylized as if it were displayed in an IDE.  This is excellent for code snippets, small blogs, or any type of examples you want to showcase!  How to use.

1. Visit the download page at [Prism.js](https://prismjs.com/download.html#themes=prism&languages=markup+css+clike+javascript+git+java+sql)
2. Select the languages you want to support
3. Download `prism.css` and `prism.js`
4. Navigate to the root of your repository and create a `/js` directory and a `/styles` directory.
5. Copy `prism.js` to your `/js` directory and copy `prism.css` to your `/styles` directory.
6. Reference the `prism.css` and `prism.js` files in your index.html

```
<head>
  <script type="text/javascript" src="js/prism.js"></script>
  <link rel="stylesheet" href="styles/prism.css">
</head>
```
Once that's done, you can start adding code snippets using following format:

```
<pre><code class="language-css">p { color: red }</code></pre>
```
If you want to display HTML, then your text will still get rendered.  To get around this, you need to use an escaped string of your HTML.  This encodes your HTML so that it will display as text and not rendered. To do this visit this page:
https://www.freeformatter.com/html-escape.html

Paste your HTML, make an escape string for it, then Copy and Paste that new text into the `<PRE><CODE>` block above.

If you use the `prism.js` and `prism.css` provided in this repo you will also have access to the following languages:

* Markup
* HTML
* XML
* CSS
* C-like
* Javascript
* Java
* SQL

Refer to the download page at [Prism.js](https://prismjs.com/download.html#themes=prism&languages=markup+css+clike+javascript+git+java+sql) to see what other languages are offered!




