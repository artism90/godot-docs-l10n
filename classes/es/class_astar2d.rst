:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the AStar2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_AStar2D:

AStar2D
=======

**Inherits:** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Representacion de la clase AStar que usa vectores 2D como lados.

Descripción
----------------------

Este es un envoltorio para la clase :ref:`AStar<class_AStar>` el cual usa vectores 2D en vez de 3D Vectors.

Métodos
--------------

+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                       | :ref:`_compute_cost<class_AStar2D_method__compute_cost>` **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)** |virtual|                                      |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                       | :ref:`_estimate_cost<class_AStar2D_method__estimate_cost>` **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)** |virtual|                                    |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`add_point<class_AStar2D_method_add_point>` **(** :ref:`int<class_int>` id, :ref:`Vector2<class_Vector2>` position, :ref:`float<class_float>` weight_scale=1.0 **)**      |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                         | :ref:`are_points_connected<class_AStar2D_method_are_points_connected>` **(** :ref:`int<class_int>` id, :ref:`int<class_int>` to_id **)** |const|                               |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`clear<class_AStar2D_method_clear>` **(** **)**                                                                                                                           |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`connect_points<class_AStar2D_method_connect_points>` **(** :ref:`int<class_int>` id, :ref:`int<class_int>` to_id, :ref:`bool<class_bool>` bidirectional=true **)**       |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`disconnect_points<class_AStar2D_method_disconnect_points>` **(** :ref:`int<class_int>` id, :ref:`int<class_int>` to_id **)**                                             |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                           | :ref:`get_available_point_id<class_AStar2D_method_get_available_point_id>` **(** **)** |const|                                                                                 |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                           | :ref:`get_closest_point<class_AStar2D_method_get_closest_point>` **(** :ref:`Vector2<class_Vector2>` to_position, :ref:`bool<class_bool>` include_disabled=false **)** |const| |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`get_closest_position_in_segment<class_AStar2D_method_get_closest_position_in_segment>` **(** :ref:`Vector2<class_Vector2>` to_position **)** |const|                     |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolIntArray<class_PoolIntArray>`         | :ref:`get_id_path<class_AStar2D_method_get_id_path>` **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)**                                                    |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                           | :ref:`get_point_capacity<class_AStar2D_method_get_point_capacity>` **(** **)** |const|                                                                                         |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolIntArray<class_PoolIntArray>`         | :ref:`get_point_connections<class_AStar2D_method_get_point_connections>` **(** :ref:`int<class_int>` id **)**                                                                  |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                           | :ref:`get_point_count<class_AStar2D_method_get_point_count>` **(** **)** |const|                                                                                               |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolVector2Array<class_PoolVector2Array>` | :ref:`get_point_path<class_AStar2D_method_get_point_path>` **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)**                                              |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                   | :ref:`get_point_position<class_AStar2D_method_get_point_position>` **(** :ref:`int<class_int>` id **)** |const|                                                                |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                       | :ref:`get_point_weight_scale<class_AStar2D_method_get_point_weight_scale>` **(** :ref:`int<class_int>` id **)** |const|                                                        |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`                       | :ref:`get_points<class_AStar2D_method_get_points>` **(** **)**                                                                                                                 |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                         | :ref:`has_point<class_AStar2D_method_has_point>` **(** :ref:`int<class_int>` id **)** |const|                                                                                  |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                         | :ref:`is_point_disabled<class_AStar2D_method_is_point_disabled>` **(** :ref:`int<class_int>` id **)** |const|                                                                  |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`remove_point<class_AStar2D_method_remove_point>` **(** :ref:`int<class_int>` id **)**                                                                                    |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`reserve_space<class_AStar2D_method_reserve_space>` **(** :ref:`int<class_int>` num_nodes **)**                                                                           |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`set_point_disabled<class_AStar2D_method_set_point_disabled>` **(** :ref:`int<class_int>` id, :ref:`bool<class_bool>` disabled=true **)**                                 |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`set_point_position<class_AStar2D_method_set_point_position>` **(** :ref:`int<class_int>` id, :ref:`Vector2<class_Vector2>` position **)**                                |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`set_point_weight_scale<class_AStar2D_method_set_point_weight_scale>` **(** :ref:`int<class_int>` id, :ref:`float<class_float>` weight_scale **)**                        |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Descripciones de Métodos
------------------------------------------------

.. _class_AStar2D_method__compute_cost:

- :ref:`float<class_float>` **_compute_cost** **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)** |virtual|

Llamado cuando se calcula el coste entre dos puntos conectados.

Nota que esta funcion esta oculta en la clase ``AStar2D`` por defecto.

----

.. _class_AStar2D_method__estimate_cost:

- :ref:`float<class_float>` **_estimate_cost** **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)** |virtual|

Llamado cuando se calcula el coste entre un punto el final de un punto de una ruta.

Nota que esta funcion esta oculta en la clase ``AStar2D`` por defecto.

----

.. _class_AStar2D_method_add_point:

- void **add_point** **(** :ref:`int<class_int>` id, :ref:`Vector2<class_Vector2>` position, :ref:`float<class_float>` weight_scale=1.0 **)**

Adds a new point at the given position with the given identifier. The ``id`` must be 0 or larger, and the ``weight_scale`` must be 1 or larger.

The ``weight_scale`` is multiplied by the result of :ref:`_compute_cost<class_AStar2D_method__compute_cost>` when determining the overall cost of traveling across a segment from a neighboring point to this point. Thus, all else being equal, the algorithm prefers points with lower ``weight_scale``\ s to form a path.

::

    var astar = AStar2D.new()
    astar.add_point(1, Vector2(1, 0), 4) # Adds the point (1, 0) with weight_scale 4 and id 1

If there already exists a point for the given ``id``, its position and weight scale are updated to the given values.

----

.. _class_AStar2D_method_are_points_connected:

- :ref:`bool<class_bool>` **are_points_connected** **(** :ref:`int<class_int>` id, :ref:`int<class_int>` to_id **)** |const|

Devuelve si hay una conexion/segmento entre los puntos dados.

----

.. _class_AStar2D_method_clear:

- void **clear** **(** **)**

Limpia todos los puntos y segmentos.

----

.. _class_AStar2D_method_connect_points:

- void **connect_points** **(** :ref:`int<class_int>` id, :ref:`int<class_int>` to_id, :ref:`bool<class_bool>` bidirectional=true **)**

Crea un segmento entre los puntos dados. Si ``bidirectional`` es ``false``, solo el movimiento desde ``id`` a ``to_id`` es permitido, no la direccion inversa.

::

    var astar = AStar2D.new()
    astar.add_point(1, Vector2(1, 1))
    astar.add_point(2, Vector(0, 5))
    astar.connect_points(1, 2, false)

----

.. _class_AStar2D_method_disconnect_points:

- void **disconnect_points** **(** :ref:`int<class_int>` id, :ref:`int<class_int>` to_id **)**

Elimina el segmento entre los puntos dados.

----

.. _class_AStar2D_method_get_available_point_id:

- :ref:`int<class_int>` **get_available_point_id** **(** **)** |const|

Devuelve el punto de Ide proximo disponible con ningun punto asociado a el.

----

.. _class_AStar2D_method_get_closest_point:

- :ref:`int<class_int>` **get_closest_point** **(** :ref:`Vector2<class_Vector2>` to_position, :ref:`bool<class_bool>` include_disabled=false **)** |const|

Devuelve el ID del punto mas cercano a ``to_position``, opcionalmente tomando puntos deshabilitados en cuenta. Devuelve ``-1`` si no hay puntos el grupo(pool) de puntos.

\ **Nota:** Si varios puntos son los más cercanos a ``to_position``, el pundo con el menor ID será devuelto, asegurando un resultado deterministico.

----

.. _class_AStar2D_method_get_closest_position_in_segment:

- :ref:`Vector2<class_Vector2>` **get_closest_position_in_segment** **(** :ref:`Vector2<class_Vector2>` to_position **)** |const|

Devuelve el punto mas cercano a ``to_position`` que reside dentro de un segmento entre dos puntos conectados.

::

    var astar = AStar2D.new()
    astar.add_point(1, Vector2(0, 0))
    astar.add_point(2, Vector2(0, 5))
    astar.connect_points(1,2)
    var res = astar.get_closest_position_in_segment(Vector2(3, 3)) # Devuelve (0, 3)

El resultado esta dentro del segmento que van desde ``y = 0`` a ``y = 5``. Es la posicion mas cercana en el segmento al punto dado.

----

.. _class_AStar2D_method_get_id_path:

- :ref:`PoolIntArray<class_PoolIntArray>` **get_id_path** **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)**

Devuelve un array con los IDs de los puntos que forman la ruta encontrada por AStar2D entre los puntos dados. El array es ordenado desde el punto inicial al punto final de la ruta.

::

    var astar = AStar2D.new()
    astar.add_point(1, Vector2(0,0))
    astar.add_point(2, Vertor2(0, 1), 1) # Por defecto el peso es 1
    astar.add_point(3, Vector2(1, 1))
    astar.add_point(4, Vector2(2,0))
    
    astar.connect_points(1, 2, false)
    astar.connect_points(2, 3, false)
    astar.connect_points(4, 3, false)
    astar.connect_points(1, 4, false)
    
    var res = astar.get_id_path(1, 3) # Devuelve [1, 2, 3]

Si tu cambias el peso del segundo punto a 3, entonces el resultado sera ``[1, 4, 3]``, porque ahora aunque la distancia es mayor, cuesta menos ir a traves del punto 4 que des punto 2.

----

.. _class_AStar2D_method_get_point_capacity:

- :ref:`int<class_int>` **get_point_capacity** **(** **)** |const|

Devuelve la capacidad de la estructura que respalda los puntos, usado junto con ``reserve_space``.

----

.. _class_AStar2D_method_get_point_connections:

- :ref:`PoolIntArray<class_PoolIntArray>` **get_point_connections** **(** :ref:`int<class_int>` id **)**

Devuelve un array con los IDs de los puntos que forman la conexion con los puntos dados.

::

    var astar = AStar2D.new()
    astar.add_point(1, Vector2(0, 0))
    astar.add_point(2, Vector2(0, 1))
    astar.add_point(3, Vector2(1, 1))
    astar.add_point(4, Vector2(2, 0))
    
    astar.connect_points(1, 2, true)
    astar.connect_points(1, 3, true)
    
    var vecinos = astar.get_point_connections(1) # Devuelve [2, 3]

----

.. _class_AStar2D_method_get_point_count:

- :ref:`int<class_int>` **get_point_count** **(** **)** |const|

Devuelve el numero de puntos actualmente en el grupo(pool) de puntos.

----

.. _class_AStar2D_method_get_point_path:

- :ref:`PoolVector2Array<class_PoolVector2Array>` **get_point_path** **(** :ref:`int<class_int>` from_id, :ref:`int<class_int>` to_id **)**

Returns an array with the points that are in the path found by AStar2D between the given points. The array is ordered from the starting point to the ending point of the path.

\ **Note:** This method is not thread-safe. If called from a :ref:`Thread<class_Thread>`, it will return an empty :ref:`PoolVector2Array<class_PoolVector2Array>` and will print an error message.

----

.. _class_AStar2D_method_get_point_position:

- :ref:`Vector2<class_Vector2>` **get_point_position** **(** :ref:`int<class_int>` id **)** |const|

Devuelve la posicion del punto asociado con el ``id`` dado.

----

.. _class_AStar2D_method_get_point_weight_scale:

- :ref:`float<class_float>` **get_point_weight_scale** **(** :ref:`int<class_int>` id **)** |const|

Devuelve el peso del punto asociado con el ``id`` dado.

----

.. _class_AStar2D_method_get_points:

- :ref:`Array<class_Array>` **get_points** **(** **)**

Devuelve un array con todos los puntos.

----

.. _class_AStar2D_method_has_point:

- :ref:`bool<class_bool>` **has_point** **(** :ref:`int<class_int>` id **)** |const|

Devuelve si un punto asociado con el ``id`` existe.

----

.. _class_AStar2D_method_is_point_disabled:

- :ref:`bool<class_bool>` **is_point_disabled** **(** :ref:`int<class_int>` id **)** |const|

Devuelve si un punto esta deshabilitado or no para el buscador de rutas. Por defecto, todos los puntos estan habilitados.

----

.. _class_AStar2D_method_remove_point:

- void **remove_point** **(** :ref:`int<class_int>` id **)**

Elimina el punto asociado con el ``id`` dado del grupo(pool) de puntos.

----

.. _class_AStar2D_method_reserve_space:

- void **reserve_space** **(** :ref:`int<class_int>` num_nodes **)**

Espacio de reserva interna para puntos ``num_nodes``, util si tu estas añadiendo un gran numero de puntos a la vez, para un grid por ejemplo. Las nuevas capacidades debes ser mayores o iguales que la anterior capacidad.

----

.. _class_AStar2D_method_set_point_disabled:

- void **set_point_disabled** **(** :ref:`int<class_int>` id, :ref:`bool<class_bool>` disabled=true **)**

Deshabilita o habilita el punto especificado para el buscador de rutas. Util para crear obstaculos temporales.

----

.. _class_AStar2D_method_set_point_position:

- void **set_point_position** **(** :ref:`int<class_int>` id, :ref:`Vector2<class_Vector2>` position **)**

Coloca la ``position`` para el punto con el ``id`` dado.

----

.. _class_AStar2D_method_set_point_weight_scale:

- void **set_point_weight_scale** **(** :ref:`int<class_int>` id, :ref:`float<class_float>` weight_scale **)**

Sets the ``weight_scale`` for the point with the given ``id``. The ``weight_scale`` is multiplied by the result of :ref:`_compute_cost<class_AStar2D_method__compute_cost>` when determining the overall cost of traveling across a segment from a neighboring point to this point.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
