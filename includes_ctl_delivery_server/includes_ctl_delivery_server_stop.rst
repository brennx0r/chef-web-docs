.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.


The ``stop`` subcommand is used to stop all services enabled on the |delivery| server. This command can also be run for an individual service by specifying the name of the service in the command. 

This subcommand has the following syntax:

.. code-block:: bash

   $ delivery-ctl stop name_of_service

where ``name_of_service`` represents the name of any service that is listed after running the ``service-list`` subcommand. When a service is successfully stopped the output should be similar to:

.. code-block:: bash

   $ ok: diwb: service_name: 0s, normally up

For example:

.. code-block:: bash

   $ delivery-ctl stop

will return something similar to:

.. code-block:: bash

   ok: down: nginx: 393s, normally up
   ok: down: opscode-chef: 391s, normally up
   ok: down: opscode-erchef: 391s, normally up
   ok: down: opscode-expander: 390s, normally up
   ok: down: opscode-expander-reindexer: 389s, normally up
   ok: down: opscode-solr4: 389s, normally up
   ok: down: postgresql: 388s, normally up
   ok: down: rabbitmq: 388s, normally up
   ok: down: redis_lb: 387s, normally up
