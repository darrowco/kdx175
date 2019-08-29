:orphan:

Welcome to Parts Log
====================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

.. raw:: html

    <script type="text/javascript" class="init">
    $(document).ready(function() {
    $('#example').DataTable();
    $('#example').tableTotal();
    } );
    var table = document.getElementById("example");
    if (table != null) {
        for (var i = 0; i < table.rows.length; i++) {
            for (var j = 0; j < table.rows[i].cells.length; j++)
            table.rows[i].cells[j].onclick = function () {
                tableText(this);
            };
        }
    }

    function tableText(tableCell) {
        alert(tableCell.innerHTML);
    }
    </script>
    <table id="example" class="display table table-bordered" style="width:100%">
    <thead>
    <tr>
    <th>&nbsp;</th>
    <th>Position</th>
    <th>Office</th>
    <th>Age</th>
    <th>Start date</th>
    <th>Salary</th>
    </tr>
    </thead>
    <tbody>
.. include:: engine_20190715.rst
    :start-after: <!-- dbRowsParts -->

.. raw:: html

    <button value="Refresh Page" onClick="window.location.reload();">


footers
