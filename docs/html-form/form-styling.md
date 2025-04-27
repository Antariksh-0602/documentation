---
title: Form styling
lang: en-US
---

# Form styling

With Formspark you get to bring your own HTML and CSS.

On this page you'll find tips, tricks and links to help you style your forms.

## Simple vertical layout

![Simple vertical layout](../.vuepress/public/simple-vertical-layout.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <style>
      .vertical-form {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
        max-width: 500px;
      }
    </style>
  </head>
  <body>
    <form class="vertical-form" action="https://submit-form.com/your-form-id">
      <label for="your-name">Your name</label>
      <input id="your-name" name="your-name" type="text" />
      <label for="email">email-id</label>
      <input id="email" name="email-id" type="email" />
      <label for="Phone-Number">Phone-Number</label>
      <input id="Phone-Number" name="Phone-Number" type="number" />
      <label for="message">Message</label>
      <textarea id="message" name="message" cols="15" rows="5"></textarea>
      <button type="submit">Submit</button>
    </form>
  </body>
</html>
```

## Add an asterisk to required field labels

![Required field label asterisk](../.vuepress/public/required-field-label-asterisk.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <style>
      label.required:after {
        content: "*";
        color: red;
      }
    </style>
  </head>
  <body>
    <form action="https://submit-form.com/your-form-id">
      <label for="first-name" class="required">First name</label>
      <input id="first-name" name="first-name" type="text" required />
      <label for="last-name">Last name</label>
      <input id="last-name" name="last-name" type="text" />
      <button type="submit">Submit</button>
    </form>
  </body>
</html>
```

## CSS frameworks

- [Bootstrap](https://getbootstrap.com/)
- [Milligram](https://milligram.io/)
- [Tailwind CSS](https://tailwindcss.com/)
