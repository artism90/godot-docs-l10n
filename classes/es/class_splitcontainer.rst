:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the SplitContainer.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_SplitContainer:

SplitContainer
==============

**Inherits:** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`HSplitContainer<class_HSplitContainer>`, :ref:`VSplitContainer<class_VSplitContainer>`

Contenedor para dividir y ajustar.

Descripción
----------------------

Contenedor para dividir dos :ref:`Control<class_Control>`\ s vertical u horizontalmente, con un agarrador que permite ajustar el desplazamiento o la relación de división.

Propiedades
----------------------

+-----------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                                         | :ref:`collapsed<class_SplitContainer_property_collapsed>`                   | ``false`` |
+-----------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
| :ref:`DraggerVisibility<enum_SplitContainer_DraggerVisibility>` | :ref:`dragger_visibility<class_SplitContainer_property_dragger_visibility>` | ``0``     |
+-----------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+
| :ref:`int<class_int>`                                           | :ref:`split_offset<class_SplitContainer_property_split_offset>`             | ``0``     |
+-----------------------------------------------------------------+-----------------------------------------------------------------------------+-----------+

Métodos
--------------

+------+---------------------------------------------------------------------------------------+
| void | :ref:`clamp_split_offset<class_SplitContainer_method_clamp_split_offset>` **(** **)** |
+------+---------------------------------------------------------------------------------------+

Señales
--------------

.. _class_SplitContainer_signal_dragged:

- **dragged** **(** :ref:`int<class_int>` offset **)**

Emitido cuando el arrastrador es arrastrado por el usuario.

Enumeraciones
--------------------------

.. _enum_SplitContainer_DraggerVisibility:

.. _class_SplitContainer_constant_DRAGGER_VISIBLE:

.. _class_SplitContainer_constant_DRAGGER_HIDDEN:

.. _class_SplitContainer_constant_DRAGGER_HIDDEN_COLLAPSED:

enum **DraggerVisibility**:

- **DRAGGER_VISIBLE** = **0** --- El arrastre dividido es visible cuando el cursor pasa por encima.

- **DRAGGER_HIDDEN** = **1** --- El arrastre dividido nunca es visible.

- **DRAGGER_HIDDEN_COLLAPSED** = **2** --- El arrastrador dividido nunca es visible y su espacio se colapsó.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_SplitContainer_property_collapsed:

- :ref:`bool<class_bool>` **collapsed**

+-----------+----------------------+
| *Default* | ``false``            |
+-----------+----------------------+
| *Setter*  | set_collapsed(value) |
+-----------+----------------------+
| *Getter*  | is_collapsed()       |
+-----------+----------------------+

Si ``true``, el área del primer :ref:`Control<class_Control>` se colapsará y el arrastrador se desactivará.

----

.. _class_SplitContainer_property_dragger_visibility:

- :ref:`DraggerVisibility<enum_SplitContainer_DraggerVisibility>` **dragger_visibility**

+-----------+-------------------------------+
| *Default* | ``0``                         |
+-----------+-------------------------------+
| *Setter*  | set_dragger_visibility(value) |
+-----------+-------------------------------+
| *Getter*  | get_dragger_visibility()      |
+-----------+-------------------------------+

Determina la visibilidad del arrastrador. Ver :ref:`DraggerVisibility<enum_SplitContainer_DraggerVisibility>` para más detalles.

----

.. _class_SplitContainer_property_split_offset:

- :ref:`int<class_int>` **split_offset**

+-----------+-------------------------+
| *Default* | ``0``                   |
+-----------+-------------------------+
| *Setter*  | set_split_offset(value) |
+-----------+-------------------------+
| *Getter*  | get_split_offset()      |
+-----------+-------------------------+

El desplazamiento inicial de la división entre los dos :ref:`Control<class_Control>`\ s, con ``0`` estando al final del primer :ref:`Control<class_Control>`.

Descripciones de Métodos
------------------------------------------------

.. _class_SplitContainer_method_clamp_split_offset:

- void **clamp_split_offset** **(** **)**

Bloquea el valor :ref:`split_offset<class_SplitContainer_property_split_offset>` para que no se salga de los valores mínimos y máximos actualmente posibles.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
