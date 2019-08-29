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
    </script>
    <table id="example" class="display table table-bordered" style="width:100%">
    <thead>
    <tr>
    <th>&nbsp;</th><th> #      </th><th> Description, part#, etc    </th><th> Source         </th><th> Cost      </th>
    </tr>
    </thead>
    <tbody>
.. include:: engine_20190715.rst
    :start-after: <!-- dbRowsParts -->

.. raw:: html

    <button value="Generate Total" onClick="window.location.reload();">Generate Total</buttom>

