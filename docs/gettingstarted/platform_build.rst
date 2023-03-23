============
Build System
============

System Workbench provides the following default build sequence for a
package definition.

--------------

.. _About:

Default Build sequence on Packages
----------------------------------

-  **Fetch:** Fetch the sources from the package location into the
   download directory
-  **Import:** Import the sources as ECLIPSE™ project into the
   workspace. The sources are copied into the workspace location
-  **Copy resources:** Copy the additional resources from platform into
   package project. It overwrite existing resources
-  **Apply patches:** Apply the patches in alpha-numerical order into
   the package project. When relaunched, it undo the previous patches
   first
-  **Configure:** Configure the project (might to nothing if not needed)
-  **Compile:** Compile the project
-  **Install:** Install the binaries into project temporary folder named
   “_install”
-  **Split:** Create subpackage feeds from binaries. It fails if a file
   in the install folder has not been put in a subpackage.
-  **Populate Sysroot:** Populate the platform sysroots with the
   subpackage feeds. When relaunched, it removes subpackages items from
   previous populate sysroot first.

--------------

.. _About:

Default Build sequence on Kernel
--------------------------------

-  **Fetch:** Fetch the sources from the package location into the
   download directory
-  **Import:** Import the sources as ECLIPSE™ project into the workspace
-  **Copy resources:** Copy the additional resources from platform into
   package project
-  **Apply patches:** Apply the patches in alpha-numerical order into
   the package project
-  **Configure Default Target:** Configure the kernel source for
   selected target
-  **Compile Image:** Compile the kernel
-  **Compile Device Tree:** Compile the selected device tree

--------------

.. _About:

Default Build sequence on Rootfs
--------------------------------

-  **Fetch:** Fetch the sources from the package location into the
   download directory
-  **Import:** Import the sources as ECLIPSE™ project into the workspace
-  **Copy resources:** Copy the additional resources from platform into
   package project
-  **Generate Skeleton:** Create the Rootfs skeleton under the
   “output/rootfs” directory
-  **Populate Rootfs:** Install selected package feeds into the
   generated rootfs skeleton
-  **Copy libraries:** Check the required compiler libraries and copy
   them into the Rootfs if required
-  **Create Image:** Generate the Rootfs image from “output/rootfs” into
   “output/image” folder

--------------

.. _About:

Modifying the build sequence
----------------------------

The build sequences can be customized in many ways. You can add or
remove tasks from the sequence or modify a task behavior. System
Workbench for Linux provides a set of tasks that the user can select or
duplicate. A custom task can be created by providing a shell script
which will be executed in the build sequence. The shell script are
executed in the package project directory. Variables set in package
definition or platform are persistent. The script shell should return 0
when the action is successful otherwise the build sequence might
indicate failure.

--------------

