:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the AnimationNodeOneShot.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_AnimationNodeOneShot:

AnimationNodeOneShot
====================

**Inherits:** :ref:`AnimationNode<class_AnimationNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Reproduce una animacion una vez en :ref:`AnimationNodeBlendTree<class_AnimationNodeBlendTree>`.

Descripción
----------------------

Un recurso para añadir a un :ref:`AnimationNodeBlendTree<class_AnimationNodeBlendTree>`. Este nodo ejecutara una subanimacion y devolvera cuando termine. Mezcla de tiempos para desvanecer y aparecer pueden ser personalizados, incluido filtros.

Tutoriales
--------------------

- :doc:`AnimationTree <../tutorials/animation/animation_tree>`

- `Third Person Shooter Demo <https://godotengine.org/asset-library/asset/678>`__

Propiedades
----------------------

+---------------------------+-----------------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`   | :ref:`autorestart<class_AnimationNodeOneShot_property_autorestart>`                           | ``false`` |
+---------------------------+-----------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`autorestart_delay<class_AnimationNodeOneShot_property_autorestart_delay>`               | ``1.0``   |
+---------------------------+-----------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`autorestart_random_delay<class_AnimationNodeOneShot_property_autorestart_random_delay>` | ``0.0``   |
+---------------------------+-----------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`fadein_time<class_AnimationNodeOneShot_property_fadein_time>`                           | ``0.1``   |
+---------------------------+-----------------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`fadeout_time<class_AnimationNodeOneShot_property_fadeout_time>`                         | ``0.1``   |
+---------------------------+-----------------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`   | :ref:`sync<class_AnimationNodeOneShot_property_sync>`                                         | ``false`` |
+---------------------------+-----------------------------------------------------------------------------------------------+-----------+

Métodos
--------------

+---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`MixMode<enum_AnimationNodeOneShot_MixMode>` | :ref:`get_mix_mode<class_AnimationNodeOneShot_method_get_mix_mode>` **(** **)** |const|                                                |
+---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
| void                                              | :ref:`set_mix_mode<class_AnimationNodeOneShot_method_set_mix_mode>` **(** :ref:`MixMode<enum_AnimationNodeOneShot_MixMode>` mode **)** |
+---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+

Enumeraciones
--------------------------

.. _enum_AnimationNodeOneShot_MixMode:

.. _class_AnimationNodeOneShot_constant_MIX_MODE_BLEND:

.. _class_AnimationNodeOneShot_constant_MIX_MODE_ADD:

enum **MixMode**:

- **MIX_MODE_BLEND** = **0**

- **MIX_MODE_ADD** = **1**

Descripciones de Propiedades
--------------------------------------------------------

.. _class_AnimationNodeOneShot_property_autorestart:

- :ref:`bool<class_bool>` **autorestart**

+-----------+------------------------+
| *Default* | ``false``              |
+-----------+------------------------+
| *Setter*  | set_autorestart(value) |
+-----------+------------------------+
| *Getter*  | has_autorestart()      |
+-----------+------------------------+

Si ``true``, las subanimaciones se reiniciaran automaticamente despues de acabar.

----

.. _class_AnimationNodeOneShot_property_autorestart_delay:

- :ref:`float<class_float>` **autorestart_delay**

+-----------+------------------------------+
| *Default* | ``1.0``                      |
+-----------+------------------------------+
| *Setter*  | set_autorestart_delay(value) |
+-----------+------------------------------+
| *Getter*  | get_autorestart_delay()      |
+-----------+------------------------------+

El retardo con el cual un reinicio automatico es lanzado, en segundos.

----

.. _class_AnimationNodeOneShot_property_autorestart_random_delay:

- :ref:`float<class_float>` **autorestart_random_delay**

+-----------+-------------------------------------+
| *Default* | ``0.0``                             |
+-----------+-------------------------------------+
| *Setter*  | set_autorestart_random_delay(value) |
+-----------+-------------------------------------+
| *Getter*  | get_autorestart_random_delay()      |
+-----------+-------------------------------------+

Si :ref:`autorestart<class_AnimationNodeOneShot_property_autorestart>` es ``true``, un retardo aleatorio adicional (en segundos) entre 0 y este valor sera añadido al [member autorestart_delay.

----

.. _class_AnimationNodeOneShot_property_fadein_time:

- :ref:`float<class_float>` **fadein_time**

+-----------+------------------------+
| *Default* | ``0.1``                |
+-----------+------------------------+
| *Setter*  | set_fadein_time(value) |
+-----------+------------------------+
| *Getter*  | get_fadein_time()      |
+-----------+------------------------+

----

.. _class_AnimationNodeOneShot_property_fadeout_time:

- :ref:`float<class_float>` **fadeout_time**

+-----------+-------------------------+
| *Default* | ``0.1``                 |
+-----------+-------------------------+
| *Setter*  | set_fadeout_time(value) |
+-----------+-------------------------+
| *Getter*  | get_fadeout_time()      |
+-----------+-------------------------+

----

.. _class_AnimationNodeOneShot_property_sync:

- :ref:`bool<class_bool>` **sync**

+-----------+---------------------+
| *Default* | ``false``           |
+-----------+---------------------+
| *Setter*  | set_use_sync(value) |
+-----------+---------------------+
| *Getter*  | is_using_sync()     |
+-----------+---------------------+

Descripciones de Métodos
------------------------------------------------

.. _class_AnimationNodeOneShot_method_get_mix_mode:

- :ref:`MixMode<enum_AnimationNodeOneShot_MixMode>` **get_mix_mode** **(** **)** |const|

----

.. _class_AnimationNodeOneShot_method_set_mix_mode:

- void **set_mix_mode** **(** :ref:`MixMode<enum_AnimationNodeOneShot_MixMode>` mode **)**

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
