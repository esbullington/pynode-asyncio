pynode-asyncio
==============

An Python 3 implementation of Pynode/ArtForz's Bitcoin half-node using the new Python 3 AsyncIO module (aka "Tulip"):

http://docs.python.org/3.4/library/asyncio.html

For Bitcoin data structures, depends on a fork of python-bitcoinlib, with some changes to accomodate Python 3 (will submit PR to original project once I clean up the code).

At the moment, I'm using this along with Tornado and PyZMQ to provide Websockets users a method to subscribe to real-time Bitcoin block and transaction updates.

##How to Install

Requires only Python 3.3 or greater, and no other dependencies.

Earlier versions of Python 3 could use this version by installing the "Tulip" module and changing the respective imports.

##Roadmap

I plan to clean up the code and find a way to integrate PyZMQ without the Tornado dependency, so ZeroMQ users can run this script and subscribe to real-time Bitcoin blockchain events.

## License

MIT

## Acknowledgements

ArtForz, for the original implementation.
Jeff Garzik, with contributions from Peter Todd and others, for the considerable work undertaken to turn the half-node into a full node (although I've not duplicated the all the Pynode features here)
