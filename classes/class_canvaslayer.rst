.. _class_CanvasLayer:

CanvasLayer
===========

**Inherits:** :ref:`Node<class_node>` **<** :ref:`Object<class_object>`

**Inherited By:** :ref:`ParallaxBackground<class_parallaxbackground>`

**Category:** Core

Brief Description
-----------------

Canvas Item layer.

Member Functions
----------------

+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_layer<class_CanvasLayer_set_layer>`  **(** :ref:`int<class_int>` layer  **)**                       |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`get_layer<class_CanvasLayer_get_layer>`  **(** **)** const                                              |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_transform<class_CanvasLayer_set_transform>`  **(** :ref:`Matrix32<class_matrix32>` transform  **)** |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`Matrix32<class_matrix32>`  | :ref:`get_transform<class_CanvasLayer_get_transform>`  **(** **)** const                                      |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_offset<class_CanvasLayer_set_offset>`  **(** :ref:`Vector2<class_vector2>` offset  **)**            |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_vector2>`    | :ref:`get_offset<class_CanvasLayer_get_offset>`  **(** **)** const                                            |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_rotation<class_CanvasLayer_set_rotation>`  **(** :ref:`float<class_float>` rotation  **)**          |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`get_rotation<class_CanvasLayer_get_rotation>`  **(** **)** const                                        |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_scale<class_CanvasLayer_set_scale>`  **(** :ref:`Vector2<class_vector2>` scale  **)**               |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_vector2>`    | :ref:`get_scale<class_CanvasLayer_get_scale>`  **(** **)** const                                              |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| Canvas                           | :ref:`get_world_2d<class_CanvasLayer_get_world_2d>`  **(** **)** const                                        |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_rid>`            | :ref:`get_viewport<class_CanvasLayer_get_viewport>`  **(** **)** const                                        |
+----------------------------------+---------------------------------------------------------------------------------------------------------------+

Description
-----------

Canvas Item layer. :ref:`CanvasItem<class_canvasitem>` nodes that are direct or indirect children of a :ref:`CanvasLayer<class_canvaslayer>` will be drawn in that layer. The layer is a numeric index that defines the draw order. The default 2D scene renders with index 0, so a :ref:`CanvasLayer<class_canvaslayer>` with index -1 will be drawn below, and one with index 1 will be drawn above. This is very useful for HUDs (in layer 1+ or above), or backgrounds (in layer -1 or below).

Member Function Description
---------------------------

.. _class_CanvasLayer_set_layer:

- void  **set_layer**  **(** :ref:`int<class_int>` layer  **)**

Set the layer index, determines the draw order, a lower value will be below a higher one.

.. _class_CanvasLayer_get_layer:

- :ref:`int<class_int>`  **get_layer**  **(** **)** const

Return the layer index, determines the draw order, a lower value will be below a higher one.

.. _class_CanvasLayer_set_transform:

- void  **set_transform**  **(** :ref:`Matrix32<class_matrix32>` transform  **)**

Set the base transform for this layer.

.. _class_CanvasLayer_get_transform:

- :ref:`Matrix32<class_matrix32>`  **get_transform**  **(** **)** const

Return the base transform for this layer.

.. _class_CanvasLayer_set_offset:

- void  **set_offset**  **(** :ref:`Vector2<class_vector2>` offset  **)**

Set the base offset for this layer (helper).

.. _class_CanvasLayer_get_offset:

- :ref:`Vector2<class_vector2>`  **get_offset**  **(** **)** const

Return the base offset for this layer (helper).

.. _class_CanvasLayer_set_rotation:

- void  **set_rotation**  **(** :ref:`float<class_float>` rotation  **)**

Set the base rotation for this layer (helper).

.. _class_CanvasLayer_get_rotation:

- :ref:`float<class_float>`  **get_rotation**  **(** **)** const

Return the base rotation for this layer (helper).

.. _class_CanvasLayer_set_scale:

- void  **set_scale**  **(** :ref:`Vector2<class_vector2>` scale  **)**

Set the base scale for this layer (helper).

.. _class_CanvasLayer_get_scale:

- :ref:`Vector2<class_vector2>`  **get_scale**  **(** **)** const

Return the base scale for this layer (helper).

.. _class_CanvasLayer_get_world_2d:

- Canvas  **get_world_2d**  **(** **)** const

Return the :ref:`World2D<class_world2d>` used by this layer.

.. _class_CanvasLayer_get_viewport:

- :ref:`RID<class_rid>`  **get_viewport**  **(** **)** const

Return the viewport RID for this layer.

