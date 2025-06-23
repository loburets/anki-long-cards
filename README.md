# 📚 Anki Styles for Long or Complex Cards

This project provides a CSS style for Anki cards that display **long content**, including code snippets, tables, headers, lists, and more.  

The goal is to make such content **easier to read, cleaner, and more compact**. So you can add any content you want, including ChatGPT generated.

---

## ✨ What It Does

This CSS:

- Shrinks font sizes for better information density
- Improves list and blockquote indentation
- Adds borders to table cells
- Makes `<code>` elements look nice and readable
- Prevents overflow by forcing normal text wrapping

Perfect for flashcards with:

- 📜 Long text explanations  
- 🧾 Tables and structured data  
- 🧠 Programming code or configuration  
- 🧩 Multi-level lists and headers  

---

## 🔍 Before / After

| ❌ Default Style | ✅ With Compact Styles |
| :-------------: | :-------------------: |
| ![Before](assets/before.png) | ![After](assets/after.png) |

> Replace the `assets/` images with your own screenshots to show the difference.

---

## 🛠️ How to Use

1. **Open Anki** → go to your deck → click **Browse**
2. Select a card → click **Cards…** to edit the card template
3. Switch to the **Styling** tab
4. Paste the CSS below **at the very top** of the style area
5. Save and preview a card

---

## 🎨 CSS Code

Paste the following into the Styling section of your card template:

```html
<style>
  li, div, code, span, th, td, blockquote,
  h1, h2, h3, h4, h5 {
    /* 
      NOTE!
      YOU CAN UPDATE NUMBER BELOW UP TO YOUR TASTE
      FOR EXAMPLE SET 0.5rem IF YOU USE
      INCREASED SCALE
    */
    font-size: 1.2rem;
    text-align:left;
    white-space: normal;
  }
  td, th {
    border-right: solid 1px black;
    border-bottom: solid 1px black;
  }
  /* Top border for the first row */
  tr:first-child td,
  tr:first-child th {
    border-top: 1px solid black;
  }
  /* Left border for the first column */
  td:first-child,
  th:first-child {
    border-left: 1px solid black;
  }
  table {
    padding: 1rem 0.5rem;
  }
  code {
   background: #eee;
   color: darkred;
   padding: 2px;
   white-space: pre-wrap;
  }
  ol, ul, li {
    /* adjust too large indents for bullets */
    padding-left: 1em;
    text-indent: -1em;
  }
  blockquote {
    padding: 0.5em 1em;
    margin-left: 0.3em;
    font-style: italic;
    background-color: #f9f9f9;
    border-left: 3px solid #ccc;
  }
</style>

<!-- Optional preview block -->
<div>
  Paste your content here
</div>
```
