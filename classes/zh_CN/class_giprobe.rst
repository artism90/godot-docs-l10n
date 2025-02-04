:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the GIProbe.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_GIProbe:

GIProbe
=======

**Inherits:** :ref:`VisualInstance<class_VisualInstance>` **<** :ref:`CullInstance<class_CullInstance>` **<** :ref:`Spatial<class_Spatial>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

实时全局光照（GI）探测。

描述
----

``GIProbe`` 可以为场景提供高质量的实时间接光照。它们预先计算发光物体和静态几何体的效果，以实时模拟复杂光线的行为。\ ``GIProbe`` 在使用前需要进行烘焙，而后，一旦烘焙，动态物体就会从它们那里接收光线。此外，灯光可以是完全动态的，也可以是烘焙的。

在场景中使用 ``GIProbe`` 会很消耗资源，可以在 :ref:`ProjectSettings<class_ProjectSettings>` 中使用 :ref:`ProjectSettings.rendering/quality/voxel_cone_tracing/high_quality<class_ProjectSettings_property_rendering/quality/voxel_cone_tracing/high_quality>` 来降低探针的质量，换取更好的性能。

\ **程序式生成：**\ ``GIProbe`` 在导出后的项目中也可以进行烘焙，因此它适合程序式生成或者用户构建的关卡，只需保证所有几何体都是预先生成的即可。

\ **性能：**\ ``GIProbe`` 相对更耗 GPU，不适合在集成显卡等低端硬件上使用，可考虑换用 :ref:`BakedLightmap<class_BakedLightmap>`\ 。要为低端硬件提供备选方案，可考虑在你项目的选项菜单中添加禁用 ``GIProbe`` 的选项。隐藏 ``GIProbe`` 节点即可将其禁用。

\ **注意：**\ 网格应该有足够厚的墙以避免漏光，注，避免单面墙。对于内部关卡，将你的关卡几何体包围在一个足够大的盒子里，并将环路联接起来以关闭网格。

\ **注意：**\ 由于渲染器的限制，在\ ``GIProbe``\ 中使用发光的\ :ref:`ShaderMaterial<class_ShaderMaterial>`\ 时不能发光。只有发射型的\ :ref:`SpatialMaterial<class_SpatialMaterial>`\ 可以在\ ``GIProbe``\ 中发射光线。

教程
----

- :doc:`GI probes <../tutorials/3d/gi_probes>`

- `Third Person Shooter Demo <https://godotengine.org/asset-library/asset/678>`__

属性
----

+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`float<class_float>`             | :ref:`bias<class_GIProbe_property_bias>`                   | ``1.5``                   |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`bool<class_bool>`               | :ref:`compress<class_GIProbe_property_compress>`           | ``false``                 |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`GIProbeData<class_GIProbeData>` | :ref:`data<class_GIProbe_property_data>`                   |                           |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`int<class_int>`                 | :ref:`dynamic_range<class_GIProbe_property_dynamic_range>` | ``4``                     |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`float<class_float>`             | :ref:`energy<class_GIProbe_property_energy>`               | ``1.0``                   |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`Vector3<class_Vector3>`         | :ref:`extents<class_GIProbe_property_extents>`             | ``Vector3( 10, 10, 10 )`` |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`bool<class_bool>`               | :ref:`interior<class_GIProbe_property_interior>`           | ``false``                 |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`float<class_float>`             | :ref:`normal_bias<class_GIProbe_property_normal_bias>`     | ``0.0``                   |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`float<class_float>`             | :ref:`propagation<class_GIProbe_property_propagation>`     | ``0.7``                   |
+---------------------------------------+------------------------------------------------------------+---------------------------+
| :ref:`Subdiv<enum_GIProbe_Subdiv>`    | :ref:`subdiv<class_GIProbe_property_subdiv>`               | ``1``                     |
+---------------------------------------+------------------------------------------------------------+---------------------------+

方法
----

+------+----------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`bake<class_GIProbe_method_bake>` **(** :ref:`Node<class_Node>` from_node=null, :ref:`bool<class_bool>` create_visual_debug=false **)** |
+------+----------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`debug_bake<class_GIProbe_method_debug_bake>` **(** **)**                                                                               |
+------+----------------------------------------------------------------------------------------------------------------------------------------------+

枚举
----

.. _enum_GIProbe_Subdiv:

.. _class_GIProbe_constant_SUBDIV_64:

.. _class_GIProbe_constant_SUBDIV_128:

.. _class_GIProbe_constant_SUBDIV_256:

.. _class_GIProbe_constant_SUBDIV_512:

.. _class_GIProbe_constant_SUBDIV_MAX:

enum **Subdiv**:

- **SUBDIV_64** = **0** --- 使用64分区，这是最低的质量设置，但也是最快的。如果你能使用它，特别是在低端硬件上使用它。

- **SUBDIV_128** = **1** --- 使用128个分区。这是默认的质量设置。

- **SUBDIV_256** = **2** --- 使用256个分区。

- **SUBDIV_512** = **3** --- 使用 512 个分区。这是最高的质量设置，但也是最慢的。在低端硬件上，这可能会导致 GPU 停顿。

- **SUBDIV_MAX** = **4** --- 代表 :ref:`Subdiv<enum_GIProbe_Subdiv>` 举的大小。

属性说明
--------

.. _class_GIProbe_property_bias:

- :ref:`float<class_float>` **bias**

+-----------+-----------------+
| *Default* | ``1.5``         |
+-----------+-----------------+
| *Setter*  | set_bias(value) |
+-----------+-----------------+
| *Getter*  | get_bias()      |
+-----------+-----------------+

从 ``GIProbe`` 偏移光贡献的查找。这可用于避免自阴影，但可能会在较高的值下引入漏光。这个和 :ref:`normal_bias<class_GIProbe_property_normal_bias>` 应该使用，以尽量减少自阴影和漏光。

\ **注意：** ``bias`` 通常应该在 1.0 以上，因为这是体素的大小。

----

.. _class_GIProbe_property_compress:

- :ref:`bool<class_bool>` **compress**

+-----------+---------------------+
| *Default* | ``false``           |
+-----------+---------------------+
| *Setter*  | set_compress(value) |
+-----------+---------------------+
| *Getter*  | is_compressed()     |
+-----------+---------------------+

*已废弃*\ 由于已知的错误，这个属性已被废弃，启用后不再有任何效果。

----

.. _class_GIProbe_property_data:

- :ref:`GIProbeData<class_GIProbeData>` **data**

+----------+-----------------------+
| *Setter* | set_probe_data(value) |
+----------+-----------------------+
| *Getter* | get_probe_data()      |
+----------+-----------------------+

持有此 ``GIProbe`` 的数据的 :ref:`GIProbeData<class_GIProbeData>` 资源。

----

.. _class_GIProbe_property_dynamic_range:

- :ref:`int<class_int>` **dynamic_range**

+-----------+--------------------------+
| *Default* | ``4``                    |
+-----------+--------------------------+
| *Setter*  | set_dynamic_range(value) |
+-----------+--------------------------+
| *Getter*  | get_dynamic_range()      |
+-----------+--------------------------+

``GIProbe`` 能识别的最大亮度。亮度将在此范围内缩放。

----

.. _class_GIProbe_property_energy:

- :ref:`float<class_float>` **energy**

+-----------+-------------------+
| *Default* | ``1.0``           |
+-----------+-------------------+
| *Setter*  | set_energy(value) |
+-----------+-------------------+
| *Getter*  | get_energy()      |
+-----------+-------------------+

能量倍数。使 ``GIProbe`` 的照明贡献更亮。

----

.. _class_GIProbe_property_extents:

- :ref:`Vector3<class_Vector3>` **extents**

+-----------+---------------------------+
| *Default* | ``Vector3( 10, 10, 10 )`` |
+-----------+---------------------------+
| *Setter*  | set_extents(value)        |
+-----------+---------------------------+
| *Getter*  | get_extents()             |
+-----------+---------------------------+

``GIProbe`` 所覆盖区域的大小。如果你让外延变大，而没有用 :ref:`subdiv<class_GIProbe_property_subdiv>` 增加细分，每个单元的大小将增加，并导致低细节照明。

----

.. _class_GIProbe_property_interior:

- :ref:`bool<class_bool>` **interior**

+-----------+---------------------+
| *Default* | ``false``           |
+-----------+---------------------+
| *Setter*  | set_interior(value) |
+-----------+---------------------+
| *Getter*  | is_interior()       |
+-----------+---------------------+

如果为\ ``true``\ ，在计算照明时忽略天空的贡献。

----

.. _class_GIProbe_property_normal_bias:

- :ref:`float<class_float>` **normal_bias**

+-----------+------------------------+
| *Default* | ``0.0``                |
+-----------+------------------------+
| *Setter*  | set_normal_bias(value) |
+-----------+------------------------+
| *Getter*  | get_normal_bias()      |
+-----------+------------------------+

根据物体的法线方向，对 ``GIProbe`` 的查找进行偏移。可以用来减少一些自阴影的假象。

----

.. _class_GIProbe_property_propagation:

- :ref:`float<class_float>` **propagation**

+-----------+------------------------+
| *Default* | ``0.7``                |
+-----------+------------------------+
| *Setter*  | set_propagation(value) |
+-----------+------------------------+
| *Getter*  | get_propagation()      |
+-----------+------------------------+

光在探针内部传播的程度。一个较高的值可以使光传播得更远。

----

.. _class_GIProbe_property_subdiv:

- :ref:`Subdiv<enum_GIProbe_Subdiv>` **subdiv**

+-----------+-------------------+
| *Default* | ``1``             |
+-----------+-------------------+
| *Setter*  | set_subdiv(value) |
+-----------+-------------------+
| *Getter*  | get_subdiv()      |
+-----------+-------------------+

对 ``GIProbe`` 所操作的网格进行细分的次数。数字越大，细节就越精细，因而视觉质量就越高，而数字越小，性能就越好。

方法说明
--------

.. _class_GIProbe_method_bake:

- void **bake** **(** :ref:`Node<class_Node>` from_node=null, :ref:`bool<class_bool>` create_visual_debug=false **)**

烘焙所有标有 :ref:`GeometryInstance.use_in_baked_light<class_GeometryInstance_property_use_in_baked_light>` 的 :ref:`GeometryInstance<class_GeometryInstance>` 和标有 :ref:`Light.BAKE_INDIRECT<class_Light_constant_BAKE_INDIRECT>` 或 :ref:`Light.BAKE_ALL<class_Light_constant_BAKE_ALL>` 的 :ref:`Light<class_Light>` 的效果。如果\ ``create_visual_debug``\ 是\ ``true``\ ，在烘焙光线后，这将生成一个\ :ref:`MultiMesh<class_MultiMesh>`\ ，其中有一个立方体代表每个实体单元，每个立方体的颜色与该单元的反照率颜色一致。这可以用来可视化 ``GIProbe`` 的数据，以调试任何可能发生的问题。

\ **注意：** :ref:`bake<class_GIProbe_method_bake>` 在编辑器和导出后的项目中都是有效的。因此适用于程序化生成或者用户构建的关卡。在多数场景中，烘焙 ``GIProbe`` 通常需要花费 5 到 20 秒。减少 :ref:`subdiv<class_GIProbe_property_subdiv>` 可以加速烘焙。

----

.. _class_GIProbe_method_debug_bake:

- void **debug_bake** **(** **)**

在启用 ``create_visual_debug`` 的情况下调用 :ref:`bake<class_GIProbe_method_bake>` 。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
