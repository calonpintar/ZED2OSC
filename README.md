# ZED2OSC
ZED Camera Position &amp; Rotation to OSC

-July 2020-
Visual Studio Community 2019 project file.
Need Zed SDK 3.2.0 installed.

Default OSC send is "192.168.5.145" port 7000, OSC address /zed2osc in case you want to try ZED_Positional_Tracking.exe,
don't forget to hook Zed Camera. 
OSC sends message in pattern fffddds -> float, float, float, decimal, decimal, decimal, string -> posX, posY, posZ, rotX, rotY, rotZ, "zed2osc"
