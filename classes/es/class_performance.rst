:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Performance.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Performance:

Performance
===========

**Inherits:** :ref:`Object<class_Object>`

Expone los datos relacionados con el rendimiento.

Descripción
----------------------

This class provides access to a number of different monitors related to performance, such as memory usage, draw calls, and FPS. These are the same as the values displayed in the **Monitor** tab in the editor's **Debugger** panel. By using the :ref:`get_monitor<class_Performance_method_get_monitor>` method of this class, you can access this data from your code.

\ **Note:** A few of these monitors are only available in debug mode and will always return 0 when used in a release build.

\ **Note:** Many of these monitors are not updated in real-time, so there may be a short delay between changes.

Métodos
--------------

+---------------------------+-------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`get_monitor<class_Performance_method_get_monitor>` **(** :ref:`Monitor<enum_Performance_Monitor>` monitor **)** |const| |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------+

Enumeraciones
--------------------------

.. _enum_Performance_Monitor:

.. _class_Performance_constant_TIME_FPS:

.. _class_Performance_constant_TIME_PROCESS:

.. _class_Performance_constant_TIME_PHYSICS_PROCESS:

.. _class_Performance_constant_MEMORY_STATIC:

.. _class_Performance_constant_MEMORY_DYNAMIC:

.. _class_Performance_constant_MEMORY_STATIC_MAX:

.. _class_Performance_constant_MEMORY_DYNAMIC_MAX:

.. _class_Performance_constant_MEMORY_MESSAGE_BUFFER_MAX:

.. _class_Performance_constant_OBJECT_COUNT:

.. _class_Performance_constant_OBJECT_RESOURCE_COUNT:

.. _class_Performance_constant_OBJECT_NODE_COUNT:

.. _class_Performance_constant_OBJECT_ORPHAN_NODE_COUNT:

.. _class_Performance_constant_RENDER_OBJECTS_IN_FRAME:

.. _class_Performance_constant_RENDER_VERTICES_IN_FRAME:

.. _class_Performance_constant_RENDER_MATERIAL_CHANGES_IN_FRAME:

.. _class_Performance_constant_RENDER_SHADER_CHANGES_IN_FRAME:

.. _class_Performance_constant_RENDER_SURFACE_CHANGES_IN_FRAME:

.. _class_Performance_constant_RENDER_DRAW_CALLS_IN_FRAME:

.. _class_Performance_constant_RENDER_2D_ITEMS_IN_FRAME:

.. _class_Performance_constant_RENDER_2D_DRAW_CALLS_IN_FRAME:

.. _class_Performance_constant_RENDER_VIDEO_MEM_USED:

.. _class_Performance_constant_RENDER_TEXTURE_MEM_USED:

.. _class_Performance_constant_RENDER_VERTEX_MEM_USED:

.. _class_Performance_constant_RENDER_USAGE_VIDEO_MEM_TOTAL:

.. _class_Performance_constant_PHYSICS_2D_ACTIVE_OBJECTS:

.. _class_Performance_constant_PHYSICS_2D_COLLISION_PAIRS:

.. _class_Performance_constant_PHYSICS_2D_ISLAND_COUNT:

.. _class_Performance_constant_PHYSICS_3D_ACTIVE_OBJECTS:

.. _class_Performance_constant_PHYSICS_3D_COLLISION_PAIRS:

.. _class_Performance_constant_PHYSICS_3D_ISLAND_COUNT:

.. _class_Performance_constant_AUDIO_OUTPUT_LATENCY:

.. _class_Performance_constant_MONITOR_MAX:

enum **Monitor**:

- **TIME_FPS** = **0** --- Número de fotogramas por segundo.

- **TIME_PROCESS** = **1** --- El tiempo que tomó completar un fotograma, en segundos.

- **TIME_PHYSICS_PROCESS** = **2** --- El tiempo que tomó completar un fotograma de la física, en segundos.

- **MEMORY_STATIC** = **3** --- Memoria estática actualmente utilizada, en bytes. No está disponible en las versiones de lanzamiento.

- **MEMORY_DYNAMIC** = **4** --- Dynamic memory currently used, in bytes. Not available in release builds.

- **MEMORY_STATIC_MAX** = **5** --- Memoria estática disponible. No disponible en las builds release.

- **MEMORY_DYNAMIC_MAX** = **6** --- Available dynamic memory. Not available in release builds.

- **MEMORY_MESSAGE_BUFFER_MAX** = **7** --- La mayor cantidad de memoria que el buffer de la cola de mensajes ha usado, en bytes. La cola de mensajes se utiliza para llamadas y notificaciones de funciones diferidas.

- **OBJECT_COUNT** = **8** --- Número de objetos actualmente instanciados (incluyendo nodos).

- **OBJECT_RESOURCE_COUNT** = **9** --- Número de recursos utilizados actualmente.

- **OBJECT_NODE_COUNT** = **10** --- Número de nodos actualmente instanciados en el árbol de la escena. Esto también incluye el nodo raíz.

- **OBJECT_ORPHAN_NODE_COUNT** = **11** --- Número de nodos huérfanos, es decir, nodos que no están engendrados en un nodo del árbol de la escena.

- **RENDER_OBJECTS_IN_FRAME** = **12** --- Objetos 3D dibujados por fotograma.

- **RENDER_VERTICES_IN_FRAME** = **13** --- Vértices dibujados por fotograma. Sólo en 3D.

- **RENDER_MATERIAL_CHANGES_IN_FRAME** = **14** --- Cambios de material por fotograma. Sólo en 3D.

- **RENDER_SHADER_CHANGES_IN_FRAME** = **15** --- Cambios de shader por fotograma. Sólo en 3D.

- **RENDER_SURFACE_CHANGES_IN_FRAME** = **16** --- Cambios en la superficie de renderizado por fotograma. Sólo en 3D.

- **RENDER_DRAW_CALLS_IN_FRAME** = **17** --- Llamadas a dibujar por fotograma. Sólo en 3D.

- **RENDER_2D_ITEMS_IN_FRAME** = **18** --- Items or joined items drawn per frame.

- **RENDER_2D_DRAW_CALLS_IN_FRAME** = **19** --- Draw calls per frame.

- **RENDER_VIDEO_MEM_USED** = **20** --- La cantidad de memoria de vídeo utilizada, es decir, la memoria de texturas y vértices combinados.

- **RENDER_TEXTURE_MEM_USED** = **21** --- La cantidad de memoria de textura utilizada.

- **RENDER_VERTEX_MEM_USED** = **22** --- La cantidad de memoria de vértices utilizada.

- **RENDER_USAGE_VIDEO_MEM_TOTAL** = **23** --- Unimplemented in the GLES2 and GLES3 rendering backends, always returns 0.

- **PHYSICS_2D_ACTIVE_OBJECTS** = **24** --- Número de nodos activos :ref:`RigidBody2D<class_RigidBody2D>` en el juego.

- **PHYSICS_2D_COLLISION_PAIRS** = **25** --- Número de pares de colisión en el motor de física 2D.

- **PHYSICS_2D_ISLAND_COUNT** = **26** --- Número de islas en el motor de física 2D.

- **PHYSICS_3D_ACTIVE_OBJECTS** = **27** --- Number of active :ref:`RigidBody<class_RigidBody>` and :ref:`VehicleBody<class_VehicleBody>` nodes in the game.

- **PHYSICS_3D_COLLISION_PAIRS** = **28** --- Número de pares de colisión en el motor de física 3D.

- **PHYSICS_3D_ISLAND_COUNT** = **29** --- Número de islas en el motor de física 3D.

- **AUDIO_OUTPUT_LATENCY** = **30** --- La latencia de salida del :ref:`AudioServer<class_AudioServer>`.

- **MONITOR_MAX** = **31** --- Representa el tamaño del enum :ref:`Monitor<enum_Performance_Monitor>`.

Descripciones de Métodos
------------------------------------------------

.. _class_Performance_method_get_monitor:

- :ref:`float<class_float>` **get_monitor** **(** :ref:`Monitor<enum_Performance_Monitor>` monitor **)** |const|

Devuelve el valor de uno de los monitores disponibles. Debe proporcionar una de las constantes :ref:`Monitor<enum_Performance_Monitor>` como argumento, así:

::

    print(Performance.get_monitor(Performance.TIME_FPS)) # Imprime el FPS a la consola

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
