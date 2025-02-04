:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualInstance.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualInstance:

VisualInstance
==============

**Inherits:** :ref:`CullInstance<class_CullInstance>` **<** :ref:`Spatial<class_Spatial>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`BakedLightmap<class_BakedLightmap>`, :ref:`GIProbe<class_GIProbe>`, :ref:`GeometryInstance<class_GeometryInstance>`, :ref:`Light<class_Light>`, :ref:`ReflectionProbe<class_ReflectionProbe>`, :ref:`RootMotionView<class_RootMotionView>`

Padre de todos los nodos visuales 3D.

Descripción
----------------------

La ``VisualInstance`` se utiliza para conectar un recurso a una representación visual. Todos los nodos visuales 3D heredan de ``VisualInstance``. En general, no debes acceder directamente a las propiedades de ``VisualInstance`` ya que son accedidas y gestionadas por los nodos que heredan de ``VisualInstance``. ``VisualInstance`` es la representación de nodo de la instancia :ref:`VisualServer<class_VisualServer>`.

Propiedades
----------------------

+-----------------------+-----------------------------------------------------+-------+
| :ref:`int<class_int>` | :ref:`layers<class_VisualInstance_property_layers>` | ``1`` |
+-----------------------+-----------------------------------------------------+-------+

Métodos
--------------

+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>` | :ref:`get_aabb<class_VisualInstance_method_get_aabb>` **(** **)** |const|                                                                          |
+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_RID>`   | :ref:`get_base<class_VisualInstance_method_get_base>` **(** **)** |const|                                                                          |
+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_RID>`   | :ref:`get_instance<class_VisualInstance_method_get_instance>` **(** **)** |const|                                                                  |
+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>` | :ref:`get_layer_mask_bit<class_VisualInstance_method_get_layer_mask_bit>` **(** :ref:`int<class_int>` layer **)** |const|                          |
+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>` | :ref:`get_transformed_aabb<class_VisualInstance_method_get_transformed_aabb>` **(** **)** |const|                                                  |
+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| void                    | :ref:`set_base<class_VisualInstance_method_set_base>` **(** :ref:`RID<class_RID>` base **)**                                                       |
+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
| void                    | :ref:`set_layer_mask_bit<class_VisualInstance_method_set_layer_mask_bit>` **(** :ref:`int<class_int>` layer, :ref:`bool<class_bool>` enabled **)** |
+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------+

Descripciones de Propiedades
--------------------------------------------------------

.. _class_VisualInstance_property_layers:

- :ref:`int<class_int>` **layers**

+-----------+-----------------------+
| *Default* | ``1``                 |
+-----------+-----------------------+
| *Setter*  | set_layer_mask(value) |
+-----------+-----------------------+
| *Getter*  | get_layer_mask()      |
+-----------+-----------------------+

La capa(s) de representación sobre la que se dibuja este ``VisualInstance``.

Este objeto sólo será visible para :ref:`Camera<class_Camera>` cuya máscara de selección incluya el objeto renderizado que este ``VisualInstance`` tiene configurado.

Descripciones de Métodos
------------------------------------------------

.. _class_VisualInstance_method_get_aabb:

- :ref:`AABB<class_AABB>` **get_aabb** **(** **)** |const|

Devuelve el :ref:`AABB<class_AABB>` (también conocido como el cuadro delimitador) para este ``VisualInstance``. Ver también :ref:`get_transformed_aabb<class_VisualInstance_method_get_transformed_aabb>`.

----

.. _class_VisualInstance_method_get_base:

- :ref:`RID<class_RID>` **get_base** **(** **)** |const|

Devuelve el RID del recurso asociado a este ``VisualInstance``. Por ejemplo, si el Nodo es un :ref:`MeshInstance<class_MeshInstance>`, esto devolverá el RID del :ref:`Mesh<class_Mesh>` asociado.

----

.. _class_VisualInstance_method_get_instance:

- :ref:`RID<class_RID>` **get_instance** **(** **)** |const|

Devuelve el RID de esta instancia. Este RID es el mismo que el RID devuelto por :ref:`VisualServer.instance_create<class_VisualServer_method_instance_create>`. Este RID es necesario si quieres llamar a las funciones de :ref:`VisualServer<class_VisualServer>` directamente en este ``VisualInstance``.

----

.. _class_VisualInstance_method_get_layer_mask_bit:

- :ref:`bool<class_bool>` **get_layer_mask_bit** **(** :ref:`int<class_int>` layer **)** |const|

Devuelve ``true`` cuando la capa especificada está activada en :ref:`layers<class_VisualInstance_property_layers>` y ``false`` en caso contrario.

----

.. _class_VisualInstance_method_get_transformed_aabb:

- :ref:`AABB<class_AABB>` **get_transformed_aabb** **(** **)** |const|

Devuelve el :ref:`AABB<class_AABB>` transformado (también conocido como el cuadro delimitador) para este ``VisualInstance``.

Transformado en este caso significa el :ref:`AABB<class_AABB>` más la posición, rotación y escala de la :ref:`Transform<class_Transform>` del :ref:`Spatial<class_Spatial>`. Ver también :ref:`get_aabb<class_VisualInstance_method_get_aabb>`.

----

.. _class_VisualInstance_method_set_base:

- void **set_base** **(** :ref:`RID<class_RID>` base **)**

Establece el recurso que es instanciado por este ``VisualInstance``, que cambia la forma en que el motor maneja el ``VisualInstance`` bajo el capó. Equivalente al :ref:`VisualServer.instance_set_base<class_VisualServer_method_instance_set_base>`.

----

.. _class_VisualInstance_method_set_layer_mask_bit:

- void **set_layer_mask_bit** **(** :ref:`int<class_int>` layer, :ref:`bool<class_bool>` enabled **)**

Permite una capa particular en :ref:`layers<class_VisualInstance_property_layers>`.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
