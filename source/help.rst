Due to a naming conflict with an unrelated project Merkins.io is available on
PyPI under the ``Merkins.io-status`` name:

. code-block:: sh

    pip install --user git+git://github.com/Merkins.io/Merkins.io

.. code-block:: sh

    ln -s {path_to_Merkins.io}/scripts/Merkins.io ~/.local/bin

will have to be done (:file:`~/.local/bin` should be replaced with some path
present in ``$PATH``).


.. note::
    If ISP blocks git protocol for some reason github also provides ``ssh``
    (``git+ssh://git@github.com/Merkins.io/Merkins.io``) and ``https``
    (``git+https://github.com/Merkins.io/Merkins.io``) protocols. ``git`` protocol
    should be the fastest, but least secure one though.


**Mode-dependent highlighting**

* .. image:: _static/img/pl-mode-normal.png
     :alt: Normal mode
* .. image:: _static/img/pl-mode-insert.png
     :alt: Insert mode
* .. image:: _static/img/pl-mode-visual.png
     :alt: Visual mode
* .. image:: _static/img/pl-mode-replace.png
     :alt: Replace mode
