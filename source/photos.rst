Photos
======

.. contents::
   :local:
   :depth: 1

.. raw:: html





    <div id="pig">
      <img id='gsPreviewImg'>
    </div>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jquery.swipebox/1.4.4/css/swipebox.min.css">
    <script src="https://code.jquery.com/jquery-2.0.3.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery.swipebox/1.4.4/js/jquery.swipebox.min.js"></script>
    <script type="text/javascript" src="https://i.modjeska.us/js/pig.js"></script>
    <script type="text/javascript">

      function compare(a, b) {
        const filenameA = a.filename.toUpperCase();
        const filenameB = b.filename.toUpperCase();
        let comparison = 0;
        if (filenameA > filenameB) {
          comparison = 1;
        } else if (filenameA < filenameB) {
          comparison = -1;
        }
        return comparison;
      }

      var imageData = [
        {"filename": "mess.jpeg", "aspectRatio": "1.4900"},
        {"filename": "out.jpeg", "aspectRatio": "1.7700"},
        {"filename": "spokes.jpeg", "aspectRatio": "1.7700"},
        {"filename": "wiring.png", "aspectRatio": "1.4900"},
        {"filename": "tools.png", "aspectRatio": "1.3300"},
        {"filename": "extract.jpeg", "aspectRatio": "1.3300"},
      ];
      imageData.sort(compare);
      var pig = new Pig(imageData, {
        urlForSize: function(filename, size) {
        return '_static/images/' + 'img/' + size + '/' + filename;
      },
      addAnchorTag: true,
      anchorTargetDir: "_static/images/",
      anchorClass: "swipebox"
      }).enable();
      ;( function( $ ) {
      	$( '.swipebox' ).swipebox();
      } )( jQuery );
    </script>





