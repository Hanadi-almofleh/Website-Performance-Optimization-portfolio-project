# Optimaization 
you can find the link of we page here
https://hanadi-almofleh.github.io/Website-Performance-Optimization-portfolio-project/

https://hanadi-almofleh.github.io/Website-Performance-Optimization-portfolio-project/views/pizza.html

## Main page (index)
 - inline styles.css to html
 - remove link to google font
 - add media print to print.css stylsheet
 - optimize and copress the images
 - minify html
---



## view page (Pizza page)
Two main subject are modified, one for scolling the page and other for slide pizza size.
those using functions updatePositions() and changePizzaSizes(size). below detail for each subject.

### 1-  update position 
##### At event after DOM content Load: 
document.addEventListener('DOMContentLoaded', function() 

- instead of calling update position function after DOM content Load, just assign the position value while creating the element as below line.
 elem.style.left = elem.basicLeft + 'px';
- also reduce number of elements make the 25 instead 200.
- add hight and width in style file.

##### At event Scroll

in the function updatePositions(), calculate the style value outside the loop to avoid FSL

---
### 2- change pizza size 
- calculate pizza width outside the loop. 
- remove unndeeded code like determineDx.
