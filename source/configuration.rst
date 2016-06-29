************
Configuración de repositorios GIT
************

GITHUB
====================
.. note::
    Gracias a la integración de Merkinsio con el API de Github no es necesario
    realizar ninguna configuración adicional en el repositorio.

BITBUCKET
================

.. note::
   * Paso 1: `Configurar SSH Git Clone URL`_
   * Paso 2: `Añadir la clave pública en el usuario de Bitbucket`_

.. _Configure SSH Git Clone URL: configuration.html#configurar-ssh-git-clone-url
.. _Añadir la clave pública en el usuario de Bitbucket: configuration.html#id1


Configurar SSH Git Clone URL
-------------

.. image:: _static/bitbucket/bitbucket_1_ssh_url.png
     :alt: Normal mode

Añadir la clave pública en el usuario de Bitbucket
-------------

Acceder al panel de configuración del usuario de Bitbucket

.. image:: _static/bitbucket/bitbucket_2_Settings.png
    :alt: Normal mode

Seleccionar el menu `security->SSH Keys`

.. image:: _static/bitbucket/bitbucket_3_SSH_keys.png
    :alt: Normal mode

Copiar la clave pública que se ha generado en Merkinsio

.. image:: _static/bitbucket/bitbucket_4_copiar_desde_merkins.png
    :alt: Normal mode

Finalmente añadir la clave pública para habilitar que Merkinsio pueda
acceder a este repositorio

.. image:: _static/bitbucket/bitbucket_5_add_ssh_key.png
    :alt: Normal mode

Webhooks
-------------

Para que Merkinsio compile en cada cambio de código es necesario configurar
un webhook en el respositorio.

La url que se necesita copiar es la URL que aparece cuando se accede a la pantalla
del proyecto en Merkinsio.

.. image:: _static/merkins_webhook.png
    :alt: Normal mode

En la imagen la URL a copiar en Bitbucket es ``https://dashboard.merkins.io/webhooks?appID=77069c08-0a3f-4d43-8a71-2576fb16fdea``
acceder a la configuración del repositorio de bitbucket y dar de alta la url como un nuevo webhook.

.. image:: _static/bitbucket/bitbucket_webhook.png
    :alt: Normal mode

GITLAB
==================

Webhooks
-------------
