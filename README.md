# rotatableSortable
A sortable jquery Plugin to sort lists in rotated Containers.

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
