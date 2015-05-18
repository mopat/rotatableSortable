# rotatableSortable
A sortable jquery Plugin to sort rotated Containers.
$playlist.rotatableSortable({
                contentId: "#rotatable",
                delegates: ".playlist-item",
                rotation: getRotation(),
                sortEnd: function () {
                    setPlaylistIds();
                }
            });
