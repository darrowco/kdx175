:orphan:

Parts & Labor Log
=================

.. toctree::
   :maxdepth: 2
   :caption: Contents:


.. raw:: html

    <script type="text/javascript" class="init">
  $(document).ready(function() {
    var table = $('#example').DataTable({
      "paging":   false,
      "searching":   false,
      "initComplete": function (settings, json) {
        this.api().columns('.sum').every(function () {
            var column = this;
            var sum = column
               .data()
               .reduce(function (a, b) {
                   a = parseFloat(a, 10);
                   if(isNaN(a)){ a = 0; }
                   b = parseFloat(b, 10);
                   if(isNaN(b)){ b = 0; }
                   return a + b;
               });
            $(column.footer()).html(sum);
        });
      }
    });
    });
    </script>
    <table id="example" class="display table table-bordered" style="width:100%">
    <thead>
    <tr>
    <th> #  </th><th align="left"> Parts & 3rd-party Labor</th><th align="left"> Source         </th><th class="sum">       Cost</th><th class="sum">My Time</th>
    </tr>
    </thead>
    <tfoot>
        <tr>
            <th></th>
            <th></th>
            <th align="right">Sums</th>
            <th align="right"></th>
            <th align="right"></th>
        </tr>
    </tfoot>
    <tbody>

.. include:: engine_20190715.rst
    :start-after: <!-- dbRowsParts -->
    :end-before: <!-- dbRowsPartsEnd -->
.. include:: electrical_20190804.rst
    :start-after: <!-- dbRowsParts -->
    :end-before: <!-- dbRowsPartsEnd -->

.. raw:: html

    </tbody>
    </table>
