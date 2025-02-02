:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/ConfirmationDialog.xml.

.. _class_ConfirmationDialog:

ConfirmationDialog
==================

**Inherits:** :ref:`AcceptDialog<class_AcceptDialog>` **<** :ref:`Window<class_Window>` **<** :ref:`Viewport<class_Viewport>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`EditorCommandPalette<class_EditorCommandPalette>`, :ref:`EditorFileDialog<class_EditorFileDialog>`, :ref:`FileDialog<class_FileDialog>`, :ref:`ScriptCreateDialog<class_ScriptCreateDialog>`

Dialog for confirmation of actions.

Description
-----------

Dialog for confirmation of actions. This dialog inherits from :ref:`AcceptDialog<class_AcceptDialog>`, but has by default an OK and Cancel button (in host OS order).

To get cancel action, you can use:


.. tabs::

 .. code-tab:: gdscript

    get_cancel_button().pressed.connect(self.cancelled)

 .. code-tab:: csharp

    GetCancelButton().Pressed += Cancelled;



Properties
----------

+---------------------------------+---------------------------------------------------------------------------------+---------------------------------------------------------------------------------+
| :ref:`String<class_String>`     | :ref:`cancel_button_text<class_ConfirmationDialog_property_cancel_button_text>` | ``"Cancel"``                                                                    |
+---------------------------------+---------------------------------------------------------------------------------+---------------------------------------------------------------------------------+
| :ref:`Vector2i<class_Vector2i>` | min_size                                                                        | ``Vector2i(200, 70)`` (overrides :ref:`Window<class_Window_property_min_size>`) |
+---------------------------------+---------------------------------------------------------------------------------+---------------------------------------------------------------------------------+
| :ref:`Vector2i<class_Vector2i>` | size                                                                            | ``Vector2i(200, 100)`` (overrides :ref:`Window<class_Window_property_size>`)    |
+---------------------------------+---------------------------------------------------------------------------------+---------------------------------------------------------------------------------+
| :ref:`String<class_String>`     | title                                                                           | ``"Please Confirm..."`` (overrides :ref:`Window<class_Window_property_title>`)  |
+---------------------------------+---------------------------------------------------------------------------------+---------------------------------------------------------------------------------+

Methods
-------

+-----------------------------+-----------------------------------------------------------------------------------------+
| :ref:`Button<class_Button>` | :ref:`get_cancel_button<class_ConfirmationDialog_method_get_cancel_button>` **(** **)** |
+-----------------------------+-----------------------------------------------------------------------------------------+

Property Descriptions
---------------------

.. _class_ConfirmationDialog_property_cancel_button_text:

- :ref:`String<class_String>` **cancel_button_text**

+-----------+-------------------------------+
| *Default* | ``"Cancel"``                  |
+-----------+-------------------------------+
| *Setter*  | set_cancel_button_text(value) |
+-----------+-------------------------------+
| *Getter*  | get_cancel_button_text()      |
+-----------+-------------------------------+

The text displayed by the cancel button (see :ref:`get_cancel_button<class_ConfirmationDialog_method_get_cancel_button>`).

Method Descriptions
-------------------

.. _class_ConfirmationDialog_method_get_cancel_button:

- :ref:`Button<class_Button>` **get_cancel_button** **(** **)**

Returns the cancel button.

\ **Warning:** This is a required internal node, removing and freeing it may cause a crash. If you wish to hide it or any of its children, use their :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` property.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
