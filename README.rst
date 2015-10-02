.. image:: https://raw.githubusercontent.com/HackEdit/hackedit/master/docs/_static/banner.png

**At the moment, the project is being worked on a private server, the code will be available when the first alpha version is ready.** *(if everything goes right the alpha should be ready in a few weeks)*

About
-----

HackEdit is a hackable editor, built with Python3, PyQt5 and pyQode.

This repository contains the core application, the core plugins. and a simple API for writing plugins and interacting with the application's main objects without knowing much about the internals.

Resources
---------

- `roadmap`_
- `design notes`_
- `screenshots`_

.. _roadmap: https://github.com/HackEdit/hackedit/wiki/Roadmap
.. _design notes: https://github.com/HackEdit/hackedit/wiki/Design-notes
.. _screenshots: https://github.com/HackEdit/hackedit/wiki/Screenshots

Requirements
-------------

- python >= 3.2
- PyQt5 >= 5.2
- pip


Installation
-------------

General instructions
++++++++++++++++++++

1. install **Python3**, **PyQt5** and **pip** (for python3) using your package manager or the installer files available for your platform.

2. install hackedit package using pip::

    pip3 install hackedit --upgrade

3. install plugins *(there will be a plugin manager interface for doing that in a future versions)*, e.g.::

    pip3 install hackedit_python hackedit_cobol --upgrade

Linux
+++++

Ubuntu
~~~~~~

1. Install pip, setuptools and pyqt5::

    sudo apt-get install python3-setuptools python3-pip python3-pyqt5 python3-pyqt5.qtsvg

2. Install hackedit::

    sudo pip3 install hackedit --upgrade

3. Run hackedit::

    hackedit

ArchLinux
~~~~~~~~~

1. Install pip, setuptools and pyqt5::

    sudo pacman -S python3-pyqt5 python3-pip python3-setuptools

2. Install hackedit::

    sudo pip3 install hackedit --upgrade

3. Run hackedit::

    hackedit


Windows/OSX Launchers
+++++++++++++++++++++

We cannot distribute hackedit as a standalone application because hackedit makes heavy use of the python ecosystem (e.g. for plugins management). The integration of python GUI application on Windows or OSX is not as good as on Linux (e.g. you cannot pin the app to the taksbar/dock,...). So we made a native launcher specifically for each platform.

**On windows**, you can grab an installer that will install a portable python installation ready with all python dependencies and a launcher executable that will use the portable installation (you can point it to another python installation). So just grab the installer, check the plugins/tools that you want and you're done.

**On OSX**, you need to install python3 and pyqt5 using a package manager such as homebrew and then use pip to install hackedit and its plugins, as indicated in the general install instructions. Then you can grab the launcher app and copy it to your Applications folder.
