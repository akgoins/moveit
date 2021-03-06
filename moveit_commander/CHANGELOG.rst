^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package moveit_commander
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.6.1 (2016-04-28)
------------------
* [feat] Add the possibility to choose description file `#43 <https://github.com/ros-planning/moveit_commander/issues/43>`_
* [improve] support pyassimp 3.2. Looks like they changed their import path. robot_description should not be hardcoded to allow changing the name of the description file. This is usefull when working with several robots that do not share the same description file. `#45 <https://github.com/ros-planning/moveit_commander/issues/45>`_
* [improve] add queue_size option in planning_scene_interface.py `#41 <https://github.com/ros-planning/moveit_commander/issues/41>`_
* Contributors: Dave Coleman, Isaac I.Y. Saito, Kei Okada, Michael Görner, buschbapti

0.6.0 (2016-01-30)
------------------
* Merge pull request #38  from 130s/doc/python_if
  [RobotCommander] Fill in in-code document where missing.
* [moveit_commander/robot.py] Code cleaning; semi-PEP8.
* Merge pull request #35  from MichaelStevens/set_num_planning_attempts
  adding set_num_planning_attempts to commander interface
* Merge pull request #30 from ymollard/indigo-devel
  Planning scene improvements +  added python wrapper for MoveGroup.asyncExecute()
* Added python wrapper for MoveGroup.asyncExecute()
* Allow to clean all objects in a row
* Allow to attash an existing object without recreating the whole CollisionObject
* Merge pull request #24  from ymollard/hydro-devel
  Allowed user to change the scale of a mesh
* Merge pull request #23  from HumaRobotics/hydro-devel
  Fixed arguments removal in python roscpp_initializer
* Merge pull request #26  from corot/hydro-devel
  Add missing variants of place (PlaceLocation, place anywhere)
* Added a way to change the size of a mesh when grasping
* Allowed user to change the scale of a mesh
* Fixed arguments removal in python roscpp_initializer
* Contributors: Dave Coleman, Ioan A Sucan, Isaac I.Y. Saito, Michael Stevens, Philippe Capdepuy, Yoan Mollard, corot

0.5.7 (2014-07-05)
------------------
* Merge pull request `#21 <https://github.com/ros-planning/moveit_commander/issues/21>` from pirobot/hydro-devel
  Added set_support_surface_name function to move_group.py
* Added set_support_surface_name function to move_group.py
* Contributors: Patrick Goebel, Sachin Chitta

0.5.6 (2014-03-24)
------------------
* Added the calls necessary to manage path constraints. 
* fix joint and link acces on __getattr__  when trying to acces a joint and its paramaters throught
* Contributors: Acorn, Emili Boronat, Sachin Chitta

0.5.5 (2014-02-27)
------------------
* adding get for active joints
* Contributors: Acorn, Sachin Chitta

0.5.4 (2014-02-06)
------------------

* Install moveit_commander_cmdline.py into package specific directory, not to global bin.
* Fix typos in comments

0.5.3 (2014-01-03)
------------------
* work around name bug
  move group interface python programs cannot be launched from launch files if
  the __name:= argument is used.  This works around the problem and allows using
  launch files to launch python moveit programs.
* Added Travis Continuous Integration

0.5.2 (2013-09-23)
------------------
* add support for setting joint targets from approximate IK
* no longer depend on manipulation_msgs
* expand functionality of MoveGroupInterface

0.5.1 (2013-08-13)
------------------
* make pick() more general
* use msg serialization
* use new attach / detach operations
* fix header for demo code
* Duration class bug fixed in commander conversion.

0.5.0 (2013-07-18)
------------------
* move msgs to common_msgs
* fixed ground command
