```markdown
# OTP Generator React App

An interactive One-Time Password (OTP) generator built with React. This app generates a 6-digit OTP that expires after 5 seconds. Users can generate a new OTP by clicking the "Generate OTP" button, which is disabled during the countdown to prevent multiple concurrent timers.

---

## Features

- Generate a 6-digit OTP with a single click.
- Displays the OTP or prompts the user to generate one.
- Shows a countdown timer indicating OTP expiry.
- Automatically expires the OTP after 5 seconds.
- Button disables during countdown to prevent multiple OTPs.
- Clear messages guide the user through the process.

---

## Technologies Used

- React (JavaScript)
- React Hooks (`useState`, `useEffect`, `useRef`)
- HTML & CSS (for styling)

---

## How to Run

### Prerequisites

- A modern web browser
- Basic knowledge of HTML and JavaScript

### Setup

1. **Clone the repository or copy the code into your project folder.**

2. **Ensure you have the following structure:**

``
index.html
index.jsx
styles.css (optional for styling)
``

3. **index.html** should contain the HTML boilerplate, including React and Babel CDN links, and a root element:

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8" />
    <title>OTP Generator</title>
    <link rel="stylesheet" href="styles.css" />
    <script src="https://cdnjs.cloudflare.com/ajax/libs/react/18.3.1/umd/react.development.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/18.3.1/umd/react-dom.development.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/7.26.5/babel.min.js"></script>
</head>
<body>
    <div id="root"></div>
    <script
      type="text/babel"
      src="index.jsx"
    ></script>
    <script>
      const { ReactDOM } = window;
      ReactDOM.createRoot(document.getElementById('root')).render(<OTPGenerator />);
    </script>
</body>
</html>
``

4. **index.jsx** should contain the `OTPGenerator` component code provided earlier.

---

## Usage

- Open `index.html` in your browser.
- Click the **"Generate OTP"** button:
  - A 6-digit OTP will be displayed.
  - A countdown timer of 5 seconds will start.
  - The button will be disabled during the countdown.
- Once the timer reaches zero:
  - The OTP expires message appears.
  - The button becomes enabled for generating a new OTP.

---

## Customization & Styling

- Use `styles.css` to add custom styles for `.container`, headings, buttons, and messages.
- You can modify the OTP length or expiration time by editing the `generateOTP` function and `setTimeLeft` value.

---

## License

This project is for educational purposes and is provided "as-is" without any warranties. Feel free to modify and extend it!

---

## Acknowledgments

Built as a React coding exercise to practice hooks and component state management.
```
