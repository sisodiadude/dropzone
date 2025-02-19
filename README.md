Sisodia DropZone - Documentation  body { background-color: #f4f7f6; font-family: 'Arial', sans-serif; } .code-block { background: #282c34; color: #ffffff; padding: 15px; border-radius: 5px; font-family: monospace; } .dropzone-preview { display: flex; flex-wrap: wrap; gap: 10px; } .dropzone-preview img { width: 100%; height: 100%; object-fit: cover; border-radius: 5px; border: 2px solid #ddd; } .container { max-width: 900px; background: white; padding: 30px; border-radius: 10px; box-shadow: 0px 4px 10px rgba(0,0,0,0.1); }

Sisodia DropZone - Documentation
================================

📌 Introduction
---------------

**Sisodia DropZone** is a lightweight and powerful jQuery plugin that enables \*\*drag & drop file uploads\*\*, \*\*direct file selection from URLs\*\*, and \*\*customizable file previews\*\* with a seamless user experience.

🔗 CDN Integration
------------------

Include the following libraries in your HTML file:

##### CSS:

<link href="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@v1.0.0/dist/style.css" rel="stylesheet">

##### JavaScript:

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://cdn.jsdelivr.net/gh/sisodiadude/dropzone@v1.0.0/dist/script.js"></script>

⚙️ jQuery Initialization
------------------------

Add an \*\*input field\*\* for file selection:

<input type="file" id="fileInput">

Then initialize it using jQuery:

$(document).ready(function() {
    $('input\[type="file"\]').sisodiaDropZone();
});

✨ Features
----------

*   🔹 \*\*Drag & Drop\*\* support
*   🔹 \*\*Browse button\*\* for file selection
*   🔹 \*\*File preview\*\* with add/remove functionality
*   🔹 \*\*Direct file select from URL\*\*
*   🔹 \*\*Multiple file selection\*\* support
*   🔹 \*\*Customizable accepted file formats\*\*

📸 Example Preview
------------------

![Preview](image-1.png)

🛠️ Advanced Configuration
--------------------------

You can customize the DropZone by passing options:

$('input\[type="file"\]').sisodiaDropZone({
    acceptedFormats: "image/png, image/jpeg, application/pdf", // Allowed file types
    inputName: "uploadedFiles", // Custom name attribute for the input field
    heading: "Upload Your Files", // Heading for the DropZone component
    subheading: "Supported formats: PNG, JPEG, PDF", // Subheading text
    browseButtonText: "Select Files", // Text for the browse button
    showUrlInput: true, // Enable or disable file selection via URL
    maxLimit: 200, // Maximum file number limit
    isMultiple: true // Allow multiple file selection
});

##### Priority Handling

**Note:** If attributes that are valid for the input tag are present, they will be used unless overridden by initialization options.

*   **Initialization options** (Highest Priority)
*   **Input tag attributes** (Medium Priority)
*   **Default settings** (Lowest Priority)
