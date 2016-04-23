webtiles
========

This is a client library for the WebTiles server protocol for the game
[Dungeon Crawl: Stone Soup](http://crawl.develz.org/).

Dependencies
------------

* Python 3.3 or later
* Recent asyncio module (3.4.3 tested)
* Recent websockets module (3.0 tested)

Installation
------------

This package uses [setuptools](http://pythonhosted.org/setuptools) and can be
installed with `pip3`. For example:

    cd webtiles
    pip3 install --user https://github.com/gammafunk/webtiles.git

The library will be available on PyPI when it reaches a more feature-complete
state.

Documentation
-------------

See the pydoc for [connection.py](webtiles/connection.py) as well as the
working example in [updaterc.py](webtiles/updaterc.py), which is installed by
`pip3` as the script `update-dcss-rc`.

The library is currently extremely simple, with only enough functionality to
support the [beem](https://github.com/gammafunk/beem) project. It can handle
the basics of connecting, authentication, reading messages, getting game types,
and updating RC files through the `WebTilesConnection` class, reading lobby
data through the `WebTilesLobbyConnection` class), and watching games and
reading/sending chat messages through the `WebTilesGameConnection` class.
