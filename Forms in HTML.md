## 🔹 **Forms in HTML**

Forms allow users to **input data** that gets sent to a server or handled by JavaScript.

All form elements are usually wrapped in a `<form>` tag.

    <form action="/submit" method="POST">
      <!-- form elements go here -->
    </form>
### **1. `<input>` – For Single-Line Input**

The `<input>` element is super versatile. Use different `type` attributes to get different kinds of inputs:

    <input type="text" placeholder="Your Name" />
    <input type="email" placeholder="Email Address" />
    <input type="password" placeholder="Password" />
    <input type="checkbox" /> I agree
    <input type="radio" name="gender" value="male" /> Male
    <input type="radio" name="gender" value="female" /> Female
    <input type="submit" value="Submit" />

