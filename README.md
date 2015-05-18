# rotatableSortable
A sortable jquery Plugin to sort lists in rotated Containers. Usage is possible with touch and mouse for Desktop, Tablet and Smartphone!

##Usage
Include the script in your website first. Add this script tag after your jQuery inclusion.
```javascript
<script src="libs/rotatableSortable.js"></script>
```
Let's say your container has the id 'my-list' and your list items have the class 'my-list-li'. 
```javascript
$('#my-list').rotatableSortable({
                delegates: '.my-list-li',
                rotation: 180,
                sortEnd: function () {
                    sortEndHandler();
                }
            });
```

##Remove
To remove the sortable from your list use the following code:
```javascript
$("#my-list").destroy({
                delegates: ".my-list-li"
            });
```
##Change rotation of the list
To change rotation of your list first destroy rotatableSortable then add again.
```javascript
// remove sort function
$("#my-list").destroy({
                delegates: ".my-list-li"
            });
```
```javascript
// add sort function with list rotation of 270 degrees
$('#my-list').rotatableSortable({
                delegates: '.my-list-li',
                rotation: 270,
                sortEnd: function () {
                    sortEndHandler();
                }
            });
```
## Possible Parameters
```javascript
// initialize with id, class or ul
$('ul').rotatableSortable({
                delegates: 'li',  // id, class or ul
                rotation: 270, // 0, 90, 180 or 270 degrees
                delay: 1500, // time in ms for tap or click to start sorting
                scrollTolerance: 150, // upper and bottom border in px of the list to start scrolling
                scrollIntervalDuration: 100, // time in ms of scroll intervall duration
                scrollPx: 100, // number of pixels to scroll up or down
                sortEnd: function () {
                    //executed when mouse or touch is released
                }
            });
```

### Defaults
```javascript
delegates: "li"
rotation: 0
delay: 1000
scrollIntervalDuration: 200
scrollTolerance: 100
scrollPx: 100
```
