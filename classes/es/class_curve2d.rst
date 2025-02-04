:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Curve2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Curve2D:

Curve2D
=======

**Inherits:** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Describe una curva de Bézier en el espacio 2D.

Descripción
----------------------

Esta clase describe una curva de Bézier en el espacio 2D. Se utiliza principalmente para dar una forma a un :ref:`Path2D<class_Path2D>`, pero puede ser muestreada manualmente para otros propósitos.

Mantiene un cacheo de puntos precalculados a lo largo de la curva, para acelerar los cálculos.

Propiedades
----------------------

+---------------------------+------------------------------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`bake_interval<class_Curve2D_property_bake_interval>` | ``5.0`` |
+---------------------------+------------------------------------------------------------+---------+

Métodos
--------------

+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`add_point<class_Curve2D_method_add_point>` **(** :ref:`Vector2<class_Vector2>` position, :ref:`Vector2<class_Vector2>` in=Vector2( 0, 0 ), :ref:`Vector2<class_Vector2>` out=Vector2( 0, 0 ), :ref:`int<class_int>` at_position=-1 **)** |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`clear_points<class_Curve2D_method_clear_points>` **(** **)**                                                                                                                                                                             |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                       | :ref:`get_baked_length<class_Curve2D_method_get_baked_length>` **(** **)** |const|                                                                                                                                                             |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolVector2Array<class_PoolVector2Array>` | :ref:`get_baked_points<class_Curve2D_method_get_baked_points>` **(** **)** |const|                                                                                                                                                             |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                       | :ref:`get_closest_offset<class_Curve2D_method_get_closest_offset>` **(** :ref:`Vector2<class_Vector2>` to_point **)** |const|                                                                                                                  |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`get_closest_point<class_Curve2D_method_get_closest_point>` **(** :ref:`Vector2<class_Vector2>` to_point **)** |const|                                                                                                                    |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                           | :ref:`get_point_count<class_Curve2D_method_get_point_count>` **(** **)** |const|                                                                                                                                                               |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`get_point_in<class_Curve2D_method_get_point_in>` **(** :ref:`int<class_int>` idx **)** |const|                                                                                                                                           |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`get_point_out<class_Curve2D_method_get_point_out>` **(** :ref:`int<class_int>` idx **)** |const|                                                                                                                                         |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`get_point_position<class_Curve2D_method_get_point_position>` **(** :ref:`int<class_int>` idx **)** |const|                                                                                                                               |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`interpolate<class_Curve2D_method_interpolate>` **(** :ref:`int<class_int>` idx, :ref:`float<class_float>` t **)** |const|                                                                                                                |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`interpolate_baked<class_Curve2D_method_interpolate_baked>` **(** :ref:`float<class_float>` offset, :ref:`bool<class_bool>` cubic=false **)** |const|                                                                                     |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`interpolatef<class_Curve2D_method_interpolatef>` **(** :ref:`float<class_float>` fofs **)** |const|                                                                                                                                      |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`remove_point<class_Curve2D_method_remove_point>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                   |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`set_point_in<class_Curve2D_method_set_point_in>` **(** :ref:`int<class_int>` idx, :ref:`Vector2<class_Vector2>` position **)**                                                                                                           |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`set_point_out<class_Curve2D_method_set_point_out>` **(** :ref:`int<class_int>` idx, :ref:`Vector2<class_Vector2>` position **)**                                                                                                         |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`set_point_position<class_Curve2D_method_set_point_position>` **(** :ref:`int<class_int>` idx, :ref:`Vector2<class_Vector2>` position **)**                                                                                               |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolVector2Array<class_PoolVector2Array>` | :ref:`tessellate<class_Curve2D_method_tessellate>` **(** :ref:`int<class_int>` max_stages=5, :ref:`float<class_float>` tolerance_degrees=4 **)** |const|                                                                                       |
+-------------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Descripciones de Propiedades
--------------------------------------------------------

.. _class_Curve2D_property_bake_interval:

- :ref:`float<class_float>` **bake_interval**

+-----------+--------------------------+
| *Default* | ``5.0``                  |
+-----------+--------------------------+
| *Setter*  | set_bake_interval(value) |
+-----------+--------------------------+
| *Getter*  | get_bake_interval()      |
+-----------+--------------------------+

La distancia en píxeles entre dos puntos cacheados adyacentes. Cambiarlo obliga a recomponer la caché la próxima vez que se llame a la función :ref:`get_baked_points<class_Curve2D_method_get_baked_points>` o :ref:`get_baked_length<class_Curve2D_method_get_baked_length>`. Cuanto menor sea la distancia, más puntos en el cache y más memoria consumirá, así que úsala con cuidado.

Descripciones de Métodos
------------------------------------------------

.. _class_Curve2D_method_add_point:

- void **add_point** **(** :ref:`Vector2<class_Vector2>` position, :ref:`Vector2<class_Vector2>` in=Vector2( 0, 0 ), :ref:`Vector2<class_Vector2>` out=Vector2( 0, 0 ), :ref:`int<class_int>` at_position=-1 **)**

Añade un punto a una curva en la posición ``position``, con puntos de control ``in`` y ``out``.

Si se da ``at_position``, el punto se inserta antes del número de punto ``at_position``, desplazando ese punto (y todos los puntos posteriores) después del punto insertado. Si no se da ``at_position``, o es un valor ilegal (``at_position <0`` o ``at_position >= [method get_point_count]``), el punto se añadirá al final de la lista de puntos.

----

.. _class_Curve2D_method_clear_points:

- void **clear_points** **(** **)**

Elimina todos los puntos de la curva.

----

.. _class_Curve2D_method_get_baked_length:

- :ref:`float<class_float>` **get_baked_length** **(** **)** |const|

Devuelve la longitud total de la curva, basada en los puntos cacheados. Si se le da suficiente densidad (ver :ref:`bake_interval<class_Curve2D_property_bake_interval>`), debe ser bastante aproximada.

----

.. _class_Curve2D_method_get_baked_points:

- :ref:`PoolVector2Array<class_PoolVector2Array>` **get_baked_points** **(** **)** |const|

Returns the cache of points as a :ref:`PoolVector2Array<class_PoolVector2Array>`.

----

.. _class_Curve2D_method_get_closest_offset:

- :ref:`float<class_float>` **get_closest_offset** **(** :ref:`Vector2<class_Vector2>` to_point **)** |const|

Devuelve el desplazamiento más cercano a ``to_point``. Este desplazamiento está destinado a ser utilizado en :ref:`interpolate_baked<class_Curve2D_method_interpolate_baked>`.

\ ``to_point`` debe estar en el espacio local de esta curva.

----

.. _class_Curve2D_method_get_closest_point:

- :ref:`Vector2<class_Vector2>` **get_closest_point** **(** :ref:`Vector2<class_Vector2>` to_point **)** |const|

Returns the closest baked point (in curve's local space) to ``to_point``.

\ ``to_point`` must be in this curve's local space.

----

.. _class_Curve2D_method_get_point_count:

- :ref:`int<class_int>` **get_point_count** **(** **)** |const|

Devuelve el número de puntos que describen la curva.

----

.. _class_Curve2D_method_get_point_in:

- :ref:`Vector2<class_Vector2>` **get_point_in** **(** :ref:`int<class_int>` idx **)** |const|

Returns the position of the control point leading to the vertex ``idx``. The returned position is relative to the vertex ``idx``. If the index is out of bounds, the function sends an error to the console, and returns ``(0, 0)``.

----

.. _class_Curve2D_method_get_point_out:

- :ref:`Vector2<class_Vector2>` **get_point_out** **(** :ref:`int<class_int>` idx **)** |const|

Returns the position of the control point leading out of the vertex ``idx``. The returned position is relative to the vertex ``idx``. If the index is out of bounds, the function sends an error to the console, and returns ``(0, 0)``.

----

.. _class_Curve2D_method_get_point_position:

- :ref:`Vector2<class_Vector2>` **get_point_position** **(** :ref:`int<class_int>` idx **)** |const|

Devuelve la posición del vértice ``idx``. Si el índice está fuera de los límites, la función envía un error a la consola, y devuelve ``(0, 0)``.

----

.. _class_Curve2D_method_interpolate:

- :ref:`Vector2<class_Vector2>` **interpolate** **(** :ref:`int<class_int>` idx, :ref:`float<class_float>` t **)** |const|

Devuelve la posición entre el vértice ``idx`` y el vértice ``idx + 1``, donde ``t`` controla si el punto es el primer vértice (``t = 0.0``), el último vértice (``t = 1.0``), o en medio. Los valores de ``t`` fuera del rango (``0.0 >= t <=1``) dan resultados extraños, pero predecibles.

Si ``idx`` está fuera de los límites se trunca el primer o último vértice, y ``t`` se ignora. Si la curva no tiene puntos, la función envía un error a la consola, y devuelve ``(0, 0)``.

----

.. _class_Curve2D_method_interpolate_baked:

- :ref:`Vector2<class_Vector2>` **interpolate_baked** **(** :ref:`float<class_float>` offset, :ref:`bool<class_bool>` cubic=false **)** |const|

Devuelve un punto dentro de la curva en la posición ``offset``, donde ``offset`` se mide como una distancia en píxeles a lo largo de la curva.

Para ello, encuentra los dos puntos en caché entre los que se encuentra ``offset``, e interpola los valores. Esta interpolación es cúbica si ``cubic`` se establece en ``true``, o lineal si se establece en ``false``.

La interpolación cúbica tiende a seguir mejor las curvas, pero la lineal es más rápida (y a menudo, suficientemente precisa).

----

.. _class_Curve2D_method_interpolatef:

- :ref:`Vector2<class_Vector2>` **interpolatef** **(** :ref:`float<class_float>` fofs **)** |const|

Devuelve la posición en el vértice ``fofs``. Llama a :ref:`interpolate<class_Curve2D_method_interpolate>` usando la parte entera de ``fofs`` como ``idx``, y su parte fraccionaria como ``t``.

----

.. _class_Curve2D_method_remove_point:

- void **remove_point** **(** :ref:`int<class_int>` idx **)**

Suprime el punto ``idx`` de la curva. Envía un error a la consola si ``idx`` está fuera de los límites.

----

.. _class_Curve2D_method_set_point_in:

- void **set_point_in** **(** :ref:`int<class_int>` idx, :ref:`Vector2<class_Vector2>` position **)**

Sets the position of the control point leading to the vertex ``idx``. If the index is out of bounds, the function sends an error to the console. The position is relative to the vertex.

----

.. _class_Curve2D_method_set_point_out:

- void **set_point_out** **(** :ref:`int<class_int>` idx, :ref:`Vector2<class_Vector2>` position **)**

Sets the position of the control point leading out of the vertex ``idx``. If the index is out of bounds, the function sends an error to the console. The position is relative to the vertex.

----

.. _class_Curve2D_method_set_point_position:

- void **set_point_position** **(** :ref:`int<class_int>` idx, :ref:`Vector2<class_Vector2>` position **)**

Establece la posición del vértice ``idx``. Si el índice está fuera de los límites, la función envía un error a la consola.

----

.. _class_Curve2D_method_tessellate:

- :ref:`PoolVector2Array<class_PoolVector2Array>` **tessellate** **(** :ref:`int<class_int>` max_stages=5, :ref:`float<class_float>` tolerance_degrees=4 **)** |const|

Devuelve una lista de puntos a lo largo de la curva, con una densidad de puntos controlada por la curvatura. Es decir, las partes más curvadas tendrán más puntos que las partes más rectas.

Esta aproximación hace segmentos rectos entre cada punto, luego subdivide esos segmentos hasta que la forma resultante es lo suficientemente similar.

\ ``max_stages`` controla cuántas subdivisiones puede afrontar un segmento de curva antes de que se considere suficientemente aproximado. Cada subdivisión divide el segmento por la mitad, por lo que las 5 etapas predeterminadas pueden significar hasta 32 subdivisiones por segmento de curva. Aumenta con cuidado!

\ ``tolerance_degrees`` controla cuántos grados puede desviarse el punto medio de un segmento de la curva real, antes de que el segmento tenga que ser subdividido.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
