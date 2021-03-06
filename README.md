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
  <script src="https://cdn.jsdelivr.net/gh/Unzor/jsvm/dist/jsvm.js"></script>
  <vm-instance floppy-disk="images/windows101.img"></vm-instance>
</body>
</html>
```
```diff
- * Windows 1.1 image from https://github.com/copy/images.
```

To create a VM instance programmatically, use this example:
```javascript
var jsvm_instance = JSvm.createInstance();
JSvm.setCDRom(jsvm_instance, "linux.iso");
document.body.appendChild(jsvm_instance);
JSvm.checkForElements();
```
To check again for elements/VM instances that need to be initialized, use this:
```javascript
JSvm.checkForElements();
```
This is useful when after adding new VM instances programmatically.

# Modes

```<vm-instance cd-rom="url"></vm-instance>``` - CD ROMS: .iso

```<vm-instance floppy-disk="url"></vm-instance>``` - Floppy Disks: .img, .dsk

```<vm-instance hard-disk="url"></vm-instance>``` - Hard Disks: .img

```<vm-instance state="url"></vm-instance>``` - Save State: .bin

# API Modes
```JSvm.setCDRom(element, url)``` - CD ROMS: .iso

```JSvm.setFloppyDisk(element, url)``` - Floppy Disks: .img, .dsk

```JSvm.setHardDisk(element, url)``` - Hard Disks: .img

```JSvm.setState(element, url)``` - Save State: .bin



