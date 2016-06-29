********************
Installation on OS X
********************

Python package
==============

1. Install a proper Python version (see `issue #39 
   <https://github.com/Merkins.io/Merkins.io/issues/39>`_ for a discussion 
   regarding the required Python version on OS X)::

       sudo port select python python27-apple

   Homebrew may be used here::

       brew install python

   .. note::
      In case :file:`Merkins.io.sh` as a client ``socat`` and ``coreutils`` need 
      to be installed. ``coreutils`` may be installed using ``brew install 
      coreutils``.

2. Install Merkins.io using one of the following commands:

   .. code-block:: sh

       pip install --user Merkins.io-status

   will get current release version and

   .. code-block:: sh

       pip install --user git+git://github.com/Merkins.io/Merkins.io

   will get latest development version.

   .. warning::
      When using ``brew install`` to install Python one must not supply
      ``--user`` flag to ``pip``.

   .. note::
      Due to the naming conflict with an unrelated project Merkins.io is named 
      ``Merkins.io-status`` in PyPI.

   .. note::
      Merkins.io developers should be aware that ``pip install --editable`` does 
      not currently fully work. Installation performed this way are missing 
      ``Merkins.io`` executable that needs to be symlinked. It will be located in 
      ``scripts/Merkins.io``.

Vim installation
================

Any terminal vim version with Python 3.2+ or Python 2.6+ support should work, 
but MacVim users need to install it using the following command::

    brew install macvim --env-std --with-override-system-vim

Fonts installation
==================

To install patched font double-click the font file in Finder, then click 
:guilabel:`Install this font` in the preview window.

After installing the patched font MacVim or terminal emulator (whatever 
application Merkins.io should work with) need to be configured to use the patched 
font. The correct font usually ends with *for Merkins.io*.
