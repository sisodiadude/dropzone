# Sisodia DropZone - Documentation

## 📌 Introduction

**Sisodia DropZone** is a lightweight, customizable, and user-friendly jQuery plugin that enables seamless **drag-and-drop file uploads**, **manual file selection**, **file input via URL**, and **rich previews**. It offers a clean UI, smart validations, image format conversion, and flexible configuration options—making it ideal for modern web applications.

---

## 🔗 CDN Integration

### CSS

```html
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@1.0.0/dist/style.css" rel="stylesheet">
```

### JavaScript

```html
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@1.0.0/dist/script.js"></script>
```

---

## ⚙️ Initialization (Basic Usage)

### HTML Input

```html
<input type="file" id="fileInput">
```

### jQuery Initialization

```javascript
$(document).ready(function() {
    $('#fileInput').sisodiaDropZone();
});
```

---

## ✨ Key Features

* ✅ **Drag & Drop** upload support
* 📁 **Browse button** for manual file selection
* 🖼️ **Real-time file previews** with remove option
* 🌐 **Add files via URL**
* 🔁 **Multiple file selection**
* 🛡️ **Accepted file format validation**
* 🧠 **Smart duplicate file detection**
* 🧱 **Image conversion before upload**
* ⚙️ **Fully customizable via initialization options**

---

## 🔧 Full Configuration Options

You can fully customize the DropZone via initialization parameters:

```javascript
$('#fileInput').sisodiaDropZone({
    acceptedFormats: "image/png, image/jpeg, application/pdf", // Accept specific formats, or use "image/*" for all images
    inputName: "uploadedFiles", // Custom input field name for server-side access
    heading: "Upload Your Files", // Main heading above the drop area
    subheading: "Supported formats: PNG, JPEG, PDF", // Subheading text
    browseButtonText: "Select Files", // Text for the browse button
    showUrlInput: true, // Enable/disable URL-based image uploads
    maxLimit: 200, // Maximum number of files allowed
    isMultiple: true, // Allow multiple file selection
    imageConversion: { // Convert uploaded image formats to match server-side requirements
        'png': 'jpg',
        'jpg': 'webp',
        'jpeg': 'png',
        'webp': 'png'
        // You can also use 'image/*': 'jpg' to convert all images to JPG
    },
    allowDuplicateFileUpload: true // Allow or prevent uploading the same file multiple times
});
```

---

## 📚 Configuration Priority

Settings are applied in the following order of precedence:

1. **Initialization Options** (`$('#selector').sisodiaDropZone({...})`)
2. **HTML Input Tag Attributes** (`<input ...>`)
3. **Plugin Defaults**

---

## 📸 Live Preview

![Preview](https://drive.google.com/file/d/1KTXwRBcEkAqRKFXZMVP4XtSSh8uE1gDb/view)

---

## 🧾 License

This plugin is open-source under the [MIT License](https://opensource.org/licenses/MIT).

---

## 🔗 Author

Developed with ❤️ by [@sisodiadude](https://github.com/sisodiadude)
