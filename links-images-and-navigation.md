# Session 5: Links, Images and Navigation

## 1. Session overview

In this session, you will make your portfolio more useful by adding links, a profile image, and a navigation menu that helps visitors move to sections of the page.

## 2. Learning objectives

- Create links with `<a>`.
- Display images with `<img>`.
- Use meaningful alternative text.
- Create in-page navigation using IDs.
- Organize project assets in an `images` folder.

## 3. Tools and requirements

- Your `my-portfolio` folder and `index.html` from Session 4
- VS Code
- A browser
- A profile image you have permission to use

## 4. Key concepts

- **Hyperlink:** A clickable link to another page, file, email address, or location.
- **`href`:** The destination of a link.
- **Image source (`src`):** The location of an image file.
- **Alternative text (`alt`):** A text alternative for people who cannot see the image or when the image fails to load.
- **ID:** A unique identifier that can be used as an in-page link destination.

## 5. Step-by-step practical

### Step 1: Organize your files

Inside `my-portfolio`, create a folder named `images`. Place a suitable image in it and rename the image `profile.jpg` if it is actually a JPEG file. Do not simply change the extension if the image is a different format.

Your project should look like:

```text
my-portfolio/
├── index.html
└── images/
    └── profile.jpg
```

### Step 2: Add a navigation menu

Inside `<body>`, below the opening body tag, add:

```html
<nav>
  <a href="#about">About</a>
  <a href="#hobbies">Hobbies</a>
  <a href="#contact">Contact</a>
</nav>
```

The `#about`, `#hobbies`, and `#contact` values point to elements with matching IDs.

### Step 3: Add matching section IDs

Update your content so the links have matching destinations:

```html
<section id="about">
  <h1>About Me</h1>
  <p>Hello! I am learning web development.</p>
</section>

<section id="hobbies">
  <h2>My Hobbies</h2>
  <ul>
    <li>Reading</li>
    <li>Learning technology</li>
    <li>Listening to music</li>
  </ul>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>You can contact me using the link below.</p>
</section>
```

For now, `<section>` is simply a way to group related content. You will study semantic page layout in a later session.

### Step 4: Add your profile image

Inside the About section, add:

```html
<img src="images/profile.jpg" alt="Profile photo of [Your Name]" width="200">
```

Replace the name in the `alt` text. If the image is purely decorative, use an empty `alt=""`; for a meaningful profile photo, describe its purpose.

### Step 5: Add an external link

Add a link to a useful learning resource:

```html
<p>
  I am learning from
  <a href="https://developer.mozilla.org/">MDN Web Docs</a>.
</p>
```

For a link that opens in a new tab, use `target="_blank"` together with `rel="noopener noreferrer"`. Do not add a new-tab target unless it is useful.

### Step 6: Test every link and the image

1. Save the HTML file.
2. Open or refresh it in your browser.
3. Click each navigation link.
4. Click the external link.
5. Confirm that the image loads.

**Expected result:** Navigation moves to the correct section, the external link opens, and the profile image is visible.

## 6. Independent practice

Add a link to one learning resource and one email link using a placeholder address, for example:

```html
<a href="mailto:student@example.com">Email me</a>
```

Replace the placeholder only if you want to publish your real contact address. Be thoughtful about personal information on a public website.

## 7. Common errors and fixes

- **Image is broken:** Check spelling, capitalization, extension, and relative path. `images/profile.jpg` is different from `Images/Profile.jpg` on many web servers.
- **Navigation does not move:** Check that the `href="#about"` value exactly matches `id="about"`.
- **External link does not open:** Check that the URL includes `https://`.
- **Image looks too large:** Adjust the `width` attribute for this exercise. Later you will learn more flexible styling with CSS.

## 8. Deliverables

- Navigation with three working in-page links
- One profile image with appropriate alternative text
- At least one working external link

## 9. Knowledge check

1. What does `href` specify?
2. What does `src` specify in an image element?
3. Why is useful `alt` text important?
4. How does an in-page link find its destination?
5. Why should you be careful about publishing personal contact details?

## 10. Completion checklist

- [ ] I created an `images` folder.
- [ ] I added a profile image.
- [ ] I added appropriate `alt` text.
- [ ] I created navigation links.
- [ ] I tested the links in the browser.
