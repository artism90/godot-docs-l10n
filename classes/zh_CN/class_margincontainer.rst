:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the MarginContainer.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_MarginContainer:

MarginContainer
===============

**Inherits:** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

简单边距容器。

描述
----

为所有作为容器的直接子节点的\ :ref:`Control<class_Control>`\ 节点添加顶部、左侧、底部和右侧的边距。要控制\ ``MarginContainer``\ 的边距，请使用下面列出的\ ``margin_*`` 主题属性。

\ **注意：**\ 要小心，\ :ref:`Control<class_Control>`\ 的margin值与常量margin值不同。如果你想通过代码改变\ ``MarginContainer``\ 的自定义边距值，应该使用下面的例子:

::

    # 这个代码示例假定当前脚本扩展自MarginContainer。
    var margin_value = 100
    add_constant_override("margin_top", margin_value)
    add_constant_override("margin_left", margin_value)
    add_constant_override("margin_bottom", margin_value)
    add_constant_override("margin_right", margin_value)

主题属性
--------

+-----------------------+--------------------------------------------------------------------------+-------+
| :ref:`int<class_int>` | :ref:`margin_bottom<class_MarginContainer_theme_constant_margin_bottom>` | ``0`` |
+-----------------------+--------------------------------------------------------------------------+-------+
| :ref:`int<class_int>` | :ref:`margin_left<class_MarginContainer_theme_constant_margin_left>`     | ``0`` |
+-----------------------+--------------------------------------------------------------------------+-------+
| :ref:`int<class_int>` | :ref:`margin_right<class_MarginContainer_theme_constant_margin_right>`   | ``0`` |
+-----------------------+--------------------------------------------------------------------------+-------+
| :ref:`int<class_int>` | :ref:`margin_top<class_MarginContainer_theme_constant_margin_top>`       | ``0`` |
+-----------------------+--------------------------------------------------------------------------+-------+

Theme Property Descriptions
---------------------------

.. _class_MarginContainer_theme_constant_margin_bottom:

- :ref:`int<class_int>` **margin_bottom**

+-----------+-------+
| *Default* | ``0`` |
+-----------+-------+

所有\ ``MarginContainer``\ 的直接子代将有\ ``margin_bottom``\ 像素的底边距。

----

.. _class_MarginContainer_theme_constant_margin_left:

- :ref:`int<class_int>` **margin_left**

+-----------+-------+
| *Default* | ``0`` |
+-----------+-------+

所有\ ``MarginContainer``\ 的直接子代将有\ ``margin_left``\ 像素的左边距。

----

.. _class_MarginContainer_theme_constant_margin_right:

- :ref:`int<class_int>` **margin_right**

+-----------+-------+
| *Default* | ``0`` |
+-----------+-------+

所有\ ``MarginContainer``\ 的直接子代将有\ ``margin_right``\ 像素的右边距。

----

.. _class_MarginContainer_theme_constant_margin_top:

- :ref:`int<class_int>` **margin_top**

+-----------+-------+
| *Default* | ``0`` |
+-----------+-------+

所有\ ``MarginContainer``\ 的直接子代将有\ ``margin_right``\ 像素的顶边距。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
