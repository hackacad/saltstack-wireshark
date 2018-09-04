Saltstack Wireshark Dissector
========================

This is a Lua dissector for Saltstack using ZeroMQ. 

![Saltstack Wireshark Dissector Screenshot](/screenshots/saltstack_wireshark_dissector.png)
saltstack_wireshark_dissector.png

Installation
------------

This dissector requires Lua 5.2 or newer.

    mkdir -p ~/.config/saltstack-wireshark/plugins
    git clone git://github.com/hackacad/saltstack-wireshark ~/.config/wireshark/plugins/saltstack-wireshark/

Usage
-----

Salt should be automatically detected by Wireshark, when using non standard ports change it on 
> Preferences → Protocols → Salt

You can use expression `salt` to filter packets. TCP segments are automatically reassembled.


License
-------

See [LICENSE](LICENSE.txt).

Acknowledgements
----------------

This dissector is based on a dissector for ZMTP https://github.com/whitequark/zmtp-wireshark
