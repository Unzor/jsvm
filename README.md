# jsvm
JavaScript virtualization library with QEMU in the backend
# Demo
[Here is the demo for JSvm.](https://unzor.github.io/jsvm)
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
```diff
- * Windows 1.1 image from https://github.com/copy/images.
```

To check again for elements/VM instances that need to be initialized, use this:
```javascript
JSvm.checkForElements();
```
This is useful when after adding new VM instances programmatically.

# Modes

```<vm-instance cd-rom="url"></vm-instance>``` - CD ROMS: .iso

```<vm-instance floppy-disk="url"></vm-instance>``` - Floppy Disks: .img, .dsk

```<vm-instance hard-disk="url"></vm-instance>``` - Hard Disks: Unknown.
