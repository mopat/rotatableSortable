# rotatableSortable
A sortable jquery Plugin to sort lists in rotated Containers.

Usage:
```javascript
$('#my-list').rotatableSortable({
                delegates: 'li .list-item-delegates',
                rotation: 180,
                sortEnd: function () {
                    sortEndHandler();
                }
            });
```
