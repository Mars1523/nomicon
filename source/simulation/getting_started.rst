Getting Started
===============

Setting up the code to support simulation

.. todo::
    Provide a base robot to teach the sim with. (Github with tags)

On its own, the simulator doesn't do much (or anything for that matter).  We
must define certain settings and define how our physics works.  Don't worry,
it isn't that complicated, just two files, and many helpers are provided to
assist you.

Configuration file
++++++++++++++++++

The simulator will load configuration from ``sim/config.json`` For more
information on this, see :doc:`additional_configuration`.

To get started, add a basic config that just says where we want our robot to be
in the field.

.. code-block:: json

    {
        "pyfrc": {
            "robot": {
                "w": 2,
                "h": 3,
                "starting_x": 2,
                "starting_y": 20,
                "starting_angle": 0
            }
        }
    }

Physics
+++++++

The next step is defining how our robot reacts.  This is documented on the next
page.