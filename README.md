# jsvm
JavaScript virtualization library with QEMU in the backend

# Installation
Include in your own site:
```html
<script src="dist/jsvm.js"></script>
```
or get it from a CDN:
```html
<script src="https://cdn.jsdelivr.net/gh/Unzor/jsvm/dist/jsvm.js"></script>
```

# Usage
Example HTML code:
```html
<!DOCTYPE HTML>
<html>
<body>
  <script src="https://cdn.jsdelivr.net/gh/Unzor/jsvm/jsvm.js"></script>
  <vm-instance floppy-disk="images/windows101.img"></vm-instance>
</body>
</html>
```

Windows 1.1 image from [https://github.com/copy/images](https://github.com/copy/images).
