# Eclipse Instructions #

This section assumes you have Eclipse and are familiar with the environment and that you have OpenKickOff currently living somewhere on your hard drive. It also is assumed that you do not have Slick as a separate project. Please see the Slick Instructions if you wish to have Slick checked out as a second project (encouraged for developers).

  1. Run ant setup at the command line
  1. Import the project into Eclipse
  1. Right-click the OpenKickOff project > “Build Path” > “Configure Build Path…”
  1. Select the “Libraries” tab
  1. Expand lwjgl.jar, select “Native library location”, select Edit
  1. Select Workspace then navigate to lib/natives/
  1. Click “Ok” then “Ok” then “OK”

Done!. Next, try to run OpenKickOff.

  1. Right click org.openkickoff.OpenKickOff > “Run as…” > “Run as Java Application”

If you plan on editing and submitting changes for Shade then please take a moment to perform one last change.

  1. Open up Eclipse preferences
  1. Expand “Java” and select “Compiler”
  1. Change the “Compiler compliance level” to 1.6