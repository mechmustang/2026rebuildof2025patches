# 2026rebuildof2025patches
Zip files of versions can be found at the google folder: https://drive.google.com/drive/folders/1MqZtYkAMpWvMVDTFV1RIQeQm0cM1hu0n?usp=drive_link

1-31-2026 Uploaded by Roer from Roer's Orange Laptop
  Roer added images to Advantagescope telling where the robot thinks it is,
    and where each camera thinks it is on the field
  Roer added a button to press to jump to where the camera thinks it is
  Roer added to Vision to calculate trust values (standard deviations) for Apriltag detections
  Roer added a RobotState class to handle changes in state (DEBUG, PREMATCH, PIT, TELEOP, etc)
  ISSUE: PoseEstimation is not entirely accurate -- I think the gyroscope is resetting at the wrong times
  TODO: Correct pose PoseEstimation/Gyroscoping
  TODO: Tune the trustvalues so that camera data adjusts pose more quickly.
  TODO: Fix logging / Epilogue so that data is sent to Network Tables more efficiently and get rid of smartdashboard lines (not allowed in 2027)


Version 1-29-26 Uploaded by Roer and Hirt from Bangma's laptop #45
   USed 1-27-26 as a base and we temporailty turned off logging because it was crashing by logging too much information
   added a VisionandLights subsystem which was able to see april tags and add vision measurements to the drive subystem
     which updated our pose (position and orientation) which we could see in AdvantageScope.
   issues to fix next time...
     rotation is incorrect - seems VERY fast -- maybe a radians/degrees issue?
     how accurate are our poses?  haven't really investigated
   desired additions:
     want to add lights using blinkin to the visionandlights subsystem
     want to create a button that autoaims...

Version 1-27-26 Uploaded by Roer from Roer's Orange laptop
   Significant amount of changes -- rewritten to post everything to Network Tables by way of Epilogue and @Logged lines
   Eliminated most of the old subsystems
   No vision code at this time -- It wasn't really working in the 1-23 version anyway.
   THIS VERSION CRASHES QUICKLY BECAUSE WE'RE LOGGING TOO MUCH INFO... 

Version 1-23-26 - Uploaded by Roer from Bangma's laptop #45. 
  Initial import of patches code from last year into wpilib 2026. 
  Some attempts at creating a vision subsystem utilizing our limelights exist, but they are a mess and need to be deleted and started over.
  We ran into issues with limelights not talking to code, but ultimately found the problem was in a poorly assigned ip address.

