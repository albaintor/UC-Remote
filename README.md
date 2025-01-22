# U Remote

Unofficial Unfolded Circle Remote app

## Important Note

I am not affiliated to Unfolded Circle company, this application is provided as is with limited support.
So do not contact Unfolded Circle if you need support, go through the support page of this project https://github.com/albaintor/UC-Remote/issues

You may install it and use it at your own risks. 
The app won't make any modifications to the remotes except the registration key which is generated and stored in the remote.

## Introduction

iOS, iPadOS application to control Unfolded Circle Remote 2 & 3
To use this application, you need to own an Unfolded Circle Remote 2 or 3
<p align="center">
<img width="200" alt="Profile view" src="https://github.com/user-attachments/assets/9c25417b-7394-49cb-89e3-69bc08cb1ccb" />&nbsp;&nbsp;
<img width="200" alt="Profile view 2" src="https://github.com/user-attachments/assets/8836e8ba-f044-42a5-854a-9a3c37dd0091" />
</p>

# Features

- Registration : remotes registration with automatic discovery (or else manual registration)
- Multiple remotes support with easy switching from the side menu, and synchronized in parallel
- Dark mode (default) / light mode
- iPhone and iPad support with landscape mode
- Navigation by profile like in the remote. Another profile can be selected from the 3 dots upper right button
- Profile pages : pull down to refresh the data (in case of disconnection or modifications on the remote)
- Profile pages : pull down to refresh will also wake up the remote (if wake on lan setting is enabled in the remote wifi settings)
- Profile pages : swipe left/right to switch between profile pages
- Profile pages : tap on entity icon for toggling lights, switch, climates, covers
- Profile pages : sliders for lights, covers and climate to change brightness/position/temperature. Tap on the slider to open popups and access additional settings of those entities
- Activities & remote entities : full ui pages & buttons support, including short press/long press, media players with artwork, media position, titles/album/artist display, volume control and seeking. All depending on the supported features of the player
- Activities & remotes : support for physical volume buttons to change volume of activity or remote entity
- Activities & remotes : touchpad available for direction pad assignments and handle of velocity (larger gestures trigger faster repeated commands)
- Activities : active activities are also accessible from side menu in addition of profiles pages
- Media players : updated in realtime (artwork, title, position...), seek video with the scrubber
- Localization based on remote settings (only English and French configured at this state)

## Limitations and future plans

- Sensor entities : not supported yet
- Media player widget : experimental support, disabled in the current release. The widget cannot take benefits of websocket notifications from the remote. Only network polling through REST APIs is allowed, but this will drain battery a little bit more. The goal is to provide a media player widget with current artwork, title, progress and a few buttons (pause, previous, next...)
- Live activities (different from widget) : experimental support for now (disabled by default, can be enabled from settings). Limitations: the app when minimized will loose its network connections, so the live activity can't be updated after a while even if tricks are possible (the progress time bar can move forward in the meantime without receiving updates). These limitations don't apply to the widget above

# Setup

1. Just download the app from the App store
2. Tap on the upper left icon to register a new remote : if your remote is connected (not in standby) it will be discovered automatically, otherwise tap the + icon and fill in its IP, and pin code for registration. Additional remotes can be registered. After the first registration, some common resources will be downloaded for later usage and only once (fonts)
3. Go into the selected remote : the default profile will be loaded. It is possible to select another profile by tapping on the 3 dots icon. It is recommended to tap on "Load resources" to download all icons and backgrounds locally for faster experience (otherwise pictures are downloaded on the fly each time)

In the screenshot one remote is registered whereas another one has been discovered and can be registered :
<p align="center">
<img width="250" alt="image" src="https://github.com/user-attachments/assets/c9b9a921-b68a-4439-b0d1-40be81d9fc32" />
</p>

# Usage

The remote needs to be connected on the network. You can wake it up with a pull down gesture in the profile pages : this will work only if you enabled this feature in the wifi setting of the remote. See capture below : 
<p align="center">
<img width="250" alt="image" src="https://github.com/user-attachments/assets/b43a4073-a755-46ba-925d-34fe796610cd" />
</p>

As soon as a remote is configured, the app will open directly in the last selected remote.
The first profile found is loaded. You can select another profile by tapping on the 3 dots button in the upper right which will raise a popup.
<p align="center"> 
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/b248fd66-a2fd-4b73-9590-afca66e7e7c6" />
</p>

In this popup you can also (re)load resources : background images, icons & fonts.

In profile pages, you can :
- Swipe profile pages from left to right
- Toggle entities : lights, climates, covers, switches
- Toggle profile groups, expand them to show its entities
- Sliders on lights, covers, climates to adjust brightness/position/temperature. Tap on slider to access additional settings.
- Open activivities, remotes and media player entities

## Activities

Same interface and behaviour if you open a remote entity or a media player entity

When you enter in activities, you have 2 tabs in bottom : one for the user interface, another one for the remote buttons.
Note : you can change this layout from global settings to have a unique scrolling view instead of 2 tabs.

If your activity holds media players, they will be rendered as on the remote. The seeking bar is dynamic if the media entity supports seeking.
Also the physical volume buttons are assigned to the volume commands of the activity.

<p align="center"> 
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/f5d5436c-417a-4e97-9d00-0c94d8751c24"/>&nbsp;&nbsp; 
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/0beed574-0c4a-404f-8387-ce66e73b0e72"/>&nbsp;&nbsp;
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/cb2d7789-1801-4537-b219-094fd35f08ba"/>
</p>

As soon as activities are on, they are also accessible directly from the side left menu

# Side menu

The side menu is accessible from the upper left 3 bars icon.
From this menu you can access to :
1. Register (or remove) remotes
2. Select a registered remote to navigate in it
3. Global settings
4. Active activities (on all configured remotes in one place)

<p align="center"> 
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/2730a79a-3276-4a87-9a98-d4de65c205f7"/>
</p>


