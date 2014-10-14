Libvirt port-forwarding hook
============================

Fork of hook made my Sascha Peilicke,
available under that link: https://github.com/saschpe/libvirt-hook-qemu

Libvirt hook for setting up firewalld port-forwarding rules when using NAT-ed
networking.


Installation
------------

To install the hook script and it's configuration files, simply use the
:file:`Makefile`:

.. code-block:: bash

    $ sudo make install

Afterwards customize :file:`/etc/libvirt/hooks/qemu.json` to your needs.
This Makefile target can be invoked multiple times, already installed
configuration files won't be touched. The files can be removed again with:

.. code-block:: bash

    $ sudo make clean


Author
------

Przemysław Szypowicz
