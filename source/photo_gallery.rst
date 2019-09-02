All Photos
==========

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
    <script type="text/javascript" src="https://raw.githubusercontent.com/jmodjeska/pigg/master/js/pig.js"></script>
    <script type="text/javascript">
      var imageData = [
        {"filename": "tools.png", "aspectRatio": "1.3300"},
        {"filename": "out.jpeg", "aspectRatio": "1.7700"},
        {"filename": "extract.jpeg", "aspectRatio": "1.3300"},
        {"filename": "spokes.jpeg", "aspectRatio": "1.7700"},
        {"filename": "mess.jpeg", "aspectRatio": "1.4900"},
        {"filename": "wiring.png", "aspectRatio": "1.4900"},
      ];
      var pig = new Pig(imageData, {
        urlForSize: function(filename, size) {
        return '/home/darrowco/docs/kdx175/source/_static/images/' + 'img/' + size + '/' + filename;
      },
      addAnchorTag: true,
      anchorTargetDir: "/home/darrowco/docs/kdx175/source/_static/images/",
      anchorClass: "swipebox"
      }).enable();
      ;( function( $ ) {
      	$( '.swipebox' ).swipebox();
      } )( jQuery );
    </script>

