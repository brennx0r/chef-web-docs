=====================================================
InSpec
=====================================================
.. include:: ../../includes_inspec/includes_inspec.rst

.. note:: See every |inspec resource| in a single topic: https://docs.chef.io/inspec_reference.html.

.. include:: ../../includes_inspec/includes_inspec_resources_list.rst

Examples
-----------------------------------------------------
The following examples show how to use the |dsl compliance| to build tests.

**Only accept requests on secure ports**

This code uses the ``port`` resource to ensure that a web server is only listening on well-secured ports.

.. include:: ../../step_inspec/step_inspec_port_listen_on_secure_ports.rst

**Use approved strong ciphers**

This code uses the ``sshd_config`` resource to ensure that only enterprise-compliant ciphers are used for |ssh| servers.

.. include:: ../../step_inspec/step_inspec_sshd_conf_use_strong_ciphers.rst

**Test a kitchen.yml file driver**

This code uses the ``yaml`` resource to ensure that the |kitchen| driver is |vagrant|.

.. include:: ../../step_inspec/step_inspec_yaml_kitchen_driver.rst
