# hugePasteFromWord

v0.0.1 alpha

A tinyMCE 6 / hugeMCE paste from word plugin

Inspiration taken from on https://github.com/ihwf/paste-from-word (the example word files I tested broke this implementation)

The PasteFromWord class handles the pasting of content from Microsoft Word into a web application. It includes methods for:

1. Detecting if the pasted content is from Word.
2. Cleaning the pasted HTML content by removing Word-specific tags and attributes.
3. Converting Word-specific lists to proper HTML lists.
4. Extracting and handling images from the clipboard data, including those in RTF format.
5. Converting blob URLs to base64 strings and replacing them in the HTML content.
6. Handling single file paste operations.

## usage

```
import "./src/pasteFromWord/index.js";
```

In your tiny / hugeMCE config add 

```
plugins: `pasteFromWord`
```