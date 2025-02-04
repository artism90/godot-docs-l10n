:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the CanvasItemMaterial.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_CanvasItemMaterial:

CanvasItemMaterial
==================

**Inherits:** :ref:`Material<class_Material>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

:ref:`CanvasItem<class_CanvasItem>`\ 的材质。

描述
----

``CanvasItemMaterial``\ 提供了一种修改与CanvasItem相关联的纹理的方法。他们专注于描述纹理的混合和照明行为。使用\ :ref:`ShaderMaterial<class_ShaderMaterial>`\ 可以更全面地自定义材质与\ :ref:`CanvasItem<class_CanvasItem>`\ 的交互。

属性
----

+-----------------------------------------------------+-------------------------------------------------------------------------------------------+-----------+
| :ref:`BlendMode<enum_CanvasItemMaterial_BlendMode>` | :ref:`blend_mode<class_CanvasItemMaterial_property_blend_mode>`                           | ``0``     |
+-----------------------------------------------------+-------------------------------------------------------------------------------------------+-----------+
| :ref:`LightMode<enum_CanvasItemMaterial_LightMode>` | :ref:`light_mode<class_CanvasItemMaterial_property_light_mode>`                           | ``0``     |
+-----------------------------------------------------+-------------------------------------------------------------------------------------------+-----------+
| :ref:`int<class_int>`                               | :ref:`particles_anim_h_frames<class_CanvasItemMaterial_property_particles_anim_h_frames>` |           |
+-----------------------------------------------------+-------------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                             | :ref:`particles_anim_loop<class_CanvasItemMaterial_property_particles_anim_loop>`         |           |
+-----------------------------------------------------+-------------------------------------------------------------------------------------------+-----------+
| :ref:`int<class_int>`                               | :ref:`particles_anim_v_frames<class_CanvasItemMaterial_property_particles_anim_v_frames>` |           |
+-----------------------------------------------------+-------------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                             | :ref:`particles_animation<class_CanvasItemMaterial_property_particles_animation>`         | ``false`` |
+-----------------------------------------------------+-------------------------------------------------------------------------------------------+-----------+

枚举
----

.. _enum_CanvasItemMaterial_BlendMode:

.. _class_CanvasItemMaterial_constant_BLEND_MODE_MIX:

.. _class_CanvasItemMaterial_constant_BLEND_MODE_ADD:

.. _class_CanvasItemMaterial_constant_BLEND_MODE_SUB:

.. _class_CanvasItemMaterial_constant_BLEND_MODE_MUL:

.. _class_CanvasItemMaterial_constant_BLEND_MODE_PREMULT_ALPHA:

enum **BlendMode**:

- **BLEND_MODE_MIX** = **0** --- 混合混合模式。假设颜色与alpha（不透明度）值无关。

- **BLEND_MODE_ADD** = **1** --- 加法混合模式。

- **BLEND_MODE_SUB** = **2** --- 减法混合模式。

- **BLEND_MODE_MUL** = **3** --- 乘法混合模式。

- **BLEND_MODE_PREMULT_ALPHA** = **4** --- 混合混合模式。假定颜色已预先乘以alpha（不透明度）值。

----

.. _enum_CanvasItemMaterial_LightMode:

.. _class_CanvasItemMaterial_constant_LIGHT_MODE_NORMAL:

.. _class_CanvasItemMaterial_constant_LIGHT_MODE_UNSHADED:

.. _class_CanvasItemMaterial_constant_LIGHT_MODE_LIGHT_ONLY:

enum **LightMode**:

- **LIGHT_MODE_NORMAL** = **0** --- 使用光敏和非光敏材料属性渲染材质。

- **LIGHT_MODE_UNSHADED** = **1** --- 将材质渲染成没有光的样子。

- **LIGHT_MODE_LIGHT_ONLY** = **2** --- 将材质渲染成只有光的样子。

属性说明
--------

.. _class_CanvasItemMaterial_property_blend_mode:

- :ref:`BlendMode<enum_CanvasItemMaterial_BlendMode>` **blend_mode**

+-----------+-----------------------+
| *Default* | ``0``                 |
+-----------+-----------------------+
| *Setter*  | set_blend_mode(value) |
+-----------+-----------------------+
| *Getter*  | get_blend_mode()      |
+-----------+-----------------------+

将材质的渲染应用于基础纹理的方式。

----

.. _class_CanvasItemMaterial_property_light_mode:

- :ref:`LightMode<enum_CanvasItemMaterial_LightMode>` **light_mode**

+-----------+-----------------------+
| *Default* | ``0``                 |
+-----------+-----------------------+
| *Setter*  | set_light_mode(value) |
+-----------+-----------------------+
| *Getter*  | get_light_mode()      |
+-----------+-----------------------+

材质对照明的反应方式。

----

.. _class_CanvasItemMaterial_property_particles_anim_h_frames:

- :ref:`int<class_int>` **particles_anim_h_frames**

+----------+------------------------------------+
| *Setter* | set_particles_anim_h_frames(value) |
+----------+------------------------------------+
| *Getter* | get_particles_anim_h_frames()      |
+----------+------------------------------------+

精灵表中分配为 :ref:`Particles2D<class_Particles2D>` 或 :ref:`CPUParticles2D<class_CPUParticles2D>` 的 :ref:`Texture<class_Texture>` 的列数。

\ **注意：**\ 仅当 :ref:`particles_animation<class_CanvasItemMaterial_property_particles_animation>` 为 ``true`` 时，此属性才在编辑器中使用和可见。

----

.. _class_CanvasItemMaterial_property_particles_anim_loop:

- :ref:`bool<class_bool>` **particles_anim_loop**

+----------+--------------------------------+
| *Setter* | set_particles_anim_loop(value) |
+----------+--------------------------------+
| *Getter* | get_particles_anim_loop()      |
+----------+--------------------------------+

如果\ ``true``\ ，粒子动画将循环播放。

\ **注意:**\ 只有当\ :ref:`particles_animation<class_CanvasItemMaterial_property_particles_animation>`\ 为\ ``true``\ 时，该属性才会在编辑器中使用并可见。

----

.. _class_CanvasItemMaterial_property_particles_anim_v_frames:

- :ref:`int<class_int>` **particles_anim_v_frames**

+----------+------------------------------------+
| *Setter* | set_particles_anim_v_frames(value) |
+----------+------------------------------------+
| *Getter* | get_particles_anim_v_frames()      |
+----------+------------------------------------+

精灵表中分配为 :ref:`Particles2D<class_Particles2D>` 或 :ref:`CPUParticles2D<class_CPUParticles2D>` 的 :ref:`Texture<class_Texture>` 的行数。

\ **注意：**\ 仅当 :ref:`particles_animation<class_CanvasItemMaterial_property_particles_animation>` 为 ``true`` 时，此属性才在编辑器中使用和可见。

----

.. _class_CanvasItemMaterial_property_particles_animation:

- :ref:`bool<class_bool>` **particles_animation**

+-----------+--------------------------------+
| *Default* | ``false``                      |
+-----------+--------------------------------+
| *Setter*  | set_particles_animation(value) |
+-----------+--------------------------------+
| *Getter*  | get_particles_animation()      |
+-----------+--------------------------------+

如果为\ ``true``\ ，当分配给 :ref:`Particles2D<class_Particles2D>` 和 :ref:`CPUParticles2D<class_CPUParticles2D>` 节点时，启用基于spritesheet的动画功能。\ :ref:`ParticlesMaterial.anim_speed<class_ParticlesMaterial_property_anim_speed>`\ 或\ :ref:`CPUParticles2D.anim_speed<class_CPUParticles2D_property_anim_speed>`\ 也应设置为正值，才能播放动画。

这个属性（以及其他依赖于它的\ ``particles_anim_*``\ 属性）对其他类型的节点没有影响。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
