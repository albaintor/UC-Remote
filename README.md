# U Remote

Unofficial Unfolded Circle Remote app

## Important Note

I am not affiliated to Unfolded Circle company, this application is provided as is with limited support.
So do not contact Unfolded Circle if you need support, go through the support page of this project https://github.com/albaintor/UC-Remote/issues

You may install it and use it at your own risks. 
The app won't make any modifications to the remotes except the registration key which is stored in the remote.

## Introduction

iOS, iPadOS application to control Unfolded Circle Remote 2 & 3
To use this application, you need to own an Unfolded Circle Remote 2 or 3
<p align="center">
<img width="200" alt="Profile view" src="https://github.com/user-attachments/assets/9c25417b-7394-49cb-89e3-69bc08cb1ccb" />&nbsp;&nbsp;
<img width="200" alt="Profile view 2" src="https://github.com/user-attachments/assets/8836e8ba-f044-42a5-854a-9a3c37dd0091" />
</p>

# Features

- Registration : remotes registration with automatic discovery (or else manual registration)
- Multiple remotes support with easy switching from the side menu
- Dark mode (default) / light mode
- iPhone and iPad support with landscape mode
- Navigation by profile like in the remote. Another profile can be selected from the 3 dots upper right button
- Profile pages : pull down to refresh the data (in case of disconnection or modifications on the remote)
- Profile pages : Pull to refresh will also wake on the remote if wake on lan setting is enabled on the remote
- Profile pages : swipe left/right to switch between profile pages
- Profile pages : tap on entity icon for toggling lights, switch, climates, covers
- Profile pages : sliders for lights and climate to change brightness or temperature. Tap on the slider to open popups and access additional settings for entities
- Activities : full ui pages & buttons support, including short press/long press, media players with artwork, media position, titles/album/artist display, volume control
- Activities : support for physical volume buttons to change volume of activity
- Media players : updated in realtime (artwork, title, position...), seek video with the scrubber (if supported by media player)

Not supported yet (planned):
- Sensor entities, shutter advanced settings, climate modes
- Media player on lock screen (experimental support, to be improved)

# Setup

1. Just download the app from the App store
2. Tap on the upper left icon to register a new remote : if your remote is connected (not in standby) it will be discovered automatically, otherwise tap the + icon and fill in its IP, and pin code for registration. Additional remotes can be registered. After the first registration, somes common resources will be downloaded (fonts)
3. Go into the selected remote : the default profile will be loaded. It is possible to select another profile by tapping on the 3 dots icon. It is recommended to tap on "Load resources" to download all icons and backgrounds locally for better experience

In the screenshot one remote is registered whereas another one has been discovered and can be registered :
<p align="center">
<img width="250" alt="image" src="https://github.com/user-attachments/assets/c9b9a921-b68a-4439-b0d1-40be81d9fc32" />
</p>

# Usage

The remote needs to be connected on the network. You can wake it up with a pull down gesture in the profile pages : this will work only if you enabled this setting on the remote. See capture below : 
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
- Sliders on lights and climates to adjust brightness and temperature. Tap on slider to access additional settings.
- Open activivities

## Activities

When you enter in activities, you have 2 tabs in bottom : one for the user interface, another one for the remote buttons.
Note : you can change this layout from global settings to have a unique scrolling view instead of 2 tabs.

If your activity holds media players, they will be rendered as on the remote. The seeking bar is dynamic if the media entity supports seeking.
Also the physical volume buttons are assigned to the volume commands of the activity.

<p align="center"> 
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/f5d5436c-417a-4e97-9d00-0c94d8751c24"/>&nbsp;&nbsp; 
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/0beed574-0c4a-404f-8387-ce66e73b0e72"/>&nbsp;&nbsp;
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/cb2d7789-1801-4537-b219-094fd35f08ba"/>
</p>


# Side menu

The side menu is accessible from the upper left 3 bars icon.
From this menu you can :
1. Register (or remove) remotes
2. Select a registered remote to navigate in it
3. Global settings

<p align="center"> 
  <img width="250" alt="image" src="https://github.com/user-attachments/assets/2730a79a-3276-4a87-9a98-d4de65c205f7"/>
</p>


