.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the BakedLightmap.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_BakedLightmap:

BakedLightmap
=============

**Inherits:** :ref:`VisualInstance<class_visualinstance>` **<** :ref:`Spatial<class_spatial>` **<** :ref:`Node<class_node>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

Prerendered indirect light map for a scene.

Member Functions
----------------

+-------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`BakeError<enum_bakedlightmap_bakeerror>`  | :ref:`bake<class_BakedLightmap_bake>` **(** :ref:`Node<class_node>` from_node=null, :ref:`bool<class_bool>` create_visual_debug=false **)** |
+-------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`debug_bake<class_BakedLightmap_debug_bake>` **(** **)**                                                                               |
+-------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_BakedLightmap_bake_cell_size:

- :ref:`float<class_float>` **bake_cell_size** - Grid subdivision size for lightmapper calculation. Default value of ``0.25`` will work for most cases. Increase for better lighting on small details or if your scene is very large.

  .. _class_BakedLightmap_bake_energy:

- :ref:`float<class_float>` **bake_energy**

  .. _class_BakedLightmap_bake_extents:

- :ref:`Vector3<class_vector3>` **bake_extents** - Size of affected area.

  .. _class_BakedLightmap_bake_hdr:

- :ref:`bool<class_bool>` **bake_hdr** - If ``true`` lightmap can capture light values greater than ``1.0``. Turning this off will result in a smaller lightmap. Default value:``false``.

  .. _class_BakedLightmap_bake_mode:

- :ref:`BakeMode<enum_bakedlightmap_bakemode>` **bake_mode** - Lightmapping mode. See :ref:`BakeMode<enum_@globalscope_bakemode>`.

  .. _class_BakedLightmap_bake_propagation:

- :ref:`float<class_float>` **bake_propagation**

  .. _class_BakedLightmap_bake_quality:

- :ref:`BakeQuality<enum_bakedlightmap_bakequality>` **bake_quality** - Three quality modes are available. Higher quality requires more rendering time. See :ref:`BakeQuality<enum_@globalscope_bakequality>`.

  .. _class_BakedLightmap_capture_cell_size:

- :ref:`float<class_float>` **capture_cell_size** - Grid size used for real-time capture information on dynamic objects. Cannot be larger than :ref:`bake_cell_size<class_BakedLightmap_bake_cell_size>`.

  .. _class_BakedLightmap_image_path:

- :ref:`String<class_string>` **image_path** - Location where lightmaps will be saved.

  .. _class_BakedLightmap_light_data:

- :ref:`BakedLightmapData<class_bakedlightmapdata>` **light_data** - The calculated light data.


Enums
-----

  .. _enum_BakedLightmap_BakeQuality:

enum **BakeQuality**

- **BAKE_QUALITY_LOW** = **0** --- Lowest bake quality mode. Fastest to calculate.
- **BAKE_QUALITY_MEDIUM** = **1** --- Default bake quality mode.
- **BAKE_QUALITY_HIGH** = **2** --- Highest bake quality mode. Takes longer to calculate.

  .. _enum_BakedLightmap_BakeError:

enum **BakeError**

- **BAKE_ERROR_OK** = **0**
- **BAKE_ERROR_NO_SAVE_PATH** = **1**
- **BAKE_ERROR_NO_MESHES** = **2**
- **BAKE_ERROR_CANT_CREATE_IMAGE** = **3**
- **BAKE_ERROR_USER_ABORTED** = **4**

  .. _enum_BakedLightmap_BakeMode:

enum **BakeMode**

- **BAKE_MODE_CONE_TRACE** = **0** --- Less precise but faster bake mode.
- **BAKE_MODE_RAY_TRACE** = **1** --- More precise bake mode but can take considerably longer to bake.


Description
-----------

Baked lightmaps are an alternative workflow for adding indirect (or baked) lighting to a scene. Unlike the :ref:`GIProbe<class_giprobe>` approach, baked lightmaps work fine on low-end PCs and mobile devices as they consume almost no resources in run-time.

Tutorials
---------

- :doc:`../tutorials/3d/baked_lightmaps`

Member Function Description
---------------------------

.. _class_BakedLightmap_bake:

- :ref:`BakeError<enum_bakedlightmap_bakeerror>` **bake** **(** :ref:`Node<class_node>` from_node=null, :ref:`bool<class_bool>` create_visual_debug=false **)**

.. _class_BakedLightmap_debug_bake:

- void **debug_bake** **(** **)**


