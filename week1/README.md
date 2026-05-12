# 📄 README — Group 06 Multi-Page Website Project

**Institution:** Ardhi University  
**School:** School of Earth Sciences, Real Estate, Business Studies and Informatics (SERBI)  
**Department:** Computer Systems and Mathematics (CSM)  
**Programme:** BSc. Computer Systems and Networks (BSc. CSN 2)  

---

## 👥 Group Members

| S/N | Name | Registration Number | Course |
|-----|------|---------------------|--------|
| 01 | Farijallah, Sandra Hashim | 34258/T.2024 | CSN |
| 02 | Bideberi, Meckzedeck Vedastus | 32470/T.2024 | CSN |
| 03 | Mrema, Felista Salvastori | 33221/T.2024 | CSN |
| 04 | Masaulwa, Kelvin Daimon | 32913/T.2024 | CSN |
| 05 | Antony, Antony Aloyce | 33788/T.2024 | CSN |

---

## 🎯 Objective

The objective of this project was to build a functioning multi-page website using HTML, demonstrating the ability to link multiple pages together through internal navigation, embed images from both local and online sources, and present structured content using lists and hyperlinks. The project specifically focused on understanding how websites are organised across multiple files and how pages communicate with each other.

---

## 📌 What Was Done

A four-page static website was built, with each page sharing a consistent navigation bar:

- **`index.html` (Home)** — The landing page. Contains a welcome message, a list of the site's features, and two embedded images (one from an online URL, one from a local file)
- **`about.html` (About)** — Describes the website's purpose and features, and also embeds the same two images to demonstrate both image sourcing methods
- **`contact.html` (Contact)** — Provides contact details including a clickable email link and a phone number presented in an unordered list
- **`external.html` (External Links)** — Contains links to external websites (Google and GitHub) that open from within the site

**Key techniques demonstrated:**
- Internal linking between pages using relative paths (`href="about.html"`)
- External linking to live websites (`href="https://www.google.com"`)
- Mailto-style contact links (`href="mremafelista118@gmail.com"`)
- Embedding images from online URLs and local files using `<img>`
- Consistent navigation repeated across all four pages
- Proper use of `<!DOCTYPE html>`, `<meta charset>`, and `<meta name="viewport">`

---

## 📚 What Was Learned

- **Multi-Page Site Structure:** How to organise a website across multiple HTML files and link them using relative paths
- **Internal vs External Links:** The difference between linking to pages within the same project and linking out to external websites
- **Image Sources:** How to embed images using both a remote URL (`https://...`) and a local file path (`image_1.jpg`)
- **Anchor Tags (`<a>`):** Practical use of `href` for navigation, external links, and contact links
- **Viewport Meta Tag:** Why `<meta name="viewport" content="width=device-width, initial-scale=1.0">` is important for mobile compatibility — this was applied correctly on all pages
- **Consistent Navigation:** How repeating a `<nav>` block across pages gives users a predictable browsing experience
- **HTML Comments:** Using `<!-- -->` to document and explain sections of code for readability

---

## ⚠️ Challenges Faced

- **Local Image Dependency:** The `image_1.jpg` reference will only work if the image file is physically placed in the same folder as the HTML files. Sharing or uploading the project without including the image will result in a broken image icon
- **No Shared CSS:** All four pages are unstyled — there is no linked stylesheet. While the HTML structure is sound, the pages look bare and inconsistent, which makes the navigation experience feel rough
- **Duplicate `<h1>` on Home Page:** `index.html` has two `<h1>` tags ("my website" and "Welcome"). Semantically, a page should only have one `<h1>` — the main heading. The first one should likely be changed to a `<header>` element or removed
- **No `target="_blank"` on External Links:** Links to Google and GitHub open in the same tab, which takes the user away from the site entirely. Adding `target="_blank" rel="noopener noreferrer"` would open them in a new tab and is standard practice
- **About Page Redundancy:** `about.html` and `index.html` contain largely the same content (same feature list, same images). The About page would be more useful if it described the group or the learning purpose of the project

---

## 🛠️ Technologies Used

- HTML5 

---

## 📁 Project Files

```
project/
├── index.html       # Home page
├── about.html       # About page
├── contact.html     # Contact page
├── external.html    # External links page
└── image_1.jpg      # Local image (must be included for images to load)
```

---
