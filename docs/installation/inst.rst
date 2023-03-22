============
Installation
============

This section describes the installation of the **System Workbench for
Linux** plug-ins as well as their dependencies.

.. _CorePlugins:

Core Plugins
------------

-  Platform (fr.ac6.platform) with Makefile, Autotools, CDT, Rootfs,
   Kernel, Prebuilt packages support
-  Compiler and Toolset (fr.ac6.linux.compiler and fr.ac6.linux.toolset)
-  Linux Kernel (fr.ac6.linux.kernel)
-  Linux Kernel Modules (fr.ac6.linux.module)
-  Modules (fr.ac6.linux.module)
-  SW Library manager (fr.ac6.library)

New plugins will be released to support additional features.

.. _Prerequisites:

Prerequisites
-------------

If you do not have ECLIPSE™ installed on your machine. You should grab
the appropriate ECLIPSE™ package from
`www.eclipse.org <www.eclipse.org>`__ website.

ECLIPSE™ itself is in great part written in Java; you thus must install
the ORACLE® Java Runtime Environment (JRE); you must install a version
of the JRE that match the ECLIPSE™ version installed (both should be 32
or 64 bits versions).

.. _SoftRequirements:

Sotfware Requirements:
~~~~~~~~~~~~~~~~~~~~~~

-  ECLIPSE™ C/C++ Development, Neon is the minimal version supported
-  System Workbench for Linux only runs on Linux distribution (such as
   Ubuntu 14.04)
-  ORACLE® Java Platform SE 1.7 JRE or alternatives (such as OpenJDK
   1.7)

.. _PackagesRequirements:

Packages Requirements:
~~~~~~~~~~~~~~~~~~~~~~

-  Build-essential (set of tools to build packages)
-  Mkimage (command to create image for U-boot)

.. _Install:

Install and automatic updates from update-site
----------------------------------------------

To install Ac6 System Workbench, start ECLIPSE™ then open the
installation window on the main menu *Help > Install New Software*.

You must then create a new update site, to be able to install System
Workbench for Linux. Click on **Add button**. Enter the update-site name
and set le location to:

+---------+-------------------------------------------------------------------------------------+
| Version | Update-site URL                                                                     |
+=========+=====================================================================================+
| Release | http://www.ac6-tools.com/Eclipse-updates/fr.ac6.system.workbench.linux.update-site/ |
+---------+-------------------------------------------------------------------------------------+

Then select it in the **Work with** area. The available plug-ins are
displayed in the table below. Please, select the plug-ins you need and
confirm the installation. Be aware that Ac6 System Workbench has
dependency with many ECLIPSE™ plug-ins, these plug-ins are automatically
installed if they have not been found. Installation and updates might
take several minutes to complete.

You have to accept the license agreement and System Workbench for Linux
edition will be installed in your ECLIPSE™ setup.

Note that you will probably have to restart ECLIPSE™ for the tools to be
available; ECLIPSE™ will automatically suggest the restart.

.. _Issues:

In case of installation issues
------------------------------

If you encounter problems during the installation for System Workbench
from ECLIPSE™, you should close and restart ECLIPSE™ then relaunch the
installation (the update site definition should still be there, but you
should check it is correct). Sometimes, ECLIPSE™ needs you to restart
the installation to pick all dependents.

You may also encounter problems on older ECLIPSE™ version when updating
your installation where ECLIPSE™ can't install both ECLIPSE™ or CDT
updates and System Workbench updates (this can the case if updating from
Kepler-SR1 to SR2's CDT and upgrading to the latest version of System
Workbench for Linux); in this case install first the ECLIPSE™ updates
(an ECLIPSE™ restart may be required), then the System Workbench
updates.

--------------
