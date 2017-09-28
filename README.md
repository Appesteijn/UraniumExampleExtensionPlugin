Example Extension
=================

This is an example extension plug-in for Uranium.

The extension type plug-in is a "generic" type of plug-in that just gets some object constructed upon loading the plug-in for the first time. Using the initialisation of that class as starting point for your code, you can access all of the application.

There are two typical use cases for extensions:
1. Modifying some behaviour in the application or modifying current functionality. This is done by listening to the desired event, such as the changing of the current machine or on start-up. When that event happens, some code can be executed that adds on the behaviour.
2. Adding a dialogue that provides additional functionality. There is a handy built-in method that allows you to add a menu item easily, and what should happen when the user clicks on it.

This plug-in shows an example of both use cases.

Packaging
---------

To package your plug-in, use the packaging script in Uranium: https://github.com/Ultimaker/Uranium/blob/master/create_plugin.py

Try the following command:

    python3 /path/to/Uranium/create_plugin.py plugin_location /path/to/UraniumExampleExtensionPlugin

That should produce a .plugin file that can be added to any application based on Uranium.