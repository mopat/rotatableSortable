# rotatableSortable
A sortable jquery Plugin to sort lists in rotated Containers. Usage is possible with touch and mouse for Desktop, Tablet and Smartphone!

##Usage##<script src="rotatableSortable.js"></script>
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

##Remove##
To remove the sortable from your list use the following code:
```javascript
$("#my-list").destroy({
                delegates: ".my-list-li"
            });
```
##Switch on/off##
To switch the sort function on or off first remove and add sort function again.
```javascript
// add sort function
$('#my-list').rotatableSortable({
                delegates: '.my-list-li',
                rotation: 180,
                sortEnd: function () {
                    sortEndHandler();
                }
            });
```

```javascript
// remove sort function
$("#my-list").destroy({
                delegates: ".my-list-li"
            });
```
