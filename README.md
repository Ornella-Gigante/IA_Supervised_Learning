📄 **jQuery Form Validator Plugin**  
A lightweight jQuery plugin for form validation with customizable error messages and styling. Ideal for enhancing user input validation in web forms.

---

## 🚀 Getting Started

### Features  
- **Validation Rules**: Supports various validations (required, email, etc.) with custom error messages.  
- **Bootstrap Integration**: Compatible with Bootstrap classes (`form-group`, `help-block`).  
- **Custom Styling**: Apply error/success states using CSS classes (`errorElementClass`, `valid`).  
- **Deprecation Handling**: Warns about outdated attributes like `data-validation-if-checked` (use `data-validation-depends-on`).  
- **Events**: Triggers events like `validationErrorDisplay` for custom error handling.  

---

## 🛠️ Installation  
Include jQuery and the plugin script:  
```html
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="jquery.form-validator.min.js"></script>
```

---

## 🎯 Usage  
Initialize validation on a form:  
```javascript
$('form').validate({
  errorMessageClass: 'alert alert-danger',
  submitErrorMessageCallback: function($form, config, errors) {
    // Custom error handling
  }
});
```

### Key Configuration Options  
| Option | Description |  
|--------|-------------|  
| `errorMessageClass` | CSS class for error messages (default: `help-block`). |  
| `inputParentClassOnError` | Parent container class on error (e.g., `has-error`). |  
| `submitErrorMessageCallback` | Callback to handle form-wide errors. |  

---

## ⚠️ Deprecation Notes  
- Avoid `errorMessageCustom`; use `submitErrorMessageCallback` instead.  
- Replace `data-validation-if-checked` with `data-validation-depends-on`.  

---

## 🔌 Events  
- `validationErrorDisplay`: Triggered when an error message is shown.  
  ```javascript
  $(window).on('validationErrorDisplay', function(event, $input, $errorMsg) {
    // Custom logic
  });
  ```

---

## 🌍 Browser Support  
Tested in modern browsers (Chrome, Firefox, Safari). IE10+ compatible.

---

## 🤝 Contributing  
1. Fork the repository.  
2. Use **Grunt** for builds (see comments in the minified code).  
3. Submit a pull request with tests.  

---

## 📜 License  
MIT License © [Victor Jonsson](http://victorjonsson.se).  

---

🛡️ **Acknowledgements**  
- Built with Grunt for task automation.  
- Inspired by community feedback and legacy validation practices.

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/14161216/2ff986e6-f053-4c9c-b5c0-cc0caeb8f3b7/jquery.form-validator.min.js
