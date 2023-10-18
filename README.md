# Responsive Login SignIn SignUp

To create a responsive login/sign-in/sign-up form using HTML, CSS (SCSS), and JavaScript:

1. Create an HTML structure for the form.
2. Style it using SCSS (CSS preprocessor).
3. Use JavaScript for form validation and switching between sign-in and sign-up.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="styles.css">
  <title>Login/Sign Up</title>
</head>
<body>
  <div class="container">
    <div class="form-container sign-in-container">
      <!-- Sign-In Form Content -->
    </div>
    <div class="form-container sign-up-container">
      <!-- Sign-Up Form Content -->
    </div>
    <div class="overlay-container">
      <div class="overlay">
        <!-- Overlay Content -->
      </div>
    </div>
  </div>
  <script src="script.js"></script>
</body>
</html>
```

In your `styles.scss`:

```scss
.container {
  display: flex;
  position: relative;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background: linear-gradient(to right, #3a6186, #89253e);
}

/* Style the sign-in and sign-up forms and overlay as needed */
```

In your `script.js`:

```javascript
const sign_in_btn = document.querySelector("#sign-in-btn");
const sign_up_btn = document.querySelector("#sign-up-btn");
const container = document.querySelector(".container");

sign_up_btn.addEventListener("click", () => {
  container.classList.add("sign-up-mode");
});

sign_in_btn.addEventListener("click", () => {
  container.classList.remove("sign-up-mode");
});
```

You'll need to add and style the form elements and validation as needed in the HTML and SCSS files.
