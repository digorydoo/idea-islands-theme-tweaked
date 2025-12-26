Digorydoo's Islands
===================

What is it
----------

This is a dark theme for IntelliJ IDEA, based on the default Islands Dark. Tested with IntelliJ IDEA CE 2025.3.1. It may
or may not work with other versions or other JetBrains products.

What I did
----------

I started with Islands Dark and changed the following:

* Slightly less dark, especially dialogs look more friendly
* Slightly warmer in tone
* Selection colour is more saturated and slightly darker to give white text better contrast
* Tree view guides are much fainter (they're annoyingly bright in default Islands Dark)
* Contextual menus look slightly denser (removed the rounded corners of items, and reduced padding)

How to build it
---------------

Open IntelliJ IDEA.

Go to `Build` > `Build Project`.

Then `Build` > `Prepare plugin for deployment`.

This should generate a JAR file, usually placed in the project root.

How to install
--------------

Open IntelliJ IDEA.

Go to `Settings` > `Plugins` > ⚙️ > `Install plugin from disk`.

Choose the JAR file you built previously. Restart IDE.

TODO
----

* Settings > Appearance > Data editor is too dark
* Settings > Plugins area is too dark
* Settings > Plugins: Foreground colour of selected plugin is hard to read when plugin is disabled
* The theme does not provide an editor scheme. Export scheme as XML, put it somewhere in the resources folder, and refer
  to it from theme.json via top-level key "editorScheme" like this: "/theme/path/to/my/editor/scheme.xml". If done
  correctly, the editor should switch to that scheme when the "Preview" button is pressed.

