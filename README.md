# Sisodia DropZone - Documentation

## 📌 Introduction
**Sisodia DropZone** is a lightweight and powerful jQuery plugin that enables **drag & drop file uploads**, **direct file selection from URLs**, and **customizable file previews**, offering a seamless user experience.

---

## 🔗 CDN Integration
Include the following libraries in your HTML file:

### CSS:
```html
<link href="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@v1.0.0/dist/style.css" rel="stylesheet">
```

### JavaScript:
```html
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@v1.0.0/dist/script.js"></script>
```

---

## ⚙️ jQuery Initialization
Add an **input field** for file selection:

```html
<input type="file" id="fileInput">
```

Then, initialize it using jQuery:
```javascript
$(document).ready(function() {
    $('input[type="file"]').sisodiaDropZone();
});
```

---

## ✨ Features
✔️ **Drag & Drop** support  
✔️ **Browse button** for file selection  
✔️ **File preview** with add/remove functionality  
✔️ **Direct file selection from URL**  
✔️ **Multiple file selection** support  
✔️ **Customizable accepted file formats**  

---

## 📸 Example Preview
![Preview](https://drive.google.com/file/d/1KTXwRBcEkAqRKFXZMVP4XtSSh8uE1gDb/view)

---

## 🛠️ Advanced Configuration
You can customize the DropZone by passing options:

```javascript
$('input[type="file"]').sisodiaDropZone({
    acceptedFormats: "image/png, image/jpeg, application/pdf", // Allowed file types
    inputName: "uploadedFiles", // Custom name attribute for the input field
    heading: "Upload Your Files", // Heading for the DropZone component
    subheading: "Supported formats: PNG, JPEG, PDF", // Subheading text
    browseButtonText: "Select Files", // Text for the browse button
    showUrlInput: true, // Enable or disable file selection via URL
    maxLimit: 200, // Maximum file number limit
    isMultiple: true // Allow multiple file selection
});
```

---

## 📌 Priority Handling
Attributes and settings are applied based on the following priority order:

1. **Initialization options** (Highest Priority)
2. **Input tag attributes** (Medium Priority)
3. **Default settings** (Lowest Priority)
