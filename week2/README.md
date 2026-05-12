# 📄 README — Group 06 Student Portal Project

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

The objective of this project was to build a structured, multi-page Student Portal website using HTML, with a focus on advanced HTML elements such as tables (including `rowspan` and `colspan`), forms with multiple input types, and consistent site-wide navigation. The project aimed to demonstrate how real-world web pages present structured data and collect user input.

---

## 📌 What Was Done

A three-page Student Portal website was built, all sharing a common navigation bar:

- **`index.html` (Home)** — The landing page. Introduces the portal with a welcome message, an ordered list of the student's daily routine, and an unordered list of hobbies
- **`timetable.html` (Timetable)** — Displays a full weekly class schedule in an HTML table with `rowspan` for double periods (e.g., Science on Monday, History on Friday, ICT on Tuesday) and `colspan` for break rows (Short Break, Lunch Break) that span all five day columns
- **`contact.html` (Contact & Register)** — Contains two forms:
  - **Part A:** A basic contact form with name, email, and message fields
  - **Part B:** A student registration form laid out inside an HTML table, using text, email, password, radio button (gender), and checkbox (courses) input types

---

## 📚 What Was Learned

- **HTML Tables:** How to build complex tables using `<table>`, `<thead>`, `<tbody>`, `<th>`, `<tr>`, and `<td>`; how `rowspan` merges cells vertically for double periods, and `colspan` merges cells horizontally for full-row breaks like lunch
- **HTML Forms:** How to build forms using `<form>`, `<input>`, `<textarea>`, `<label>`, and `<button>`; the difference between `type="text"`, `type="email"`, `type="password"`, `type="radio"`, and `type="checkbox"`
- **Form Validation Attributes:** Using `required` on inputs to enforce that fields are filled before submission, and `placeholder` to guide the user
- **Table-Based Form Layout:** Using a `<table>` inside a `<form>` to align labels and inputs neatly in two columns (Part B of contact page)
- **Multi-Page Navigation:** Maintaining a consistent `<nav>` with internal links across all three pages, including marking the current page with `class="active"` for potential CSS styling
- **Semantic Structure:** Using `<h1>` for the main page heading, `<h2>` for subsections, and meaningful `<label>` elements associated with form inputs
- **`<small>` Tag:** Used inside table cells to add sub-labels like "(Double)" or "(double)" to indicate double periods without disrupting the layout

---

## ⚠️ Challenges Faced

- **Unclosed `<h2>` Tag in `index.html`:** The nav header is written as `<h2>Student Portal<h2>` — the closing tag is missing the forward slash. It should be `</h2>`. This causes the browser to silently try to auto-correct it, but the result is unpredictable
- **`rowspan` Alignment in Timetable:** Correctly counting which cells to omit in subsequent rows when using `rowspan` is easy to get wrong. For example, the 08:15–09:00 row on Monday is missing its `<td>` because the Mathematics cell above spans two rows — this was handled correctly, which shows careful attention to table structure
- **No CSS Applied:** All three pages are unstyled. The timetable in particular would benefit significantly from CSS — alternating row colours, border styling, and font sizing would make it far more readable. The `border="2"` attribute used on the table is an outdated HTML 4 approach; modern practice is to handle borders in CSS
- **`align="center"` is Deprecated:** Used on the break rows in the timetable (`align="center"`), this attribute was removed in HTML5. The correct approach is `style="text-align: center"` or a CSS class
- **Stray `</span>` Tag:** In `timetable.html`, the lunch break row contains a stray `</span>` closing tag with no matching opening tag — a small but real markup error
- **Forms Have No `action` Attribute:** Both forms in `contact.html` have no `action` attribute, meaning submissions go nowhere. For a real project, `action` should point to a server-side handler or a service like Formspree
- **Inconsistent Capitalisation:** "kiswahili" is written in lowercase throughout the timetable while all other subjects are capitalised — it should be "Kiswahili"

---

## 🛠️ Technologies Used

- HTML5 
---

## 📁 Project Files

```
project/
├── index.html        # Home page — daily routine and hobbies
├── timetable.html    # Weekly timetable with rowspan and colspan
└── contact.html      # Contact form (Part A) and Registration form (Part B)
```

---
