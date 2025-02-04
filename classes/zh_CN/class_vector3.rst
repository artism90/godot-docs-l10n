:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Vector3.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Vector3:

Vector3
=======

用于 3D 数学的向量。

描述
----

可用于表示 3D 空间中的位置或任何其他数值对的 3 元素结构。

\ **注意：** 在布尔上下文中，如果 Vector3 等于 ``Vector3(0, 0, 0)``\ ，将评估为 ``false``\ 。否则， Vector3 将始终评估为 ``true``\ 。

教程
----

- :doc:`Math tutorial index <../tutorials/math/index>`

- :doc:`Vector math <../tutorials/math/vector_math>`

- :doc:`Advanced vector math <../tutorials/math/vectors_advanced>`

- `3Blue1Brown Essence of Linear Algebra <https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab>`__

- `Matrix Transform Demo <https://godotengine.org/asset-library/asset/584>`__

- `All 3D Demos <https://github.com/godotengine/godot-demo-projects/tree/master/3d>`__

属性
----

+---------------------------+------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`x<class_Vector3_property_x>` | ``0.0`` |
+---------------------------+------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`y<class_Vector3_property_y>` | ``0.0`` |
+---------------------------+------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`z<class_Vector3_property_z>` | ``0.0`` |
+---------------------------+------------------------------------+---------+

方法
----

+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`Vector3<class_Vector3_method_Vector3>` **(** :ref:`float<class_float>` x, :ref:`float<class_float>` y, :ref:`float<class_float>` z **)**                                                                            |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`abs<class_Vector3_method_abs>` **(** **)**                                                                                                                                                                          |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`angle_to<class_Vector3_method_angle_to>` **(** :ref:`Vector3<class_Vector3>` to **)**                                                                                                                               |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`bounce<class_Vector3_method_bounce>` **(** :ref:`Vector3<class_Vector3>` n **)**                                                                                                                                    |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`ceil<class_Vector3_method_ceil>` **(** **)**                                                                                                                                                                        |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`cross<class_Vector3_method_cross>` **(** :ref:`Vector3<class_Vector3>` b **)**                                                                                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`cubic_interpolate<class_Vector3_method_cubic_interpolate>` **(** :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` pre_a, :ref:`Vector3<class_Vector3>` post_b, :ref:`float<class_float>` weight **)** |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`direction_to<class_Vector3_method_direction_to>` **(** :ref:`Vector3<class_Vector3>` b **)**                                                                                                                        |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`distance_squared_to<class_Vector3_method_distance_squared_to>` **(** :ref:`Vector3<class_Vector3>` b **)**                                                                                                          |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`distance_to<class_Vector3_method_distance_to>` **(** :ref:`Vector3<class_Vector3>` b **)**                                                                                                                          |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`dot<class_Vector3_method_dot>` **(** :ref:`Vector3<class_Vector3>` b **)**                                                                                                                                          |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`floor<class_Vector3_method_floor>` **(** **)**                                                                                                                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`inverse<class_Vector3_method_inverse>` **(** **)**                                                                                                                                                                  |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`is_equal_approx<class_Vector3_method_is_equal_approx>` **(** :ref:`Vector3<class_Vector3>` v **)**                                                                                                                  |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`is_normalized<class_Vector3_method_is_normalized>` **(** **)**                                                                                                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`length<class_Vector3_method_length>` **(** **)**                                                                                                                                                                    |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`length_squared<class_Vector3_method_length_squared>` **(** **)**                                                                                                                                                    |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`limit_length<class_Vector3_method_limit_length>` **(** :ref:`float<class_float>` length=1.0 **)**                                                                                                                   |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`linear_interpolate<class_Vector3_method_linear_interpolate>` **(** :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` weight **)**                                                                         |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`max_axis<class_Vector3_method_max_axis>` **(** **)**                                                                                                                                                                |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`min_axis<class_Vector3_method_min_axis>` **(** **)**                                                                                                                                                                |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`move_toward<class_Vector3_method_move_toward>` **(** :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` delta **)**                                                                                        |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`normalized<class_Vector3_method_normalized>` **(** **)**                                                                                                                                                            |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Basis<class_Basis>`     | :ref:`outer<class_Vector3_method_outer>` **(** :ref:`Vector3<class_Vector3>` b **)**                                                                                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`posmod<class_Vector3_method_posmod>` **(** :ref:`float<class_float>` mod **)**                                                                                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`posmodv<class_Vector3_method_posmodv>` **(** :ref:`Vector3<class_Vector3>` modv **)**                                                                                                                               |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`project<class_Vector3_method_project>` **(** :ref:`Vector3<class_Vector3>` b **)**                                                                                                                                  |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`reflect<class_Vector3_method_reflect>` **(** :ref:`Vector3<class_Vector3>` n **)**                                                                                                                                  |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`rotated<class_Vector3_method_rotated>` **(** :ref:`Vector3<class_Vector3>` axis, :ref:`float<class_float>` phi **)**                                                                                                |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`round<class_Vector3_method_round>` **(** **)**                                                                                                                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`sign<class_Vector3_method_sign>` **(** **)**                                                                                                                                                                        |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`signed_angle_to<class_Vector3_method_signed_angle_to>` **(** :ref:`Vector3<class_Vector3>` to, :ref:`Vector3<class_Vector3>` axis **)**                                                                             |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`slerp<class_Vector3_method_slerp>` **(** :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` weight **)**                                                                                                   |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`slide<class_Vector3_method_slide>` **(** :ref:`Vector3<class_Vector3>` n **)**                                                                                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`snapped<class_Vector3_method_snapped>` **(** :ref:`Vector3<class_Vector3>` by **)**                                                                                                                                 |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Basis<class_Basis>`     | :ref:`to_diagonal_matrix<class_Vector3_method_to_diagonal_matrix>` **(** **)**                                                                                                                                            |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

常量
----

.. _class_Vector3_constant_AXIS_X:

.. _class_Vector3_constant_AXIS_Y:

.. _class_Vector3_constant_AXIS_Z:

.. _class_Vector3_constant_ZERO:

.. _class_Vector3_constant_ONE:

.. _class_Vector3_constant_INF:

.. _class_Vector3_constant_LEFT:

.. _class_Vector3_constant_RIGHT:

.. _class_Vector3_constant_UP:

.. _class_Vector3_constant_DOWN:

.. _class_Vector3_constant_FORWARD:

.. _class_Vector3_constant_BACK:

- **AXIS_X** = **0** --- X 轴的枚举值。由 :ref:`max_axis<class_Vector3_method_max_axis>` 和 :ref:`min_axis<class_Vector3_method_min_axis>` 返回。

- **AXIS_Y** = **1** --- Y 轴的枚举值。由 :ref:`max_axis<class_Vector3_method_max_axis>` 和 :ref:`min_axis<class_Vector3_method_min_axis>` 返回。

- **AXIS_Z** = **2** --- Z 轴的枚举值。由 :ref:`max_axis<class_Vector3_method_max_axis>` 和 :ref:`min_axis<class_Vector3_method_min_axis>` 返回。

- **ZERO** = **Vector3( 0, 0, 0 )** --- 零向量，所有分量都设置为 ``0`` 的向量。

- **ONE** = **Vector3( 1, 1, 1 )** --- 一向量，所有分量都设置为 ``1`` 的向量。

- **INF** = **Vector3( inf, inf, inf )** --- 无穷大向量，所有分量都设置为 :ref:`@GDScript.INF<class_@GDScript_constant_INF>` 的向量。

- **LEFT** = **Vector3( -1, 0, 0 )** --- 左单位向量。代表局部的左方向，全局的西方向。

- **RIGHT** = **Vector3( 1, 0, 0 )** --- 右单位向量。代表局部的右方向，全局的东方向。

- **UP** = **Vector3( 0, 1, 0 )** --- 上单位向量。

- **DOWN** = **Vector3( 0, -1, 0 )** --- 下单位向量。

- **FORWARD** = **Vector3( 0, 0, -1 )** --- 前单位向量。代表局部的前方向，全局的北方向。

- **BACK** = **Vector3( 0, 0, 1 )** --- 后单位向量。代表局部的后方向，全局的南方向。

属性说明
--------

.. _class_Vector3_property_x:

- :ref:`float<class_float>` **x**

+-----------+---------+
| *Default* | ``0.0`` |
+-----------+---------+

向量的 X 分量。也可以通过使用索引位置 ``[0]`` 访问。

----

.. _class_Vector3_property_y:

- :ref:`float<class_float>` **y**

+-----------+---------+
| *Default* | ``0.0`` |
+-----------+---------+

向量的 Y 分量。也可以通过使用索引位置 ``[1]`` 访问。

----

.. _class_Vector3_property_z:

- :ref:`float<class_float>` **z**

+-----------+---------+
| *Default* | ``0.0`` |
+-----------+---------+

向量的Z分量。也可以通过使用索引位置\ ``[2]``\ 访问。

方法说明
--------

.. _class_Vector3_method_Vector3:

- :ref:`Vector3<class_Vector3>` **Vector3** **(** :ref:`float<class_float>` x, :ref:`float<class_float>` y, :ref:`float<class_float>` z **)**

返回具有给定分量的Vector3。

----

.. _class_Vector3_method_abs:

- :ref:`Vector3<class_Vector3>` **abs** **(** **)**

返回一个新的向量，其所有分量都是绝对值，即正值。

----

.. _class_Vector3_method_angle_to:

- :ref:`float<class_float>` **angle_to** **(** :ref:`Vector3<class_Vector3>` to **)**

返回与给定向量的无符号最小角度，单位为弧度。

----

.. _class_Vector3_method_bounce:

- :ref:`Vector3<class_Vector3>` **bounce** **(** :ref:`Vector3<class_Vector3>` n **)**

返回从由给定法线定义的平面上“反弹”的向量。

----

.. _class_Vector3_method_ceil:

- :ref:`Vector3<class_Vector3>` **ceil** **(** **)**

返回一个新的向量，所有的分量都是四舍五入的，向正无穷大。

----

.. _class_Vector3_method_cross:

- :ref:`Vector3<class_Vector3>` **cross** **(** :ref:`Vector3<class_Vector3>` b **)**

返回此向量与 ``b`` 的叉积。

----

.. _class_Vector3_method_cubic_interpolate:

- :ref:`Vector3<class_Vector3>` **cubic_interpolate** **(** :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` pre_a, :ref:`Vector3<class_Vector3>` post_b, :ref:`float<class_float>` weight **)**

在向量\ ``pre_a``, ``a``, ``b``, ``post_b``\ （\ ``a``\ 是当前的）之间，通过给定的量\ ``weight``\ 进行三次插值。\ ``weight``\ 的范围是0.0到1.0，表示插值的数量。

----

.. _class_Vector3_method_direction_to:

- :ref:`Vector3<class_Vector3>` **direction_to** **(** :ref:`Vector3<class_Vector3>` b **)**

返回从这个向量指向\ ``b``\ 的归一化向量。这相当于使用\ ``(b-a).normalized()``\ 。

----

.. _class_Vector3_method_distance_squared_to:

- :ref:`float<class_float>` **distance_squared_to** **(** :ref:`Vector3<class_Vector3>` b **)**

返回这个向量与\ ``b``\ 之间的平方距离。

这个方法比\ :ref:`distance_to<class_Vector3_method_distance_to>`\ 运行得更快，所以如果你需要比较向量或需要一些公式的平方距离，则更喜欢它。

----

.. _class_Vector3_method_distance_to:

- :ref:`float<class_float>` **distance_to** **(** :ref:`Vector3<class_Vector3>` b **)**

返回此向量与\ ``b``\ 之间的距离。

----

.. _class_Vector3_method_dot:

- :ref:`float<class_float>` **dot** **(** :ref:`Vector3<class_Vector3>` b **)**

返回此向量与\ ``b``\ 的点积。这可以用来比较两个向量之间的角度。例如，这可以用来确定一个敌人是否正面对玩家。

对于直角90度，点积将是\ ``0``\ ，对于窄于90度的角度，点积大于0，对于宽于90度的角度，点积小于0。

当使用归一化单位向量，向量朝向相反方向时，结果总是在\ ``-1.0``\ （180度角）和\ ``1.0``\ （0度角）之间，当向量对齐。

\ **注意：**\ ``a.dot(b)``\ 等同于\ ``b.dot(a)``\ 。

----

.. _class_Vector3_method_floor:

- :ref:`Vector3<class_Vector3>` **floor** **(** **)**

返回一个新的向量，所有的向量都被四舍五入，向负无穷大。

----

.. _class_Vector3_method_inverse:

- :ref:`Vector3<class_Vector3>` **inverse** **(** **)**

返回向量的反值。这与\ ``Vector3( 1.0 / v.x, 1.0 / v.y, 1.0 / v.z )``\ 相同。

----

.. _class_Vector3_method_is_equal_approx:

- :ref:`bool<class_bool>` **is_equal_approx** **(** :ref:`Vector3<class_Vector3>` v **)**

通过对每个分量运行\ :ref:`@GDScript.is_equal_approx<class_@GDScript_method_is_equal_approx>`\ ，如果这个向量和\ ``v``\ 近似相等，返回\ ``true``\ 。

----

.. _class_Vector3_method_is_normalized:

- :ref:`bool<class_bool>` **is_normalized** **(** **)**

如果向量被归一化，返回\ ``true``\ ，否则返回\ ``false``\ 。

----

.. _class_Vector3_method_length:

- :ref:`float<class_float>` **length** **(** **)**

返回这个向量的长度，即大小。

----

.. _class_Vector3_method_length_squared:

- :ref:`float<class_float>` **length_squared** **(** **)**

返回这个向量的平方长度，即平方大小。

这个方法比\ :ref:`length<class_Vector3_method_length>`\ 运行得更快，所以如果你需要比较向量或需要一些公式的平方距离时，更喜欢用它。

----

.. _class_Vector3_method_limit_length:

- :ref:`Vector3<class_Vector3>` **limit_length** **(** :ref:`float<class_float>` length=1.0 **)**

通过限制其长度为\ ``length``\ ，返回具有最大长度的向量。

----

.. _class_Vector3_method_linear_interpolate:

- :ref:`Vector3<class_Vector3>` **linear_interpolate** **(** :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` weight **)**

返回这个向量与\ ``to``\ 之间的线性插值的结果，插值量为\ ``t``\ 。\ ``weight``\ 的范围是0.0到1.0，表示插值的数量。

----

.. _class_Vector3_method_max_axis:

- :ref:`int<class_int>` **max_axis** **(** **)**

返回向量的最大值的轴。参阅\ ``AXIS_*``\ 常量。如果所有分量都相等，该方法返回\ :ref:`AXIS_X<class_Vector3_constant_AXIS_X>`\ 。

----

.. _class_Vector3_method_min_axis:

- :ref:`int<class_int>` **min_axis** **(** **)**

返回矢量的最小值的轴。参阅\ ``AXIS_*``\ 常量。如果所有分量都相等，本方法返回\ :ref:`AXIS_Z<class_Vector3_constant_AXIS_Z>`\ 。

----

.. _class_Vector3_method_move_toward:

- :ref:`Vector3<class_Vector3>` **move_toward** **(** :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` delta **)**

将此向量向\ ``to``\ 移动，以固定\ ``delta``\ 量。

----

.. _class_Vector3_method_normalized:

- :ref:`Vector3<class_Vector3>` **normalized** **(** **)**

返回缩放为单位长度的向量。相当于\ ``v/v.length()``\ 。

----

.. _class_Vector3_method_outer:

- :ref:`Basis<class_Basis>` **outer** **(** :ref:`Vector3<class_Vector3>` b **)**

返回与 ``b`` 的外积。

----

.. _class_Vector3_method_posmod:

- :ref:`Vector3<class_Vector3>` **posmod** **(** :ref:`float<class_float>` mod **)**

返回一个由这个向量分量的\ :ref:`@GDScript.fposmod<class_@GDScript_method_fposmod>`\ 和\ ``mod``\ 组成的向量。

----

.. _class_Vector3_method_posmodv:

- :ref:`Vector3<class_Vector3>` **posmodv** **(** :ref:`Vector3<class_Vector3>` modv **)**

返回一个由这个向量的\ ``modv``\ 分量和\ :ref:`@GDScript.fposmod<class_@GDScript_method_fposmod>`\ 分量组成的向量。

----

.. _class_Vector3_method_project:

- :ref:`Vector3<class_Vector3>` **project** **(** :ref:`Vector3<class_Vector3>` b **)**

返回这个向量投射到另一个向量\ ``b``\ 上的结果。

----

.. _class_Vector3_method_reflect:

- :ref:`Vector3<class_Vector3>` **reflect** **(** :ref:`Vector3<class_Vector3>` n **)**

返回从给定法线定义的平面上反射的向量。

----

.. _class_Vector3_method_rotated:

- :ref:`Vector3<class_Vector3>` **rotated** **(** :ref:`Vector3<class_Vector3>` axis, :ref:`float<class_float>` phi **)**

将此向量绕给定的轴旋转\ ``phi``\ 弧度。该轴必须是归一化的矢量。

----

.. _class_Vector3_method_round:

- :ref:`Vector3<class_Vector3>` **round** **(** **)**

返回这个向量的所有分量都被四舍五入为最接近的整数，中间情况下四舍五入为零。

----

.. _class_Vector3_method_sign:

- :ref:`Vector3<class_Vector3>` **sign** **(** **)**

返回一个向量，每个分量设置为1或负1，取决于这个向量的分量的符号。如果分量为0，则返回正1。

----

.. _class_Vector3_method_signed_angle_to:

- :ref:`float<class_float>` **signed_angle_to** **(** :ref:`Vector3<class_Vector3>` to, :ref:`Vector3<class_Vector3>` axis **)**

返回给定向量的带符号的角度，单位是弧度。当从\ ``axis``\ 指定的一侧看，该角度的符号在逆时针方向是正的，在顺时针方向是负的。

----

.. _class_Vector3_method_slerp:

- :ref:`Vector3<class_Vector3>` **slerp** **(** :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` weight **)**

返回这个向量与\ ``to``\ 之间的球面线性插值的结果，按\ ``weight``\ 的数量。\ ``weight``\ 的范围是0.0到1.0，表示插值的数量。

\ **注意：**\ 两个向量都必须被归一化。

----

.. _class_Vector3_method_slide:

- :ref:`Vector3<class_Vector3>` **slide** **(** :ref:`Vector3<class_Vector3>` n **)**

返回沿着由给定法线定义的平面滑动的向量。

----

.. _class_Vector3_method_snapped:

- :ref:`Vector3<class_Vector3>` **snapped** **(** :ref:`Vector3<class_Vector3>` by **)**

返回这个向量，每个分量都捕捉到\ ``step``\ 的最近倍数。这也可以用来四舍五入到任意数量的小数。

----

.. _class_Vector3_method_to_diagonal_matrix:

- :ref:`Basis<class_Basis>` **to_diagonal_matrix** **(** **)**

返回一个以该向量为主对角线的对角线矩阵。

这相当于一个没有旋转或剪切的Basis，这个向量的分量被设定为缩放。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
