Digorydoo's Islands
===================

What the heck is this?
----------------------

It's a dark theme for IntelliJ IDEA, based on the default Islands Dark. Tested with IntelliJ IDEA CE 2025.3.1. It may
or may not work with other versions or other Jetbrains products.

What I did
----------

I started with Islands Dark and changed the following:

   * Slightly less dark, especially dialogs look more friendly
   * Slightly warmer in tone
   * Selection colour is more saturated and slightly darker to give white text better contrast
   * Tree view guides are much fainter (they're annoyingly bright in default Islands Dark)
   * Contextual menus look slightly denser (removed the rounded corners of items, and reduced padding)

How to install
--------------

Open IntelliJ IDEA.

Go to Settings > Plugins.

Click the gear, choose "Install plugin from disk".

Pick the JAR file. No JAR? Well... build it first, genius!

How to build it
---------------

Open IntelliJ IDEA (duh).

Build > Build Project.

Build > Prepare plugin for deployment.

Here you are: a shiny JAR file, usually chilling in your project root.

How to test, debug, or... tweak?!
---------------------------------

Grab the Plugin Devkit from the IDEA marketplace.

Open `resources/theme/*.theme.json`.

Hit the preview button. See how the theme is *not* supposed to look. Well... The preview is a little unreliable.
Parent theme keys might be ignored, usually leaving you staring at a blinding white editor. So really, build the JAR
and install it. Yes, for every change. Yes, restart required. Yes, annoying.

Inside the JSON, `colors` keys are arbitrary names, which you can then use in the `ui` section. Editor auto-completion
exists, but it's a mischievous sprite. Sometimes it underlines things that totally work. Sometimes it doesn't underline
things that refuse to cooperate. Documentation? Ha! Good luck. Chatbots may be your only hope.
