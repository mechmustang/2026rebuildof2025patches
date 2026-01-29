# 2026rebuildof2025patches
Zip files of versions can be found at the google folder: https://drive.google.com/file/d/1XCEm8a74K_W4b87cwHWCmf_2W0Et0Gkm/view?usp=drive_link

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

