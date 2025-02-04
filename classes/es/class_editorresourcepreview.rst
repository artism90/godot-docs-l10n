:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the EditorResourcePreview.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_EditorResourcePreview:

EditorResourcePreview
=====================

**Inherits:** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Ayudante para generar vistas previas de recursos o archivos.

Descripción
----------------------

Este objeto se utiliza para generar vistas previas de los recursos de los archivos.

\ **Nota:** Esta clase no debe ser instanciada directamente. En su lugar, accede al singleton usando :ref:`EditorInterface.get_resource_previewer<class_EditorInterface_method_get_resource_previewer>`.

Métodos
--------------

+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`add_preview_generator<class_EditorResourcePreview_method_add_preview_generator>` **(** :ref:`EditorResourcePreviewGenerator<class_EditorResourcePreviewGenerator>` generator **)**                                                                                             |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`check_for_invalidation<class_EditorResourcePreview_method_check_for_invalidation>` **(** :ref:`String<class_String>` path **)**                                                                                                                                                |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`queue_edited_resource_preview<class_EditorResourcePreview_method_queue_edited_resource_preview>` **(** :ref:`Resource<class_Resource>` resource, :ref:`Object<class_Object>` receiver, :ref:`String<class_String>` receiver_func, :ref:`Variant<class_Variant>` userdata **)** |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`queue_resource_preview<class_EditorResourcePreview_method_queue_resource_preview>` **(** :ref:`String<class_String>` path, :ref:`Object<class_Object>` receiver, :ref:`String<class_String>` receiver_func, :ref:`Variant<class_Variant>` userdata **)**                       |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`remove_preview_generator<class_EditorResourcePreview_method_remove_preview_generator>` **(** :ref:`EditorResourcePreviewGenerator<class_EditorResourcePreviewGenerator>` generator **)**                                                                                       |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Señales
--------------

.. _class_EditorResourcePreview_signal_preview_invalidated:

- **preview_invalidated** **(** :ref:`String<class_String>` path **)**

Emitido si se invalida (cambia) una vista previa. ``path`` corresponde a la ruta de la vista previa.

Descripciones de Métodos
------------------------------------------------

.. _class_EditorResourcePreview_method_add_preview_generator:

- void **add_preview_generator** **(** :ref:`EditorResourcePreviewGenerator<class_EditorResourcePreviewGenerator>` generator **)**

Crear un generador de previsualización propio y personalizado.

----

.. _class_EditorResourcePreview_method_check_for_invalidation:

- void **check_for_invalidation** **(** :ref:`String<class_String>` path **)**

Compruebe si el recurso ha cambiado, si es así, se invalidará y se emitirá la señal correspondiente.

----

.. _class_EditorResourcePreview_method_queue_edited_resource_preview:

- void **queue_edited_resource_preview** **(** :ref:`Resource<class_Resource>` resource, :ref:`Object<class_Object>` receiver, :ref:`String<class_String>` receiver_func, :ref:`Variant<class_Variant>` userdata **)**

Queue the ``resource`` being edited for preview. Once the preview is ready, the ``receiver``'s ``receiver_func`` will be called. The ``receiver_func`` must take the following four arguments: :ref:`String<class_String>` path, :ref:`Texture<class_Texture>` preview, :ref:`Texture<class_Texture>` thumbnail_preview, :ref:`Variant<class_Variant>` userdata. ``userdata`` can be anything, and will be returned when ``receiver_func`` is called.

\ **Note:** If it was not possible to create the preview the ``receiver_func`` will still be called, but the preview will be null.

----

.. _class_EditorResourcePreview_method_queue_resource_preview:

- void **queue_resource_preview** **(** :ref:`String<class_String>` path, :ref:`Object<class_Object>` receiver, :ref:`String<class_String>` receiver_func, :ref:`Variant<class_Variant>` userdata **)**

Queue a resource file located at ``path`` for preview. Once the preview is ready, the ``receiver``'s ``receiver_func`` will be called. The ``receiver_func`` must take the following four arguments: :ref:`String<class_String>` path, :ref:`Texture<class_Texture>` preview, :ref:`Texture<class_Texture>` thumbnail_preview, :ref:`Variant<class_Variant>` userdata. ``userdata`` can be anything, and will be returned when ``receiver_func`` is called.

\ **Note:** If it was not possible to create the preview the ``receiver_func`` will still be called, but the preview will be null.

----

.. _class_EditorResourcePreview_method_remove_preview_generator:

- void **remove_preview_generator** **(** :ref:`EditorResourcePreviewGenerator<class_EditorResourcePreviewGenerator>` generator **)**

Elimina un generador de previsualización personalizado.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
