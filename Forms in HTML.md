
# 📝 HTML Forms Tutorial

Learn how to use `input`, `textarea`, `label`, `select`, and `button` to create interactive forms in HTML.

---

## 📦 Basic Form Structure

```html
<form action="/submit" method="POST">
  <!-- form elements go here -->
</form>
```

- `action`: URL to send the data
- `method`: usually `POST` or `GET`

---

## 🔹 1. `<input>` — Single-line Fields

```html
<input type="text" placeholder="Your Name" />
<input type="email" placeholder="Email Address" />
<input type="password" placeholder="Password" />
<input type="checkbox" /> I agree
<input type="radio" name="gender" value="male" /> Male
<input type="radio" name="gender" value="female" /> Female
<input type="submit" value="Submit" />
```

- Use `type` attribute to change input behavior

---

## 🔹 2. `<textarea>` — Multi-line Input

```html
<textarea rows="4" cols="50" placeholder="Your message here..."></textarea>
```

- Use `rows` and `cols` to control size

---

## 🔹 3. `<label>` — Accessible Labels

```html
<label for="email">Email:</label>
<input type="email" id="email" />
```

- `for` matches the input’s `id`
- Clicking the label focuses the input

---

## 🔹 4. `<select>` and `<option>` — Dropdown Menus

```html
<label for="country">Country:</label>
<select id="country">
  <option value="usa">USA</option>
  <option value="uk">UK</option>
  <option value="canada">Canada</option>
</select>
```

---

## 🔹 5. `<button>` — Action Buttons

```html
<button type="submit">Submit</button>
<button type="button" onclick="alert('Hello!')">Click Me</button>
```

- `type="submit"` triggers form submission
- `type="button"` is used for custom scripts

---

## ✅ Full Example: Contact Form

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contact Form</title>
</head>
<body>

  <h2>Contact Us</h2>

  <form action="/submit-form" method="POST">

    <!-- Name -->
    <label for="name">Full Name:</label><br />
    <input type="text" id="name" name="name" placeholder="Enter your full name" required /><br /><br />

    <!-- Email -->
    <label for="email">Email Address:</label><br />
    <input type="email" id="email" name="email" placeholder="example@mail.com" required /><br /><br />

    <!-- Gender -->
    <label>Gender:</label><br />
    <input type="radio" id="male" name="gender" value="male" />
    <label for="male">Male</label>
    <input type="radio" id="female" name="gender" value="female" />
    <label for="female">Female</label><br /><br />

    <!-- Country -->
    <label for="country">Country:</label><br />
    <select id="country" name="country">
      <option value="usa">USA</option>
      <option value="uk">UK</option>
      <option value="canada">Canada</option>
    </select><br /><br />

    <!-- Message -->
    <label for="message">Message:</label><br />
    <textarea id="message" name="message" rows="4" cols="40" placeholder="Write your message here..."></textarea><br /><br />

    <!-- Terms -->
    <input type="checkbox" id="agree" name="agree" required />
    <label for="agree">I agree to the terms and conditions</label><br /><br />

    <!-- Submit -->
    <button type="submit">Send Message</button>

  </form>

</body>
</html>
```

---

## 💡 Tips

- Always use `name` attributes so data is submitted correctly.
- Use `required` to enforce form validation.
- Wrap form elements in labels or associate with `for` for accessibility.
