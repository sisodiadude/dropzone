# Sisodia DropZone - Documentation

## 📌 Introduction
**Sisodia DropZone** is a lightweight, customizable, and user-friendly jQuery plugin that enables seamless **drag-and-drop file uploads**, **file selection via URLs**, and **rich preview support**. It offers a clean UI and flexible configuration options, making it ideal for any modern web project.

---

## 🔗 CDN Integration
Include the following dependencies in your HTML file:

### CSS
```html
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@1.0.0/dist/style.css" rel="stylesheet">
````

### JavaScript

```html
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@1.0.0/dist/script.js"></script>
```

---

## ⚙️ Initialization (Basic Usage)

Add an input element to your HTML:

```html
<input type="file" id="fileInput">
```

Initialize Sisodia DropZone via jQuery:

```javascript
$(document).ready(function() {
    $('#fileInput').sisodiaDropZone();
});
```

---

## ✨ Key Features

* ✅ **Drag & Drop** file upload support
* 📁 **Browse button** for manual file selection
* 🖼️ **File previews** with remove option
* 🌐 **Direct file input from URL**
* 🔄 **Multiple file selection**
* ⚙️ **Fully customizable via options**

---

## 📸 Live Preview

![Preview](https://drive.google.com/file/d/1KTXwRBcEkAqRKFXZMVP4XtSSh8uE1gDb/view)

---

## 🛠️ Advanced Configuration

You can pass configuration options while initializing:

```javascript
$('#fileInput').sisodiaDropZone({
    acceptedFormats: "image/png, image/jpeg, application/pdf", // Allowed MIME types
    inputName: "uploadedFiles", // Custom input field name
    heading: "Upload Your Files", // Main title of the drop zone
    subheading: "Supported formats: PNG, JPEG, PDF", // Subtitle below the heading
    browseButtonText: "Select Files", // Text on the browse button
    showUrlInput: true, // Enables file input via URL
    maxLimit: 200, // Maximum number of files allowed
    isMultiple: true // Enable multiple file upload
});
```

---

## 📚 Priority Handling

Configuration precedence is as follows (highest to lowest):

1. **Initialization options** (via jQuery)
2. **HTML input tag attributes**
3. **Default plugin settings**

---

## 🧾 License

This plugin is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).

---

## 🔗 Author

Developed with ❤️ by [@sisodiadude](https://github.com/sisodiadude)
