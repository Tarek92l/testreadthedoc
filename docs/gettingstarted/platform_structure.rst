==========================
Platform project structure
==========================

The Platform project is composed of the following files and folders:

-  **.project:** ECLIPSETM project description file (do not modify it!)

-  **ac6_platform_manifest.xml:** Platform project manifest file, it
   contains the Platform properties. Double click on it to open the
   Platform Editor.

-  **scripts:** Input folder where the user can add its own scripts
   which can be executed on the build steps.

-  **resources:** Folder where the platform local resources are stored.
   PLATFORM_RESOURCES_LOC variable to this folder location.

-  **metadata:** Input folder where the internal packages description
   file are located. If user manually modifies the contents, close then
   open the Platform editor once again to reload the metadata.

-  **feeds:** Output folder where the feeds are generated

-  **sysroots:** Output folder where the packages are installed

-  

   -  **target sysroot (with architecture name):** folder where the
      cross-compiled binaries (executables, libraries...) are installed.
   -  **native:** native system location where the compiler and tools
      are installed

