# Enmity Theme Color Map
Created by: NEO#7154

If you want to contribute, please check the "Unknowns" section and see if you can find any of the properties.
- - - -

- [Enmity Theme Color Map](#enmity-theme-color-map)
  - [**Details**](#details)
  - [**Format**](#format)
  - [**"theme_color_map" object**](#theme_color_map-object)
      - [Background Properties](#background-properties)
      - [Text Colors](#text-colors)
  - [**"colors" object**](#colors-object)
      - [Colors used throughout Discord](#colors-used-throughout-discord)
  - [**"unsafe_colors" object**](#unsafe_colors-object)
      - [Used to theme the annoying grey bottom bar (homebar area)](#used-to-theme-the-annoying-grey-bottom-bar-homebar-area)
  - [**Unknowns**](#unknowns)
      - [**Long** ass list of unknown properties.](#long-ass-list-of-unknown-properties)
      - [**"theme_color_map" object unknown**](#theme_color_map-object-unknown)
      - [**"colors" object unknown**](#colors-object-unknown)

## **Details**
* This a _semi-organized_ and _incomplete_ list of the iOS Discord Theme Color Map.

* Many Properties __overlap__ each other. Some compromises have to be made when themeing.

## **Format**
> [Check the example template here](example.json)
```json 
"theme_color_map": {
    "BACKGROUND_PRIMARY": ["#000000", "#FFFFFF"],
                         //Dark Mode , //Light Mode
},
"colours": {
    "PRIMARY_DARK": "#0F0FFF",
 },
"unsafe_colors": {
    "CHAT_GREY": "#000000"
}
```
- - - -

## **"theme_color_map" object**
[Back to Top](#)
#### Background Properties
> Properties that theme most background elements

| Property | Description |
| --------------- | :---------------: |
| KEYBOARD | Color to theme keyboard in an upcoming Enmity update |
| BACKGROUND_PRIMARY | Background (Search, Mentions, Channel, Channel Info, Invite UI, Set Status, User List, Threads, Notifications, Behind the keyboard *looks sick yo*) |
| BACKGROUND_SECONDARY | Profile background, Server info background, Slash Command Top bar, Button Backgrounds (Server List, Reactions), Embed Background, Code Blocks, Call background in chat |
| BACKGROUND_SECONDARY_ALT | Profile Notes background, About Me background, Embed Background, Reactions Background, Message Input Background, Missed Call/etc |
| BACKGROUND_TERTIARY | Background background BACKGROUND (server list and around things), Search bar background, spoilers, Top bar seperator, About me and Notes outline, three dots button |
| BACKGROUND_ACCENT | Reply Pipe, Album Buttons, Thread Buttons, Flashes this color when some stuff loads |
| BACKGROUND_FLOATING | Profile background, Server Boost Page Icons |
| BACKGROUND_NESTED_FLOATING | Settings buttons/boxes background |
| BACKGROUND_MOBILE_PRIMARY | Account/Settings background |
| BACKGROUND_MOBILE_SECONDARY | Channel List/DM Background, Header App Wide |
| BACKGROUND_MODIFIER_ACCENT | Seperators (Server List Top, Bottom Bar, User List, Notifications, Friends, Search, Settings) |
| BACKGROUND_MODIFIER_ACTIVE | When holding/clicking on a button |
| BACKGROUND_MODIFIER_SELECTED | Selected Channel/User background |
| CHANNELS_DEFAULT | Category titles, User list names |
| HEADER_PRIMARY | Top Bar (Server Name, Channel Name, User Name, Follow channel text, Invite members text, Profile Name text, slash command text, mention channel name text, Pop up text [add theme]) |
| HEADER_SECONDARY | Some titles, Most subtitles (channel info, user now playing, etc), Profile #'s, Settings titles |
| INTERACTIVE_ACTIVE | Active bottom bar icon fill, Selected server bar, Selected channel text, some title text |
| INTERACTIVE_MUTED | Unselected muted channel text, block quote bar |
| INTERACTIVE_NORMAL | Button/glyph Accent colors (Top bar, Server Settings, Channel Settings, Member list roles, User settings, input bar, chevrons), Bottom bar inactive color fill, incoming typing member text |
| ACTIVITY_CARD_BACKGROUND | New Messages Seperator (always red?) |
| TEXTBOX_MARKDOWN_SYNTAX | Markdown text background? |

#### Text Colors
> Properties that theme most text colors

| Property | Description |
| --------------- | :---------------: |
| TEXT_DANGER | Enmity Uninstall text |
| TEXT_LINK | Link text global |
| TEXT_MUTED | Search bar text, Timestamp text, Input box text, Symbols (@, lock, # [except muted channels]), bunch of settings subtitles |
| TEXT_NORMAL | Text color like everywhere |

## **"colors" object**
[Back to Top](#)
#### Colors used throughout Discord
> Some Properties overlap with the color map.

| Property | Description |
| --------------- | :---------------: |
| PRIMARY_DARK | Popup seperators?, Profile notes text |
| PRIMARY_DARK_100 | Popup Header? Text (Enmity Apply), Search/Type Cursor color |
| PRIMARY_DARK_300 | Grabber Color, ? Glyph Color, No Pinned messages text, Channel Settings channel name, Connections text |
| PRIMARY_DARK_360 | Unselected, Unmuted, Read Channel Name text |
| PRIMARY_DARK_400 | Different Day Message seperator, Search tab subtext, 2FA text, 'New Unreads' banner |
| PRIMARY_DARK_500 | Invite Button background, User Watch Live button, Default (grey) Role circle color, "Public" server button |
| PRIMARY_DARK_600 | Chat Input Border Background fill, Global? pop up background |
| PRIMARY_DARK_630 | Hold/Click on message background, Slash Command background, Search in Channel background, Spotify Now playing scrubber bar |
| PRIMARY_DARK_700 | Role Background color, Top and Bottom Bar Seperators, Global Toast background, Side of screen flashes this color when moving to new pages ??? |
| PRIMARY_DARK_800 | The Entire Bottom bar (and homebar) [Discord Icon, People Icon, Profile, etc.], Tints GIF categories in search |
| BRAND_NEW | Direct Message Button background (top left), New Message Top Baner, Floating New Banner progress bar, Global Switcher Color, Send Button |
| BRAND_NEW_360 | Random Nitro stuff. Who cares |
| WHITE | Global Cursor, DMs username text, Add Files button colors, GIF text, Send button glyph, Server Name and 3 dots text, Invite Text, Role Text color, Video/Picture controls, Channel Search text |
| STATUS_RED/GREEN/YELLOW/GREY/ORANGE 100-900 | Various colored elements like logout text, security text. Pain in the ass. good luck |

## **"unsafe_colors" object**
[Back to Top](#)
#### Used to theme the annoying grey bottom bar (homebar area)

| Property | Description |
| --------------- | :---------------: |
| CHAT_GREY | cmon man. you know... the thing |

## **Unknowns**
[Back to Top](#)
#### **Long** ass list of unknown properties. 
> Some of these just don't do anything, or I couldn't find what they changed.
>> If you can figure these out, let me know


<details>
  <summary>Expand Me!</summary>
  
  #### **"theme_color_map" object unknown**
| Property | Description |
| --------------- | :---------------: |
| TEXT_LINK_LOW_SATURATION | ??? |
| TEXT_POSITIVE | ??? |
| TEXT_WARNING | ??? |
| INTERACTIVE_HOVER | ??? |
| BACKGROUND_MODIFIER_HOVER | ??? |
| INFO_POSITIVE_BACKGROUND | ??? |
| INFO_POSITIVE_FOREGROUND | ??? |
| INFO_POSITIVE_TEXT | ??? |
| INFO_WARNING_BACKGROUND | ??? |
| INFO_WARNING_FOREGROUND | ??? |
| INFO_WARNING_TEXT | ??? |
| INFO_DANGER_BACKGROUND | ??? |
| INFO_DANGER_FOREGROUND | ??? |
| INFO_DANGER_TEXT | ??? |
| INFO_HELP_BACKGROUND | ??? |
| INFO_HELP_FOREGROUND | ??? |
| INFO_HELP_TEXT | ??? |
| STATUS_POSITIVE_BACKGROUND | ??? |
| STATUS_POSITIVE_TEXT | ??? |
| STATUS_WARNING_BACKGROUND | ??? |
| STATUS_WARNING_TEXT | ??? |
| STATUS_DANGER_BACKGROUND | ??? |
| STATUS_DANGER_TEXT | ??? |
| SCROLLBAR_THIN_THUMB | ??? |
| SCROLLBAR_THIN_TRACK | ??? |
| SCROLLBAR_AUTO_THUMB | ??? |
| SCROLLBAR_AUTO_TRACK | ??? |
| SCROLLBAR_AUTO_SCROLLBAR_COLOR_THUMB | ??? |
| SCROLLBAR_AUTO_SCROLLBAR_COLOR_TRACK | ??? |
| ELEVATION_STROKE | ??? |
| ELEVATION_LOW | ??? |
| ELEVATION_MEDIUM | ??? |
| ELEVATION_HIGH | ??? |
| LOGO_PRIMARY | ??? |
| FOCUS_PRIMARY | ??? |
| CONTROL_BRAND_FOREGROUND | ??? |
| CONTROL_BRAND_FOREGROUND_NEW | ??? |
| BACKGROUND_MENTIONED | ??? |
| BACKGROUND_MENTIONED_HOVER | ??? |
| BACKGROUND_MESSAGE_HOVER | ??? |
| GUILD_HEADER_TEXT_SHADOW | ??? |
| CHANNELTEXTAREA_BACKGROUND | ??? |
| DEPRECATED_CARD_BG | ??? |
| DEPRECATED_CARD_EDITABLE_BG | ??? |
| DEPRECATED_STORE_BG | ??? |
| DEPRECATED_QUICKSWITCHER_INPUT_BACKGROUND | ??? |
| DEPRECATED_QUICKSWITCHER_INPUT_PLACEHOLDER | ??? |
| DEPRECATED_TEXT_INPUT_BG | ??? |
| DEPRECATED_TEXT_INPUT_BORDER | ??? |
| DEPRECATED_TEXT_INPUT_BORDER_HOVER | ??? |
| DEPRECATED_TEXT_INPUT_BORDER_DISABLED | ??? |
| DEPRECATED_TEXT_INPUT_PREFIX | ??? |

#### **"colors" object unknown**

| Property | Description |
| --------------- | :---------------: |
| PRIMARY_LIGHT_100 | ??? |
| PRIMARY_LIGHT_130 | ??? |
| PRIMARY_LIGHT_160 | ??? |
| PRIMARY_LIGHT_200 | ??? |
| PRIMARY_LIGHT_230 | ??? |
| PRIMARY_LIGHT_260 | ??? |
| PRIMARY_LIGHT_300 | ??? |
| PRIMARY_LIGHT_330 | ??? |
| PRIMARY_LIGHT_360 | ??? |
| PRIMARY_LIGHT_400 | ??? |
| PRIMARY_LIGHT_430 | ??? |
| PRIMARY_LIGHT_460 | ??? |
| PRIMARY_LIGHT_500 | ??? |
| PRIMARY_LIGHT | ??? |
| PRIMARY_LIGHT_530 | ??? |
| PRIMARY_LIGHT_560 | ??? |
| PRIMARY_LIGHT_600 | ??? |
| PRIMARY_LIGHT_630 | ??? |
| PRIMARY_LIGHT_660 | ??? |
| PRIMARY_LIGHT_700 | ??? |
| PRIMARY_LIGHT_730 | ??? |
| PRIMARY_LIGHT_760 | ??? |
| PRIMARY_LIGHT_800 | ??? |
| PRIMARY_LIGHT_830 | ??? |
| PRIMARY_LIGHT_860 | ??? |
| PRIMARY_LIGHT_900 | ??? |
| BRAND_100 | ??? |
| BRAND_130 | ??? |
| BRAND_160 | ??? |
| BRAND_200 | ??? |
| BRAND_230 | ??? |
| BRAND_260 | ??? |
| BRAND_300 | ??? |
| BRAND_330 | ??? |
| BRAND_360 | ??? |
| BRAND_400 | ??? |
| BRAND_430 | ??? |
| BRAND_460 | ??? |
| BRAND_500 | ??? |
| BRAND | ??? |
| BRAND_530 | ??? |
| BRAND_560 | ??? |
| BRAND_600 | ??? |
| BRAND_630 | ??? |
| BRAND_660 | ??? |
| BRAND_700 | ??? |
| BRAND_730 | ??? |
| BRAND_760 | ??? |
| BRAND_800 | ??? |
| BRAND_830 | ??? |
| BRAND_860 | ??? |
| BRAND_900 | ??? |
| BRAND_NEW_100 | ??? |
| BRAND_NEW_130 | ??? |
| BRAND_NEW_160 | ??? |
| BRAND_NEW_200 | ??? |
| BRAND_NEW_230 | ??? |
| BRAND_NEW_260 | ??? |
| BRAND_NEW_300 | ??? |
| BRAND_NEW_330 | ??? |
| BRAND_NEW_360 | ??? |
| BRAND_NEW_400 | ??? |
| BRAND_NEW_430 | ??? |
| BRAND_NEW_460 | ??? |
| BRAND_NEW_500 | ??? |
| BRAND_NEW | ??? |
| BRAND_NEW_530 | ??? |
| BRAND_NEW_560 | ??? |
| BRAND_NEW_600 | ??? |
| BRAND_NEW_630 | ??? |
| BRAND_NEW_660 | ??? |
| BRAND_NEW_700 | ??? |
| BRAND_NEW_730 | ??? |
| BRAND_NEW_760 | ??? |
| BRAND_NEW_800 | ??? |
| BRAND_NEW_830 | ??? |
| BRAND_NEW_860 | ??? |
| BRAND_NEW_900 | ??? |
| FOCUS_PRIMARY_100 | ??? |
| FOCUS_PRIMARY_130 | ??? |
| FOCUS_PRIMARY_160 | ??? |
| FOCUS_PRIMARY_200 | ??? |
| FOCUS_PRIMARY_230 | ??? |
| FOCUS_PRIMARY_260 | ??? |
| FOCUS_PRIMARY_300 | ??? |
| FOCUS_PRIMARY_330 | ??? |
| FOCUS_PRIMARY_360 | ??? |
| FOCUS_PRIMARY_400 | ??? |
| FOCUS_PRIMARY_430 | ??? |
| FOCUS_PRIMARY_460 | ??? |
| FOCUS_PRIMARY_500 | ??? |
| FOCUS_PRIMARY | ??? |
| FOCUS_PRIMARY_530 | ??? |
| FOCUS_PRIMARY_560 | ??? |
| FOCUS_PRIMARY_600 | ??? |
| FOCUS_PRIMARY_630 | ??? |
| FOCUS_PRIMARY_660 | ??? |
| FOCUS_PRIMARY_700 | ??? |
| FOCUS_PRIMARY_730 | ??? |
| FOCUS_PRIMARY_760 | ??? |
| FOCUS_PRIMARY_800 | ??? |
| FOCUS_PRIMARY_830 | ??? |
| FOCUS_PRIMARY_860 | ??? |
| FOCUS_PRIMARY_900 | ??? |
| LINK_100 | ??? |
| LINK_130 | ??? |
| LINK_160 | ??? |
| LINK_200 | ??? |
| LINK_230 | ??? |
| LINK_260 | ??? |
| LINK_300 | ??? |
| LINK_330 | ??? |
| LINK_360 | ??? |
| LINK_400 | ??? |
| LINK_430 | ??? |
| LINK_460 | ??? |
| LINK_500 | ??? |
| LINK | ??? |
| LINK_530 | ??? |
| LINK_560 | ??? |
| LINK_600 | ??? |
| LINK_630 | ??? |
| LINK_660 | ??? |
| LINK_700 | ??? |
| LINK_730 | ??? |
| LINK_760 | ??? |
| LINK_800 | ??? |
| LINK_830 | ??? |
| LINK_860 | ??? |
| LINK_900 | ??? |
| LINK_LOW_SATURATION_100 | ??? |
| LINK_LOW_SATURATION_130 | ??? |
| LINK_LOW_SATURATION_160 | ??? |
| LINK_LOW_SATURATION_200 | ??? |
| LINK_LOW_SATURATION_230 | ??? |
| LINK_LOW_SATURATION_260 | ??? |
| LINK_LOW_SATURATION_300 | ??? |
| LINK_LOW_SATURATION_330 | ??? |
| LINK_LOW_SATURATION_360 | ??? |
| LINK_LOW_SATURATION_400 | ??? |
| LINK_LOW_SATURATION_430 | ??? |
| LINK_LOW_SATURATION_460 | ??? |
| LINK_LOW_SATURATION_500 | ??? |
| LINK_LOW_SATURATION | ??? |
| LINK_LOW_SATURATION_530 | ??? |
| LINK_LOW_SATURATION_560 | ??? |
| LINK_LOW_SATURATION_600 | ??? |
| LINK_LOW_SATURATION_630 | ??? |
| LINK_LOW_SATURATION_660 | ??? |
| LINK_LOW_SATURATION_700 | ??? |
| LINK_LOW_SATURATION_730 | ??? |
| LINK_LOW_SATURATION_760 | ??? |
| LINK_LOW_SATURATION_800 | ??? |
| LINK_LOW_SATURATION_830 | ??? |
| LINK_LOW_SATURATION_860 | ??? |
| LINK_LOW_SATURATION_900 | ??? |
| LINK_LIGHT_100 | ??? |
| LINK_LIGHT_130 | ??? |
| LINK_LIGHT_160 | ??? |
| LINK_LIGHT_200 | ??? |
| LINK_LIGHT_230 | ??? |
| LINK_LIGHT_260 | ??? |
| LINK_LIGHT_300 | ??? |
| LINK_LIGHT_330 | ??? |
| LINK_LIGHT_360 | ??? |
| LINK_LIGHT_400 | ??? |
| LINK_LIGHT_430 | ??? |
| LINK_LIGHT_460 | ??? |
| LINK_LIGHT_500 | ??? |
| LINK_LIGHT | ??? |
| LINK_LIGHT_530 | ??? |
| LINK_LIGHT_560 | ??? |
| LINK_LIGHT_600 | ??? |
| LINK_LIGHT_630 | ??? |
| LINK_LIGHT_660 | ??? |
| LINK_LIGHT_700 | ??? |
| LINK_LIGHT_730 | ??? |
| LINK_LIGHT_760 | ??? |
| LINK_LIGHT_800 | ??? |
| LINK_LIGHT_830 | ??? |
| LINK_LIGHT_860 | ??? |
| LINK_LIGHT_900 | ??? |
| PREMIUM_TIER_2_PURPLE_500 | ??? |
| PREMIUM_TIER_2_PURPLE | ??? |
| PREMIUM_TIER_2_PINK_500 | ??? |
| PREMIUM_TIER_2_PINK | ??? |
| PREMIUM_TIER_1_PURPLE_500 | ??? |
| PREMIUM_TIER_1_PURPLE | ??? |
| PREMIUM_TIER_1_BLUE_500 | ??? |
| PREMIUM_TIER_1_BLUE | ??? |
| PREMIUM_GUILD_PINK_500 | ??? |
| PREMIUM_GUILD_PINK | ??? |
| PREMIUM_GUILD_PURPLE_500 | ??? |
| PREMIUM_GUILD_PURPLE | ??? |
| PREMIUM_GUILD_BLUE_500 | ??? |
| PREMIUM_GUILD_BLUE | ??? |
| CREATOR_REVENUE_START_500 | ??? |
| CREATOR_REVENUE_START | ??? |
| CREATOR_REVENUE_END_500 | ??? |
| CREATOR_REVENUE_END | ??? |
| HYPESQUAD_HOUSE_1_500 | ??? |
| HYPESQUAD_HOUSE_1 | ??? |
| HYPESQUAD_HOUSE_2_500 | ??? |
| HYPESQUAD_HOUSE_2 | ??? |
| HYPESQUAD_HOUSE_3_500 | ??? |
| HYPESQUAD_HOUSE_3 | ??? |
| GOLD_500 | ??? |
| GOLD | ??? |
| PARTNER_500 | ??? |
| PARTNER | ??? |
| SKYPE_500 | ??? |
| SKYPE | ??? |
| BATTLENET_500 | ??? |
| BATTLENET | ??? |
| STEAM_500 | ??? |
| STEAM | ??? |
| LOL_500 | ??? |
| LOL | ??? |
| TWITCH_500 | ??? |
| TWITCH | ??? |
| YOUTUBE_500 | ??? |
| YOUTUBE | ??? |
| TWITTER_500 | ??? |
| TWITTER | ??? |
| REDDIT_500 | ??? |
| REDDIT | ??? |
| SPOTIFY_500 | ??? |
| SPOTIFY | ??? |
| FACEBOOK_500 | ??? |
| FACEBOOK | ??? |
| SAMSUNG_500 | ??? |
| SAMSUNG | ??? |
| XBOX_500 | ??? |
| XBOX | ??? |
| GITHUB_500 | ??? |
| GITHUB | ??? |
| TRANSPARENT | ??? |
</details>

[Back to Top](#)
