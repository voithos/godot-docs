.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the InputEvent.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_InputEvent:

InputEvent
==========

**Inherits:** :ref:`Resource<class_resource>` **<** :ref:`Reference<class_reference>` **<** :ref:`Object<class_object>`

**Inherited By:** :ref:`InputEventScreenTouch<class_inputeventscreentouch>`, :ref:`InputEventWithModifiers<class_inputeventwithmodifiers>`, :ref:`InputEventScreenDrag<class_inputeventscreendrag>`, :ref:`InputEventJoypadMotion<class_inputeventjoypadmotion>`, :ref:`InputEventJoypadButton<class_inputeventjoypadbutton>`, :ref:`InputEventAction<class_inputeventaction>`

**Category:** Core

Brief Description
-----------------

Generic input event

Member Functions
----------------

+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_string>`          | :ref:`as_text<class_InputEvent_as_text>` **(** **)** const                                                                                                            |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`            | :ref:`get_action_strength<class_InputEvent_get_action_strength>` **(** :ref:`String<class_string>` action **)** const                                                 |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`              | :ref:`is_action<class_InputEvent_is_action>` **(** :ref:`String<class_string>` action **)** const                                                                     |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`              | :ref:`is_action_pressed<class_InputEvent_is_action_pressed>` **(** :ref:`String<class_string>` action **)** const                                                     |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`              | :ref:`is_action_released<class_InputEvent_is_action_released>` **(** :ref:`String<class_string>` action **)** const                                                   |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`              | :ref:`is_action_type<class_InputEvent_is_action_type>` **(** **)** const                                                                                              |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`              | :ref:`is_echo<class_InputEvent_is_echo>` **(** **)** const                                                                                                            |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`              | :ref:`is_pressed<class_InputEvent_is_pressed>` **(** **)** const                                                                                                      |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`              | :ref:`shortcut_match<class_InputEvent_shortcut_match>` **(** :ref:`InputEvent<class_inputevent>` event **)** const                                                    |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`InputEvent<class_inputevent>`  | :ref:`xformed_by<class_InputEvent_xformed_by>` **(** :ref:`Transform2D<class_transform2d>` xform, :ref:`Vector2<class_vector2>` local_ofs=Vector2( 0, 0 ) **)** const |
+--------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_InputEvent_device:

- :ref:`int<class_int>` **device** - The event's device ID.


Description
-----------

Base class of all sort of input event. See :ref:`Node._input<class_Node__input>`.

Tutorials
---------

- :doc:`../tutorials/inputs/inputevent`
- :doc:`../tutorials/2d/2d_transforms`

Member Function Description
---------------------------

.. _class_InputEvent_as_text:

- :ref:`String<class_string>` **as_text** **(** **)** const

Returns a :ref:`String<class_string>` representation of the event.

.. _class_InputEvent_get_action_strength:

- :ref:`float<class_float>` **get_action_strength** **(** :ref:`String<class_string>` action **)** const

.. _class_InputEvent_is_action:

- :ref:`bool<class_bool>` **is_action** **(** :ref:`String<class_string>` action **)** const

Returns ``true`` if this input event matches a pre-defined action of any type.

.. _class_InputEvent_is_action_pressed:

- :ref:`bool<class_bool>` **is_action_pressed** **(** :ref:`String<class_string>` action **)** const

Returns ``true`` if the given action is being pressed (and is not an echo event for KEY events). Not relevant for the event types ``MOUSE_MOTION``, ``SCREEN_DRAG`` or ``NONE``.

.. _class_InputEvent_is_action_released:

- :ref:`bool<class_bool>` **is_action_released** **(** :ref:`String<class_string>` action **)** const

Returns ``true`` if the given action is released (i.e. not pressed). Not relevant for the event types ``MOUSE_MOTION``, ``SCREEN_DRAG`` or ``NONE``.

.. _class_InputEvent_is_action_type:

- :ref:`bool<class_bool>` **is_action_type** **(** **)** const

Returns ``true`` if this input event's type is one of the ``InputEvent`` constants.

.. _class_InputEvent_is_echo:

- :ref:`bool<class_bool>` **is_echo** **(** **)** const

Returns ``true`` if this input event is an echo event (only for events of type KEY).

.. _class_InputEvent_is_pressed:

- :ref:`bool<class_bool>` **is_pressed** **(** **)** const

Returns ``true`` if this input event is pressed. Not relevant for the event types ``MOUSE_MOTION``, ``SCREEN_DRAG`` or ``NONE``.

.. _class_InputEvent_shortcut_match:

- :ref:`bool<class_bool>` **shortcut_match** **(** :ref:`InputEvent<class_inputevent>` event **)** const

.. _class_InputEvent_xformed_by:

- :ref:`InputEvent<class_inputevent>` **xformed_by** **(** :ref:`Transform2D<class_transform2d>` xform, :ref:`Vector2<class_vector2>` local_ofs=Vector2( 0, 0 ) **)** const


