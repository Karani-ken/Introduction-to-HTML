# Session 7: Semantic HTML and Page Layout

## 1. Session overview

Semantic HTML uses elements that describe the purpose of different parts of a page. In this session, you will organize your portfolio using elements such as `header`, `nav`, `main`, `section`, and `footer`.

## 2. Learning objectives

- Explain semantic HTML.
- Identify common semantic elements.
- Refactor a page into meaningful regions.
- Use headings in a logical hierarchy.
- Explain how semantic structure supports accessibility and maintainability.

## 3. Tools and requirements

- Your existing `my-portfolio/index.html`
- VS Code
- A browser

## 4. Key concepts

- `<header>` contains introductory content for a page or section.
- `<nav>` groups major navigation links.
- `<main>` contains the page's primary content. A typical page has one main element.
- `<section>` groups related content, usually with a heading.
- `<article>` represents self-contained content that could stand on its own.
- `<footer>` contains footer information for a page or section.
- `<div>` is a generic container with no inherent semantic meaning.

Semantic elements describe the role of content. They do not automatically make a page visually attractive; CSS is used for styling.

## 5. Step-by-step practical

### Step 1: Review your current HTML

Open `index.html`. Identify your navigation, About, Hobbies, Skills, and Contact content.

### Step 2: Add a page header

Move the page introduction into a `<header>`:

```html
<header>
  <h1>My Portfolio</h1>
  <p>Welcome to my first website.</p>
</header>
```

Avoid keeping multiple unrelated copies of the same main heading.

### Step 3: Keep navigation in a nav element

```html
<nav aria-label="Main navigation">
  <a href="#about">About</a>
  <a href="#hobbies">Hobbies</a>
  <a href="#skills">Skills</a>
  <a href="#contact">Contact</a>
</nav>
```

### Step 4: Group primary content in main

Place your main portfolio sections inside one `<main>` element:

```html
<main>
  <section id="about">
    <h2>About Me</h2>
    <p>Write a short introduction here.</p>
  </section>

  <section id="hobbies">
    <h2>My Hobbies</h2>
    <ul>
      <li>Reading</li>
      <li>Learning technology</li>
    </ul>
  </section>

  <section id="skills">
    <h2>My Skills</h2>
    <!-- Place your skills table here. -->
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <!-- Place your contact form here. -->
  </section>
</main>
```

Move your existing table and form into their matching sections instead of leaving duplicate placeholders.

### Step 5: Add a footer

After `</main>`, add:

```html
<footer>
  <p>&copy; 2026 [Your Name]. Built as a learning project.</p>
</footer>
```

Replace the placeholder with your name. The year can be updated when needed.

### Step 6: Check the overall document

Your page should follow this general order:

```html
<body>
  <header>
    <!-- Site introduction -->
  </header>

  <nav>
    <!-- Navigation links -->
  </nav>

  <main>
    <!-- Main page sections -->
  </main>

  <footer>
    <!-- Footer information -->
  </footer>
</body>
```

This is a structure example, not a complete replacement for your content.

### Step 7: Test your page

1. Save the file.
2. Refresh the browser.
3. Test every navigation link.
4. Confirm each section has a suitable heading.
5. Check that the table, form, and image still appear.

**Expected result:** Your page content remains visible but is now organized into meaningful regions.

## 6. Independent practice

Add a section titled **My Learning Journey** with a paragraph and a list of topics you want to learn. Place it inside `<main>` and give it a unique ID.

## 7. Common errors and fixes

- **Page content disappears:** Check that opening and closing tags match and that content was moved, not deleted.
- **Navigation breaks:** Keep the target section IDs unchanged or update the link destinations.
- **Sections have duplicate IDs:** Each ID should be unique on the page.
- **Everything looks plain:** Semantic HTML describes structure; visual styling will be added with CSS later.
- **Too many main elements:** Use one primary `<main>` element for the page's main content.

## 8. Deliverables

- Portfolio organized with `header`, `nav`, `main`, `section`, and `footer`
- Unique section IDs
- Working navigation

## 9. Knowledge check

1. What does semantic HTML mean?
2. What is the purpose of `<main>`?
3. How is `<section>` different from a generic `<div>`?
4. Why should IDs be unique?
5. Do semantic elements automatically style a page?

## 10. Completion checklist

- [ ] I added a page header.
- [ ] I used a navigation element.
- [ ] I grouped primary content inside main.
- [ ] I used meaningful sections and headings.
- [ ] I added a footer.
- [ ] I tested the page in a browser.
