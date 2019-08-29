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
    table = $('#example').DataTable( {
		"ajax": "/ajax/objects.txt",
		"columns": [
			{ "data": "name" },
			{ "data": "position" },
			{ "data": "office" },
			{ "data": "extn" },
			{ "data": "start_date" },
			{ "data": "salary" }
		],
        dom: 'frtip',
        select: true,
	} );
    table2 = $('#example2').DataTable({
        dom: 'frtip',
        select: true,
    });
    </script>
    <table id="example" class="display table table-bordered" style="width:100%">
    <thead>
    <tr>
    <th>&nbsp;</th>
    <th name="id1">Position</th>
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
