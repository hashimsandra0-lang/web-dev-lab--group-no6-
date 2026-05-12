# 📄 README — Group 06 Web Development Project

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

The objective of this project was to design and build a basic personal/group profile website using fundamental web technologies. The project aimed to demonstrate an understanding of HTML structure, CSS styling techniques, and how the two technologies work together to produce a functional and styled web page.

---

## 📌 What Was Done

The group developed a multi-section static website (`index.html` + `style.css`) that includes:

- **Header section** — Displays the group name and a short description
- **Navigation bar** — Links to the About, Skills, and Daily Routine sections using anchor tags
- **About section** — A brief introduction to the group with an embedded image
- **Skills section** — An unordered list of technical and soft skills learned
- **Daily Routine section** — An ordered list of a typical student's daily schedule

The project also demonstrates three methods of applying CSS:
1. **External CSS** (`style.css`) — Applied globally via a linked stylesheet
2. **Internal CSS** (`<style>` block in the `<head>`) — Used for navigation and section headings
3. **Inline CSS** — Applied directly on individual HTML elements

---

## 📚 What Was Learned

- **HTML Structure:** How to use semantic and non-semantic elements (`<div>`, `<nav>`, `<ul>`, `<ol>`, `<img>`, etc.) to build the skeleton of a webpage
- **CSS Selectors:** Practical use of element selectors, class selectors (`.section`), ID selectors (`#header`), group selectors (`h1, h2, h3`), descendant selectors (`nav ul li a`), and pseudo-classes (`:hover`)
- **Three Ways to Apply CSS:** The difference between inline, internal, and external CSS, and when each is appropriate
- **Box Model Awareness:** Understanding how background colors, spacing, and sizing affect how elements appear on screen
- **Linking Files:** How to properly link an external CSS file to an HTML document using `<link>`
- **Navigation with Anchors:** Using `href="#id"` to create in-page navigation links
- **Image Embedding:** Using the `<img>` tag with `src` and `alt` attributes

---

## ⚠️ Challenges Faced

- **CSS Specificity Conflicts:** Having inline, internal, and external CSS in the same project caused some styles to override others unexpectedly, requiring careful ordering and specificity management
- **Navigation Styling Bug:** The `nav ul li a` descendant selector in the external CSS did not apply because the HTML `<nav>` uses `<a>` tags directly (not nested inside `<ul><li>`), meaning the hover effects and white color rule were non-functional
- **Image Path Issue:** The image referenced in the About section (`Image 17.jpg`) uses a filename with a space, which can cause loading failures on some servers or environments depending on URL encoding
- **Inconsistent Styling Approach:** Mixing inline styles with external and internal CSS made the codebase harder to maintain and debug, particularly when trying to understand which rule was being applied
- **Responsive Design:** The site has no viewport meta tag or responsive CSS, meaning it does not adapt well to different screen sizes or mobile devices

---

## 🛠️ Technologies Used

- HTML5
- CSS3 (External, Internal, and Inline)

---

## 📁 Project Files

```
project/
├── index.html      # Main HTML structure
├── style.css       # External stylesheet
└── Image 17.jpg    # Group photo (referenced in About section)
```

---
