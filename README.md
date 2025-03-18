# TEKICON

## About
This is a lightweight package of SVG icons.

## Install
Run the command
```bash
  npm i tekicon
```
### JS

Place the following code in your JavaScript file:
```javascript
import iconSetter from "tkicon";

document.addEventListener("DOMContentLoaded", function(event){
    iconSetter();
});
```
and

To get a list of icons:
```javascript
import {iconList} from "tkicon";

console.log(iconList)
```
`iconList` return an object

### HTML

in HTML pages use:
```html
<i class="tkicon" data-icon="example" size="24"></i>
```
for example `<i class="tkicon" data-icon="wolrd" size="24">`
- Icons have a default size of 24px, but you can modify it.

### CSS
Almost all icons contain two *path* tags (using **stroke** instead of fill), allowing you to style them individually or via the svg tag.

for example:

```css
svg.tkicon{
    fill:none;
    stroke: #1d0002;
}
```
or
```css
.tkicon path:nth-child(1){
    fill:#1d0002;
    stroke: #1d0002;
}
.tkicon path:nth-child(2){
    fill:none;
    stroke: #51a2ff;
}
```

## How it works
The `iconSetter` function scans for elements containing the **tkicon** class, replacing them with svg tags to keep the document clean and free of redundant elements.

## also see
- [npm](https://www.npmjs.com/package/tekicon)
- [github](https://github.com/teksite/tekicon.git)
- [laratek](https://laratek.ir)
- [teksite](https://teksite.net)
