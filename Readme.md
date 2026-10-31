# Session 4: HTML Structure and Text Elements

## 1. Session overview

HTML provides the structure of a web page. In this session, you will create an HTML document and use headings, paragraphs, and lists to build the About Me section of a personal portfolio.

## 2. Learning objectives

- Explain what HTML is used for.
- Create a basic HTML document.
- Use headings, paragraphs, ordered lists, and unordered lists.
- Save an HTML file and open it in a browser.

## 3. Tools and requirements

- VS Code
- A web browser
- Your training folder

## 4. Key concepts

- **HTML:** HyperText Markup Language, used to structure web content.
- **Element:** A piece of HTML, often made of an opening tag, content, and closing tag.
- **Tag:** Markup such as `<p>` or `</p>`.
- **Attribute:** Additional information in an element, such as `lang="en"`.
- **Nesting:** Placing one element inside another.

Headings range from `<h1>` (highest-level heading) to `<h6>` (lowest-level heading). Use them to reflect the structure of your content, not just to make text look large.

## 5. Step-by-step practical

### Step 1: Create your portfolio folder

Create a folder named `my-portfolio` and open it in VS Code.

### Step 2: Create `index.html`

Create a file named `index.html`. Enter this starter document:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
</head>
<body>
  <h1>About Me</h1>
  <p>Hello! My name is [Your Name]. I am learning web development.</p>
</body>
</html>
```

Replace `[Your Name]` with your name, then save the file.

### Step 3: Understand the document

- `<!DOCTYPE html>` tells the browser to use modern HTML.
- `<html lang="en">` contains the page and identifies its language.
- `<head>` contains page information that is not the main visible content.
- `<meta charset="UTF-8">` supports a broad range of characters.
- The viewport meta tag helps the page scale on mobile screens.
- `<title>` sets the browser tab title.
- `<body>` contains the visible page content.

### Step 4: Add headings and paragraphs

Inside the `<body>`, add:

```html
<h1>About Me</h1>
<p>I am a beginner learning how to build websites.</p>

<h2>My Interests</h2>
<p>I enjoy technology, solving problems, and learning new skills.</p>
```

A page should generally have a clear main heading and use lower-level headings for subsections.

### Step 5: Add an unordered list

```html
<h2>My Hobbies</h2>
<ul>
  <li>Reading</li>
  <li>Learning technology</li>
  <li>Listening to music</li>
</ul>
```

`<ul>` creates a bulleted list and each `<li>` is a list item.

### Step 6: Add an ordered list

```html
<h2>My Learning Goals</h2>
<ol>
  <li>Learn HTML</li>
  <li>Learn CSS</li>
  <li>Learn JavaScript</li>
</ol>
```

`<ol>` creates a numbered list.

### Step 7: View the page

1. Save `index.html`.
2. Open the file in your browser, or use a live preview tool if your instructor has installed one.
3. Change a sentence in VS Code, save, and refresh the browser.

**Expected result:** The browser displays your headings, paragraphs, and lists.

## 6. Independent practice

Add these sections to your page:
- A short introduction
- Three interests
- Three learning goals
- A paragraph explaining why you want to learn web development

Use meaningful headings and keep the content appropriate for a public portfolio.

## 7. Common errors and fixes

- **The browser displays HTML tags as text:** Check that the file is saved as `index.html`, not `index.html.txt`.
- **A change is not visible:** Save the file and refresh the browser.
- **An element looks broken:** Check that tags are spelled correctly and nested in the correct order.
- **The page has no visible content:** Confirm that your content is inside `<body>`.

## 8. Deliverables

- `my-portfolio/index.html`
- An About Me section with headings, paragraphs, and both list types

## 9. Knowledge check

1. What is HTML used for?
2. What is the purpose of `<head>`?
3. What is the difference between `<ul>` and `<ol>`?
4. Why is `<h1>` not the same as a paragraph?
5. Why should you save and refresh after editing?

## 10. Completion checklist

- [ ] I created `index.html`.
- [ ] I used headings and paragraphs.
- [ ] I added an unordered list.
- [ ] I added an ordered list.
- [ ] I opened my page in a browser.



