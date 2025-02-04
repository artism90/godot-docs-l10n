:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualScriptSequence.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualScriptSequence:

VisualScriptSequence
====================

**Inherits:** :ref:`VisualScriptNode<class_VisualScriptNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Ejecuta una serie de puertos de secuencia.

Descripción
----------------------

Pasos a través de una serie de uno o más puertos de secuencia de salida. El puerto de datos ``current`` da salida al elemento que se está ejecutando actualmente.

\ **Puertos de entrada:**\ 

- Secuencia: ``in order``\ 

\ **Puertos de salida:**\ 

- Secuencia: ``1``\ 

- Secuencia: ``2 - n`` (opcional)

- Data (int): ``current``

Propiedades
----------------------

+-----------------------+---------------------------------------------------------+-------+
| :ref:`int<class_int>` | :ref:`steps<class_VisualScriptSequence_property_steps>` | ``1`` |
+-----------------------+---------------------------------------------------------+-------+

Descripciones de Propiedades
--------------------------------------------------------

.. _class_VisualScriptSequence_property_steps:

- :ref:`int<class_int>` **steps**

+-----------+------------------+
| *Default* | ``1``            |
+-----------+------------------+
| *Setter*  | set_steps(value) |
+-----------+------------------+
| *Getter*  | get_steps()      |
+-----------+------------------+

El número de pasos en la secuencia.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
