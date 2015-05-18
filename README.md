# rotatableSortable
A sortable jquery Plugin to sort lists in rotated Containers.

Usage:
`$playlist.rotatableSortable({
                contentId: "#rotatable",
                delegates: ".playlist-item",
                rotation: getRotation(),
                sortEnd: function () {
                    setPlaylistIds();
                }
            });
          `
