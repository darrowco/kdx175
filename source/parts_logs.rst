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
    document.querySelector("table").addEventListener("click", ({target}) => {
      // discard direct clicks on input elements
      if (target.nodeName === "INPUT") return;
      // get the nearest tr
      const tr = target.closest("tr");
      if (tr) {
        // if it exists, get the first checkbox
        const checkbox = tr.querySelector("input[type='checkbox']");
        if (checkbox) {
          // if it exists, toggle the checked property
          checkbox.checked = !checkbox.checked;
        }
      }
    });
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
