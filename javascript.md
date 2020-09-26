# Lunch script each 1 second
```javascript
for (i=0; i< links.length; i++) {
    setTimeout((link) => {
	  link.click();
    }, i * 1000, links[i]);
}
```
