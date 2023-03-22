=====
Views
=====

Views support editors and provide alternative presentations as well as
ways to navigate the information in your Workbench. For example, on the
left side, the Project Explorer displayed by default and other
navigation views display resources that you are working with.

.. _prjexplorer:

Project explorer
----------------

The **Project Explorer** View provides a hierarchical view of the
ECLIPSE project.

.. image:: ../images/ui/viewsimg1.png

To add the Project Explorer view to the current perspective, click
*Window > Show View > Other... > General > Project Explorer*.

.. _tasktracker:

Task tracker
------------

The **Task Tracker View** displays the executed tasks (filtered by
package) from a Platform artifact build sequence and their status are
displayed. It shows the currently executed task, the task done and the
task ended in error to track which step is running.

.. image:: ../images/ui/viewsimg2.png

To add the Task tracker, Go to *Window > Show View > Other... > Platform
> Task Tracker*.

======================================== ======== ===================================
Icon                                     Status   Description
======================================== ======== ===================================
|image1|                                OK       The task has been successfully done
|image2|                                On going The task is currently executed
|image3|                                Pause    The task is pending
|image4|                                Failed   The task has failed
======================================== ======== ===================================

.. |image1| image:: ../images/ui/viewsicon1.png
.. |image2| image:: ../images/ui/viewsicon2.png
.. |image3| image:: ../images/ui/viewsicon3.png
.. |image4| image:: ../images/ui/viewsicon4.png


Some actions can be trigger on this view, right-click on the element to
show the menu:

| - On package: Build or Rebuild
| - On task: Execute, Force Execute or Display log (if a log file
  exists)

.. _buildtracker:

Packages Build tracker
----------------------

The **Package Build tracker** view lists all the package definitions
added to the platform. The user can know the build status for any
packages.


To add the Packages Build tracker, *Go to Window > Show View > Other...
> Platform > Packages Build Tracker*

Console
-------

The **Console View** displays a variety of console types depending on
the type of development and the current set of user settings.

+--------------------------------------+------------------+------------------+------------------+
| Command                              | Name             | Description      | Availability     |
+======================================+==================+==================+==================+
|.. image:: ../images/ui/viewsicon5.png| Clear console    | Clears the       | Context menu and |
|                                      |                  | currently active | view action      |
|                                      |                  | console, and is  |                  |
|                                      |                  | available as     |                  |
|                                      |                  | both a view      |                  |
|                                      |                  | command and a    |                  |
|                                      |                  | contextual menu  |                  |
|                                      |                  | item.            |                  |
+--------------------------------------+------------------+------------------+------------------+
|.. image:: ../images/ui/viewsicon6.png| Display selected | Opens a listing  | View action      |
|                                      | console          | of current       |                  |
|                                      |                  | consoles and     |                  |
|                                      |                  | allows you to    |                  |
|                                      |                  | select which one |                  |
|                                      |                  | you would like   |                  |
|                                      |                  | to see.          |                  |
+--------------------------------------+------------------+------------------+------------------+
|.. image:: ../images/ui/viewsicon7.png| Open console     | Opens a new      | View action      |
|                                      |                  | console of the   |                  |
|                                      |                  | selected type.   |                  |
+--------------------------------------+------------------+------------------+------------------+
|.. image:: ../images/ui/viewsicon8.png| Pin              | Pins the current | View action      |
|                                      |                  | console to       |                  |
|                                      |                  | remain on top of |                  |
|                                      |                  | all other        |                  |
|                                      |                  | consoles.        |                  |
+--------------------------------------+------------------+------------------+------------------+
|.. image:: ../images/ui/viewsicon9.png| Scroll lock      | Changes if       | Context menu and |
|                                      |                  | scroll lock      | view action      |
|                                      |                  | should be        |                  |
|                                      |                  | enabled or not   |                  |
|                                      |                  | in the current   |                  |
|                                      |                  | console.         |                  |
+--------------------------------------+------------------+------------------+------------------+

--------------
