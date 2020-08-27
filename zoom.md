# OBS Setup for Recording Zoom Meetings

## Overview

Written by fuyubear#0765 from Discord.

You are ultimately responsible for using this for good (not for bad) purposes.

This setup allows you to record Zoom meetings without showing your other monitor contents or recording your Discord (or other VoIP) calls and other irrelevant stuff on your PC. Gives comparable file sizes to Zoom's recordings (120-180 MB per 75-80 minutes).

Tested with OBS 25.0.8, GTX 1070 Ti (Driver 452.06), Zoom 5.2.1 (44052.0816), and Windows 10 2004.

The zoom720p10fps folder is the profile loaded into OBS, while the zoom720p10fpsscenes.json file is for the scenes.

**Note: the Output -> Streaming settings are tweaked for Nvidia GPUs only. If you use QuickSync, AMF, or CPU (x264) encoding, you may need to use different Output -> Streaming settings to maintain visual fidelity.**

**Needs more verification: OBS source capturing (capturing the Zoom window) may break whenever you are sent in/out to/from a separate breakout room by the Host. When this happens, restart OBS.**

## Setup

1. Extract the zip package somewhere accessible on your PC.

2. Install VoiceMeeter, then restart your PC.

3. Open VoiceMeeter.

4. Any hardware inputs in VoiceMeeter should be muted.

5. In VoiceMeeter, click on A1 and select your default Audio Out (the speakers you use) device. Generally, the A devices manage the output audio device(s) of whatever gets inputted into VoiceMeeter.

6. Open Zoom, then click the gear on the top right.

7. Go to General (on left bar) and uncheck "Enter full screen automatically when starting or joining the meeting". **Leaving this box checked breaks the OBS video source capturing anytime you start or join a Zoom meeting.**

8. Go to Audio (on left bar) and change the Speaker to VoiceMeeter Input.

9. Go to Share Screen (on left bar) and uncheck the "Enter full screen when a participant shares screen" box. **Leaving this box checked breaks the OBS video source capturing anytime a participant starts sharing their screen.**

10. Test the Speaker to make sure you can hear the Zoom audio test. Stop here and get help from somewhere if you can't hear it.

11. Install and open OBS.

12. In OBS, go to Profile -> Import and select the zoom720p10fps folder.

13. In OBS, go to Scene Collection -> Import, click the "..." in the first row of the popup window, and select the zoom720p10fpsscenes.json file, then click Import. The Scenes and Sources should be loaded.

14. (Optional, for the purpose of video censoring) In OBS, right click on the Image source under Sources, go to Properties, and change the Image Source to the provided black.jpg image. You may want to Copy and Duplicate these Image sources for more censoring coverage.

15. In OBS, change the devices under Settings -> Audio -> Devices, or use the cogs next to the Desktop Audio and Mic/Aux areas in the Audio Mixer. The Desktop Audio device should be your VoiceMeeter Input device, while your Mic/Aux device should be your mic.

16. Click on the "speaker with waves" icon associated with the Mic/Aux area to turn off your mic. During recording, click on the "speaker with red x" icon whenever you want to turn on your mic (like when you speak in Zoom), and click it again to turn your mic off. It may be beneficial to have a Hotkey (in Settings) set to quickly unmute your mic on OBS matching your hotkey for unmuting yourself on Zoom.

17. Make other Setting tweaks in OBS as needed. See [Setting Values](#setting-values) for more.

18. It's time to test your setup. Create a new Meeting for yourself, and start the recording. You should be able to see your meeting window in the OBS preview area. If not, change the Window Capture source to match your meeting window. After doing this, OBS should automatically capture the window whenever you go to future meetings. Also, whenever you go into meetings, be sure to adjust the size of the window capture by clicking on the Zoom window in the OBS preview area, and use the red boxes to resize the Zoom window to fill the screen. You may need to resize your Zoom window and click Participants/Chat (if you want to record them) to fill the OBS preview area (and thus, the video recording) with the Zoom Window. Use the Image scenes (duplicate if needed) to cover up webcam content to save bitrate and privacy, as needed. **This whole process may need to be done every time you join a Zoom meeting, especially if you want to record Participants/Chat contents.**

19. Stop the test recording when you are done. The recording should be located in the Recording Path set in Output -> Recording settings.

20. You should be good to go! Whenever you are ready to join the Zoom meeting, open VoiceMeeter, OBS, and Zoom; join the Zoom meeting; make Zoom window adjustments (see step 18); and then start/stop the recording as needed. Monitor the OBS window to make sure the recording works, especially when entering/exiting breakout rooms, to restart OBS and the recording as needed.

## Setting Values

Here is a listing of key Setting values within the profile. You must change the devices under Settings -> Audio -> Devices, or use the cogs next to the Desktop Audio and Mic/Aux areas in the Audio Mixer. You may need to adjust all of the Output -> Streaming settings if you don't have a Nvidia GPU. The VBR ranges and FPS can be increased if your Zoom meeting has more movement (check Zoom diagnostic details in settings to verify if more FPS/bitrate is needed).

- Output -> Streaming settings:
  
  - Encoder: NVIDIA NVENC H.264 (new)
  
  - VBR (Variable BitRate) range: 250-750 kbps
  
  - Keyframe Interval: auto
  
  - Preset: Quality
  
  - Profile: High
  
  - Look-ahead: On
  
  - Psycho Visual Tuning: On
  
  - Max B-frames: 4

- Output -> Recording settings:
  
  - Type: Standard
  
  - Recording Path: C:\
  
  - Recording Format: mkv
  
  - Audio Track: (check next to 1, leave others unchecked)
  
  - Encoder: Use stream encoder

- Output -> Audio settings:
  
  - Track 1 -> Audio Bitrate: 128 kbps

- Audio -> General:
  
  - Sample Rate: 44.1 kHz
  
  - Channels: Stereo

- Audio -> Devices:
  
  - [MUST CHANGE] Desktop Audio: Your VoiceMeeter Input device
  
  - [MUST CHANGE] Mic/Aux Audio: Your mic device

- Audio -> Advanced:
  
  - Monitoring Device: Default
  
  - Disable Windows audio ducking: On

- Video:
  
  - Base (Canvas) Resolution: 1280x720
  
  - Output (Scaled) Resolution: 1280x720
  
  - Downscale Filter: Bicubic
  
  - Common FPS Values: 10
