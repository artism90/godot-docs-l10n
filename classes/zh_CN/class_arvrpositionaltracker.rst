:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ARVRPositionalTracker.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ARVRPositionalTracker:

ARVRPositionalTracker
=====================

**Inherits:** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

跟踪对象。

描述
----

此对象的实例表示被跟踪的设备，例如控制器或锚点。由于 HMD 是在内部处理的，因此不表示 HMD。

当控制器打开并且 AR/VR 界面检测到它们时，此对象的实例会自动添加到可通过 :ref:`ARVRServer<class_ARVRServer>` 访问的活动的跟踪对象列表中。

\ :ref:`ARVRController<class_ARVRController>` 和 :ref:`ARVRAnchor<class_ARVRAnchor>` 都使用这种类型的对象，你应该在的项目中使用。位置跟踪器只是使这一切正常工作的底层对象。这些大部分都是公开的，以便基于 GDNative 的接口可以与它们交互。

教程
----

- :doc:`../tutorials/vr/index`

属性
----

+---------------------------+------------------------------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`rumble<class_ARVRPositionalTracker_property_rumble>` | ``0.0`` |
+---------------------------+------------------------------------------------------------+---------+

方法
----

+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TrackerHand<enum_ARVRPositionalTracker_TrackerHand>` | :ref:`get_hand<class_ARVRPositionalTracker_method_get_hand>` **(** **)** |const|                                                             |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                                      | :ref:`get_joy_id<class_ARVRPositionalTracker_method_get_joy_id>` **(** **)** |const|                                                         |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Mesh<class_Mesh>`                                    | :ref:`get_mesh<class_ARVRPositionalTracker_method_get_mesh>` **(** **)** |const|                                                             |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                                | :ref:`get_name<class_ARVRPositionalTracker_method_get_name>` **(** **)** |const|                                                             |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Basis<class_Basis>`                                  | :ref:`get_orientation<class_ARVRPositionalTracker_method_get_orientation>` **(** **)** |const|                                               |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>`                              | :ref:`get_position<class_ARVRPositionalTracker_method_get_position>` **(** **)** |const|                                                     |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                                      | :ref:`get_tracker_id<class_ARVRPositionalTracker_method_get_tracker_id>` **(** **)** |const|                                                 |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                    | :ref:`get_tracks_orientation<class_ARVRPositionalTracker_method_get_tracks_orientation>` **(** **)** |const|                                 |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                    | :ref:`get_tracks_position<class_ARVRPositionalTracker_method_get_tracks_position>` **(** **)** |const|                                       |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Transform<class_Transform>`                          | :ref:`get_transform<class_ARVRPositionalTracker_method_get_transform>` **(** :ref:`bool<class_bool>` adjust_by_reference_frame **)** |const| |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TrackerType<enum_ARVRServer_TrackerType>`            | :ref:`get_type<class_ARVRPositionalTracker_method_get_type>` **(** **)** |const|                                                             |
+------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------+

枚举
----

.. _enum_ARVRPositionalTracker_TrackerHand:

.. _class_ARVRPositionalTracker_constant_TRACKER_HAND_UNKNOWN:

.. _class_ARVRPositionalTracker_constant_TRACKER_LEFT_HAND:

.. _class_ARVRPositionalTracker_constant_TRACKER_RIGHT_HAND:

enum **TrackerHand**:

- **TRACKER_HAND_UNKNOWN** = **0** --- 这个追踪器所持的手是未知的或不适用的。

- **TRACKER_LEFT_HAND** = **1** --- 此跟踪器是左手控制器。

- **TRACKER_RIGHT_HAND** = **2** --- 此跟踪器是右手控制器。

属性说明
--------

.. _class_ARVRPositionalTracker_property_rumble:

- :ref:`float<class_float>` **rumble**

+-----------+-------------------+
| *Default* | ``0.0``           |
+-----------+-------------------+
| *Setter*  | set_rumble(value) |
+-----------+-------------------+
| *Getter*  | get_rumble()      |
+-----------+-------------------+

追踪器噪声的程度。范围从\ ``0.0``\ 到\ ``1.0``\ ，精度\ ``.01``\ 。

方法说明
--------

.. _class_ARVRPositionalTracker_method_get_hand:

- :ref:`TrackerHand<enum_ARVRPositionalTracker_TrackerHand>` **get_hand** **(** **)** |const|

返回持有此追踪器的手，如果知道。参阅\ :ref:`TrackerHand<enum_ARVRPositionalTracker_TrackerHand>`\ 常量。

----

.. _class_ARVRPositionalTracker_method_get_joy_id:

- :ref:`int<class_int>` **get_joy_id** **(** **)** |const|

如果这是一个正在被追踪的控制器，该控制器将由一个具有此ID的操纵杆条目表示。

----

.. _class_ARVRPositionalTracker_method_get_mesh:

- :ref:`Mesh<class_Mesh>` **get_mesh** **(** **)** |const|

如果可用，则返回与控制器或锚点相关的网格。

----

.. _class_ARVRPositionalTracker_method_get_name:

- :ref:`String<class_String>` **get_name** **(** **)** |const|

如果可用，返回控制器或锚点的名称。

----

.. _class_ARVRPositionalTracker_method_get_orientation:

- :ref:`Basis<class_Basis>` **get_orientation** **(** **)** |const|

返回控制器的方向矩阵。

----

.. _class_ARVRPositionalTracker_method_get_position:

- :ref:`Vector3<class_Vector3>` **get_position** **(** **)** |const|

返回世界空间控制器的位置。

----

.. _class_ARVRPositionalTracker_method_get_tracker_id:

- :ref:`int<class_int>` **get_tracker_id** **(** **)** |const|

返回内部跟踪器的ID。这是对每个跟踪器类型的唯一标识，与你需要为\ :ref:`ARVRController<class_ARVRController>`\ 和\ :ref:`ARVRAnchor<class_ARVRAnchor>`\ 节点指定的ID相匹配。

----

.. _class_ARVRPositionalTracker_method_get_tracks_orientation:

- :ref:`bool<class_bool>` **get_tracks_orientation** **(** **)** |const|

如果该设备跟踪方向，则返回\ ``true``\ 。

----

.. _class_ARVRPositionalTracker_method_get_tracks_position:

- :ref:`bool<class_bool>` **get_tracks_position** **(** **)** |const|

如果该设备跟踪位置，则返回\ ``true``\ 。

----

.. _class_ARVRPositionalTracker_method_get_transform:

- :ref:`Transform<class_Transform>` **get_transform** **(** :ref:`bool<class_bool>` adjust_by_reference_frame **)** |const|

返回组合此设备的方向和坐标的变换。

----

.. _class_ARVRPositionalTracker_method_get_type:

- :ref:`TrackerType<enum_ARVRServer_TrackerType>` **get_type** **(** **)** |const|

返回跟踪器的类型。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
