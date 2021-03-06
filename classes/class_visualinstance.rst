.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualInstance.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualInstance:

VisualInstance
==============

**Inherits:** :ref:`Spatial<class_spatial>` **<** :ref:`Node<class_node>` **<** :ref:`Object<class_object>`

**Inherited By:** :ref:`BakedLightmap<class_bakedlightmap>`, :ref:`Light<class_light>`, :ref:`RootMotionView<class_rootmotionview>`, :ref:`ReflectionProbe<class_reflectionprobe>`, :ref:`CSGShape<class_csgshape>`, :ref:`GIProbe<class_giprobe>`, :ref:`GeometryInstance<class_geometryinstance>`

**Category:** Core

Brief Description
-----------------



Member Functions
----------------

+--------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_aabb>`  | :ref:`get_aabb<class_VisualInstance_get_aabb>` **(** **)** const                                                                            |
+--------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`  | :ref:`get_layer_mask_bit<class_VisualInstance_get_layer_mask_bit>` **(** :ref:`int<class_int>` layer **)** const                            |
+--------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_aabb>`  | :ref:`get_transformed_aabb<class_VisualInstance_get_transformed_aabb>` **(** **)** const                                                    |
+--------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`set_base<class_VisualInstance_set_base>` **(** :ref:`RID<class_rid>` base **)**                                                       |
+--------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`set_layer_mask_bit<class_VisualInstance_set_layer_mask_bit>` **(** :ref:`int<class_int>` layer, :ref:`bool<class_bool>` enabled **)** |
+--------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_VisualInstance_layers:

- :ref:`int<class_int>` **layers** - The render layer(s) this VisualInstance is drawn on.

This object will only be visible for :ref:`Camera<class_camera>`\ s whose cull mask includes the render object this VisualInstance is set to.


Member Function Description
---------------------------

.. _class_VisualInstance_get_aabb:

- :ref:`AABB<class_aabb>` **get_aabb** **(** **)** const

Returns the :ref:`AABB<class_aabb>` (also known as the bounding box) for this VisualInstance.

.. _class_VisualInstance_get_layer_mask_bit:

- :ref:`bool<class_bool>` **get_layer_mask_bit** **(** :ref:`int<class_int>` layer **)** const

.. _class_VisualInstance_get_transformed_aabb:

- :ref:`AABB<class_aabb>` **get_transformed_aabb** **(** **)** const

Returns the transformed :ref:`AABB<class_aabb>` (also known as the bounding box) for this VisualInstance.

Transformed in this case means the :ref:`AABB<class_aabb>` plus the position, rotation, and scale of the :ref:`Spatial<class_spatial>`\ s :ref:`Transform<class_transform>`

.. _class_VisualInstance_set_base:

- void **set_base** **(** :ref:`RID<class_rid>` base **)**

Sets the base of the VisualInstance, which changes how the engine handles the VisualInstance under the hood.

It is recommended to only use set_base if you know what you're doing.

.. _class_VisualInstance_set_layer_mask_bit:

- void **set_layer_mask_bit** **(** :ref:`int<class_int>` layer, :ref:`bool<class_bool>` enabled **)**


