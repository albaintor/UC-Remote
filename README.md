#  U Remote Control

<a href="https://apps.apple.com/us/app/u-remote-control/id6740058993"><img width="60" height="60" src="https://is1-ssl.mzstatic.com/image/thumb/Purple211/v4/bf/da/6d/bfda6d6f-7401-dda6-d8ca-c1f0b60f196c/AppIcon-0-0-1x_U007epad-0-1-85-220.png/248x248bb.webp"/></a> Unofficial Unfolded Circle Remote iOS app

[Download from App Store](https://apps.apple.com/us/app/u-remote-control/id6740058993)

## Important Note

I am not affiliated to Unfolded Circle company, this application is provided as is with limited support.
So do not contact Unfolded Circle if you need support, go through the support page of this project https://github.com/albaintor/UC-Remote/issues

You may install it and use it at your own risks. 
The app won't make any modifications to the remotes except the registration entry which is generated and stored in the remote.

## Introduction

iOS, iPadOS application to control Unfolded Circle Remote 2 & 3
To use this application, you need to own an Unfolded Circle Remote 2 or 3
<p align="center">
<img width="200" alt="Profile view" src="https://github.com/user-attachments/assets/9c25417b-7394-49cb-89e3-69bc08cb1ccb" />&nbsp;&nbsp;
<img width="200" alt="Profile view 2" src="https://github.com/user-attachments/assets/8836e8ba-f044-42a5-854a-9a3c37dd0091" />
</p>

# Features

- Registration : remotes registration with automatic discovery (or else manual registration)
- Multiple remotes support with easy switching from the left side menu, and synchronized in background
- Dark mode (default) / light mode / sync with system
- iPhone, iPad & MacOS (Catalyst) support with landscape mode
- Navigation by profile like in the remote. Another profile can be selected from the 3 dots upper right button
- Profile pages : pull down to refresh the data (in case of disconnection or modifications on the remote)
- Profile pages, activities, entities : pull down to refresh will also wake up the remote (if wake on lan setting is enabled in the remote wifi settings)
- Profile pages : swipe left/right to switch between profile pages
- Profile pages : tap on entity icon for toggling lights, switch, climates, covers
- Profile pages : sliders for lights, covers and climate to change brightness/position/temperature. Tap on the slider to open popups and access additional settings of those entities
- Activities, remote & media player entities : full ui pages & buttons support, including short press/long press, media players with artwork, media position, titles/album/artist display, volume control and seeking. All depending on the supported features of the player
- Activities, remotes & media players : support for physical volume buttons to change volume of activity or remote entity
- Activities, remotes & media players : touchpad available for direction pad assignments and handle of velocity (larger gestures trigger faster repeated commands)
- Activities : active (running) activities are also directly accessible from side menu in addition of profiles pages
- Activities : on interface pages, when long pressing an item which corresponds to a light, a cover or a climate, a popup is opened with additional settings. Otherwise the command is executed
- Media players : updated in realtime (artwork, title, position...), seek video with the scrubber
- Localization based on remote settings (English, French, German & Dutch configured at this state)
- Widget : available in 3 sizes, lets control the running activities and display its state if available (artwork, title, album, artist) with the following buttons : play/pause, volume up/down, mute, rewind/forward and refresh button to update. If several activities are active, the first one found will be taken unless you select the activity from the app and minimize it (the widget will be reloaded then with the selected activity).
- Widtet : a toggle button switches to a page of entities, configurable from the app. Each entities are togglable, except sensors that display the sensor value.
- Live activities : live activites are like widgets but activated by the app when entering into an activity page, and remain accessible from the dynamic island or the lock screen. The same commands are available
- Diagnostics : access to app logs as well as extraction of remote logs by category

## Limitations and future plans

- Activity widget : the widget cannot take benefits of websocket notifications from the remote. Only network polling through REST APIs is allowed, but this will drain battery a little bit more, so the updates can be done manually through the refresh button (otherwise they are performed automatically when using the app and minimize it)
- Live activities : disabled by default, can be enabled from settings. Limitation: the app when minimized will loose its network connections, so the live activity can't be updated after a while and the status will become out of sync. However a refresh button will update the media state

# Support

If you have issues you can post a support ticket here https://github.com/albaintor/UC-Remote/issues but first be sure that it has not already been reported.

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
- Refresh pages on pull (added/removed or renamed entities for ex)

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

On interface pages, when long pressing an item which corresponds to a light, a cover or a climate, a popup is opened with additional settings. Otherwise the command is executed
<p align="center"> 
 <img width="250" alt="image" src="https://github.com/user-attachments/assets/a82b06df-2b2b-4681-ae71-625d06797f5d"/>
</p>


As soon as activities are on, they are also accessible directly from the side left menu
<p align="center"> 
 <img width="250" alt="image" src="https://github.com/user-attachments/assets/d0f3b698-3644-4a8f-b90d-64f723343721"/>
</p>


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


# Widgets & Live Activities

3 sizes are available for widgets

## Large size
<p align="center"> 
<img width="275" alt="image" src="https://github.com/user-attachments/assets/e0aa11d3-b661-45b5-91ca-ef5655f38feb" />
</p>

## Medium size
<p align="center"> 
<img width="275" alt="image" src="https://github.com/user-attachments/assets/77f2cab1-dbcb-450c-8a51-4be08eee4aa3" />
</p>

## Small size
<p align="center"> 
<img width="131" alt="image" src="https://github.com/user-attachments/assets/86d7f704-7dd6-486f-ab96-43227c5f31b5" />
</p>

## Entities page

<p align="center"> 
<img width="269" alt="image" src="https://github.com/user-attachments/assets/4e2e5ea5-06da-4b5c-b3e7-46b1b7036cf8" />
</p>

The widgets have a toggle button that can switch to a page of entities. This button is hidden if no entities have been configured from the app.
Each entity will display its state depending on its nature : brightness for lights, position for shutters/covers, on/off state for activities...
A tap on an entity will toggle it : switch on/off lights, turn on/off an activity, open/close covers...
Except sensors that just display information

### Configuration of entities page

Open side menu > Settings : scroll down to the widget section and select the remote to be configured.
Then you can search and add or remove entities to the widget page from there. You can also reorder the list

<p align="center"> 
<img width="300" alt="image" src="https://github.com/user-attachments/assets/a2b94b2f-61a0-4761-8245-cedf609d4547" />
</p>



