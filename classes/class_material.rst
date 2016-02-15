.. _class_Material:

Material
========

**Inherits:** :ref:`Resource<class_resource>` **<** :ref:`Reference<class_reference>` **<** :ref:`Object<class_object>`

**Inherited By:** :ref:`ShaderMaterial<class_shadermaterial>`, :ref:`FixedMaterial<class_fixedmaterial>`

**Category:** Core

Brief Description
-----------------

Abstract base :ref:`Resource<class_resource>` for coloring and shading geometry.

Member Functions
----------------

+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_flag<class_Material_set_flag>`  **(** :ref:`int<class_int>` flag, :ref:`bool<class_bool>` enable  **)** |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`    | :ref:`get_flag<class_Material_get_flag>`  **(** :ref:`int<class_int>` flag  **)** const                           |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_blend_mode<class_Material_set_blend_mode>`  **(** :ref:`int<class_int>` mode  **)**                     |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`      | :ref:`get_blend_mode<class_Material_get_blend_mode>`  **(** **)** const                                           |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_line_width<class_Material_set_line_width>`  **(** :ref:`float<class_float>` width  **)**                |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`  | :ref:`get_line_width<class_Material_get_line_width>`  **(** **)** const                                           |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_depth_draw_mode<class_Material_set_depth_draw_mode>`  **(** :ref:`int<class_int>` mode  **)**           |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`      | :ref:`get_depth_draw_mode<class_Material_get_depth_draw_mode>`  **(** **)** const                                 |
+----------------------------+-------------------------------------------------------------------------------------------------------------------+

Numeric Constants
-----------------

- **FLAG_VISIBLE** = **0** --- Geometry is visible when this flag is enabled (default).
- **FLAG_DOUBLE_SIDED** = **1** --- Both front facing and back facing triangles are rendered when this flag is enabled.
- **FLAG_INVERT_FACES** = **2** --- Front facing and back facing order is swapped when this flag is enabled.
- **FLAG_UNSHADED** = **3** --- Shading (lighting) is disabled when this flag is enabled.
- **FLAG_ONTOP** = **4**
- **FLAG_LIGHTMAP_ON_UV2** = **5**
- **FLAG_COLOR_ARRAY_SRGB** = **6**
- **FLAG_MAX** = **7** --- Maximum amount of flags.
- **DEPTH_DRAW_ALWAYS** = **0**
- **DEPTH_DRAW_OPAQUE_ONLY** = **1**
- **DEPTH_DRAW_OPAQUE_PRE_PASS_ALPHA** = **2**
- **DEPTH_DRAW_NEVER** = **3**
- **BLEND_MODE_MIX** = **0** --- Use the regular alpha blending equation (source and dest colors are faded) (default).
- **BLEND_MODE_ADD** = **1** --- Use additive blending equation, often used for particle effects such as fire or light decals.
- **BLEND_MODE_SUB** = **2** --- Use substractive blending equation, often used for some smoke effects or types of glass.
- **BLEND_MODE_MUL** = **3**
- **BLEND_MODE_PREMULT_ALPHA** = **4**

Description
-----------

Material is a base :ref:`Resource<class_resource>` used for coloring and shading geometry. All materials inherit from it and almost all :ref:`VisualInstance<class_visualinstance>` derived nodes carry a Material. A few flags and parameters are shared between all material types and are configured here.

Member Function Description
---------------------------

.. _class_Material_set_flag:

- void  **set_flag**  **(** :ref:`int<class_int>` flag, :ref:`bool<class_bool>` enable  **)**

Set a :ref:`Material<class_material>` flag, which toggles on or off a behavior when rendering. See enumeration FLAG\_\* for a list.

.. _class_Material_get_flag:

- :ref:`bool<class_bool>`  **get_flag**  **(** :ref:`int<class_int>` flag  **)** const

Return a :ref:`Material<class_material>` flag, which toggles on or off a behavior when rendering. See enumeration FLAG\_\* for a list.

.. _class_Material_set_blend_mode:

- void  **set_blend_mode**  **(** :ref:`int<class_int>` mode  **)**

Set blend mode for the material, which can be one of BLEND_MODE_MIX (default), BLEND_MODE_ADD, BLEND_MODE_SUB. Keep in mind that only BLEND_MODE_MIX ensures that the material *may* be opaque, any other blend mode will render with alpha blending enabled in raster-based :ref:`VisualServer<class_visualserver>` implementations.

.. _class_Material_get_blend_mode:

- :ref:`int<class_int>`  **get_blend_mode**  **(** **)** const

Return blend mode for the material, which can be one of BLEND_MODE_MIX (default), BLEND_MODE_ADD, BLEND_MODE_SUB. Keep in mind that only BLEND_MODE_MIX ensures that the material *may* be opaque, any other blend mode will render with alpha blending enabled in raster-based :ref:`VisualServer<class_visualserver>` implementations.

.. _class_Material_set_line_width:

- void  **set_line_width**  **(** :ref:`float<class_float>` width  **)**

Set the line width for geometry drawn with FLAG_WIREFRAME enabled, or LINE primitives. Note that not all hardware or VisualServer backends support this (like DirectX).

.. _class_Material_get_line_width:

- :ref:`float<class_float>`  **get_line_width**  **(** **)** const

Return the line width for geometry drawn with FLAG_WIREFRAME enabled, or LINE primitives. Note that not all hardware or VisualServer backends support this (like DirectX).

.. _class_Material_set_depth_draw_mode:

- void  **set_depth_draw_mode**  **(** :ref:`int<class_int>` mode  **)**

.. _class_Material_get_depth_draw_mode:

- :ref:`int<class_int>`  **get_depth_draw_mode**  **(** **)** const

