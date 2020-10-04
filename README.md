# vandy-hacks-2020

Group Members: Nilai, Carly, Shiv, Jack

Brainstorming:
- GAN to make vid chat higher quality
- AR in vid chat with retro-themed popups
- make vid chat less boring
- reminders to move around
- eye tracking to see if you are paying attention

Inspiration:
- [avatarify](https://github.com/alievk/avatarify)
  - make a virtual camera to interface with Zoom

## Product Description
 - Marketing:
   - marketed as retro-zoom
   - marketed as an extension to zoom, but really its 3rd party application
   - "An interactive Zoom tool that promotes engagement and prevents Zoom fatigue"
 - Features:
   - self monitor for productiveness (Carly - retro filter, coin update in coin grab game)
      - mario pipeline fills when you pay attention and are happy
      - get coins each time pipeline is complete
      - displayed through zoom camera
      - reports send to db and displayed in ui
   - popups (Shiv/Nilai - data analytics - stacked hist, seeing group emotion over time)
      - prompted by long periods of high sad, low joy emotions (tracked in bg, not notified, presented in summary)
      - prompted by eye tracker sensing long periods of wandering (difficult to implement, perhaps not accurate indicator of productivity)
      - prompted by time limit set to daily value (store value in file to track time during day, sound or popup)
   - games (Nilai - object find - what labels? game logic implementation) (Jack - asteroid game - then data analytics w shiv)
      - coin collect
        - move your head around to collect bags of coins. 
        - coins explode in cool gravity fashion when collected
      - object find
        - prompt you to find an object, must present it to the camera
        - apple, banana, tv remote, phone, can, etc. 
        - coin animation for getting an item correct
      - flappy bird
        - flappy bird but your head/nose is the bird and you have to move your head to direct it
        - count obstacles gone through
      - astroid dodge
        - dodge the astroids coming from offscreen with head

## Getting Started:

First, install the following dependencies (you will need Python 3.8):

- [OBS Studio](https://obsproject.com/download)
- [OBS Studio Virtual Camera Plug-in](https://obsproject.com/forum/resources/obs-virtualcam.949/)
- [Python Libraries](requirements.txt) - These can be installed by running `pip install -r requirements.txt` in the
 command line
    - [`pyvirtualcam` python library](https://github.com/letmaik/pyvirtualcam)
    - numpy
    - open cv 

Instructions:
1. Set up a virtual camera in OBS Studio
2. Close OBS Studio
3. Run the Python code (`python control.py` in the command line)
4. Start a Zoom meeting
5. Select OBS as your camera
6. You should see yourself, distorted and with a delay...
