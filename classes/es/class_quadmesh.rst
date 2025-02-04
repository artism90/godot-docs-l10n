:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the QuadMesh.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_QuadMesh:

QuadMesh
========

**Inherits:** :ref:`PrimitiveMesh<class_PrimitiveMesh>` **<** :ref:`Mesh<class_Mesh>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Clase que representa una malla cuadrada.

Descripción
----------------------

Clase que representa un cuadrado :ref:`PrimitiveMesh<class_PrimitiveMesh>`. Esta malla plana no tiene espesor. Por defecto, esta malla está alineada en los ejes X e Y; esta rotación por defecto es más adecuada para su uso con materiales de cartelería. A diferencia de :ref:`PlaneMesh<class_PlaneMesh>`, esta malla no proporciona opciones de subdivisión.

Tutoriales
--------------------

- `GUI in 3D Demo <https://godotengine.org/asset-library/asset/127>`__

- `2D in 3D Demo <https://godotengine.org/asset-library/asset/129>`__

Propiedades
----------------------

+-------------------------------+-------------------------------------------------------------+------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`center_offset<class_QuadMesh_property_center_offset>` | ``Vector3( 0, 0, 0 )`` |
+-------------------------------+-------------------------------------------------------------+------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`size<class_QuadMesh_property_size>`                   | ``Vector2( 1, 1 )``    |
+-------------------------------+-------------------------------------------------------------+------------------------+

Descripciones de Propiedades
--------------------------------------------------------

.. _class_QuadMesh_property_center_offset:

- :ref:`Vector3<class_Vector3>` **center_offset**

+-----------+--------------------------+
| *Default* | ``Vector3( 0, 0, 0 )``   |
+-----------+--------------------------+
| *Setter*  | set_center_offset(value) |
+-----------+--------------------------+
| *Getter*  | get_center_offset()      |
+-----------+--------------------------+

Offset of the generated Quad. Useful for particles.

----

.. _class_QuadMesh_property_size:

- :ref:`Vector2<class_Vector2>` **size**

+-----------+---------------------+
| *Default* | ``Vector2( 1, 1 )`` |
+-----------+---------------------+
| *Setter*  | set_size(value)     |
+-----------+---------------------+
| *Getter*  | get_size()          |
+-----------+---------------------+

Tamaño en los ejes X e Y.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
