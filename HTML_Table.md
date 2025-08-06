# 📊 HTML Tables Tutorial: `table`, `tr`, `td`, `th`

## ✅ 1. What is a Table in HTML?

An **HTML table** is used to display data in **rows** and **columns** — just like a spreadsheet.

---

## 🔧 2. Basic Table Structure

```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

---

## 🧩 3. Tag Breakdown

| Tag      | Description |
|----------|-------------|
| `<table>` | Wraps the entire table |
| `<tr>`    | Table **row** (used to group cells horizontally) |
| `<th>`    | Table **header cell** (bold & centered by default) |
| `<td>`    | Table **data cell** |

---

## 🧪 4. Example Table – Student Grades

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Math</th>
    <th>Science</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>90</td>
    <td>85</td>
  </tr>
  <tr>
    <td>Bob</td>
    <td>78</td>
    <td>88</td>
  </tr>
</table>
```

---

## 🎨 5. Optional Styling Tips (CSS)

```html
<style>
  table {
    width: 100%;
    border-collapse: collapse;
  }

  th, td {
    padding: 10px;
    border: 1px solid #333;
    text-align: left;
  }

  th {
    background-color: #f4f4f4;
  }
</style>
```

---

## ✅ Bonus Tips

| Feature        | How to Do It |
|----------------|--------------|
| **Merge Cells Horizontally** | `<td colspan="2">Merged Cell</td>` |
| **Merge Cells Vertically**   | `<td rowspan="2">Merged Down</td>` |
| **Add Caption**              | `<caption>Table Title</caption>` |
| **No Border by Default**     | Add CSS or `border="1"` for quick preview |
