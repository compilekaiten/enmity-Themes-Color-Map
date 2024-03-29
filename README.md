# Enmity Theme Color Map
> This is updated for Discord **v164.0** and Enmity **v2.1.4**

> This list will **NOT** work for Discord v165.0 or above. Wait for Enmity 3.0.

Document Compiled by: [notNeo#4932]()

Research: [sudo#1469](https://github.com/sudo9000)

JSON Schema: [beerpsi#5270](https://github.com/beerpiss)

PR: [rens#3405](https://github.com/T7a9)

- - - -

### Please PR, if you have found any other keys/values/descriptions... i'm lazy

- - - -

- [Enmity Theme Color Map](#enmity-theme-color-map)
  - [**Details**](#details)
  - [**Format**](#format)
  - [**Theme `Information` Block**](#theme-information-block)
      - [Information about your theme](#information-about-your-theme)
  - [**`authors` object**](#authors-object)
      - [Theme Authors Information](#theme-authors-information)
  - [**`background` object**](#background-object)
      - [Main Chat Background Images](#main-chat-background-images)
  - [**`theme_color_map` object**](#theme_color_map-object)
      - [Background Properties](#background-properties)
      - [Text Colors](#text-colors)
  - [**`colours` object**](#colours-object)
      - [Colors used throughout Discord](#colors-used-throughout-discord)
  - [**`unsafe_colors` object**](#unsafe_colors-object)
      - [Used to theme the annoying grey bottom bar (homebar area)](#used-to-theme-the-annoying-grey-bottom-bar-homebar-area)
  - [**`Unknowns`**](#unknowns)
      - [**Long** list of unknown properties.](#long-list-of-unknown-properties)
      - [**`theme_color_map` object unknown**](#theme_color_map-object-unknown)
      - [**`colors` object unknown**](#colors-object-unknown)
  
- - - -

## **Details**
* This a _semi-organized_ list of the iOS Discord Theme Color Map.

* Many Properties __overlap__ each other. Some compromises have to be made when themeing.

- - - -

## **Format**
> [Check the example template here](example.json)

> [A JSON Schema created by beerpiss, is available here](https://beerpiss.github.io/enmity-theme-schema/enmity-theme.schema.json)
>> [Human readable Schema Doc Page](https://beerpiss.github.io/enmity-theme-schema/)

The `name` string is case sensitive, and *MUST* match your final filename.
  - `"name": "example",` === `example.json`

Strings inside the `authors` object should be the following:
* `name` --> The name you want displayed in Enmity's Theme Settings
* `id` --> Your **Unique** discord ID. Google how to get it.

The `background` object can have the following values:
* `blur` --> Integer between 0 - 20
* `url` --> The Direct URL to your background image. Leave blank for no image background
* `alpha` --> Integer value

`theme_color_map` keys have two values, seperated by a comma. One for Dark Mode, and one for Light Mode. **Both must be present!**

Color codes inside the `theme_color_map` and `colours` object can be the following:
* 6 character HEX --> `#RRGGBB`
  * Enmity can also take 8 character HEX --> `#RRGGBBAA`, but the ALPHA value is ignored
* CSS `rgba()` --> `rgba(0, 0, 0, 1)`
  * **[ ! ]** `rbga()` needs to follow the above format exactly. You **cannot** use `rgba(r g b a)` or `rgba(r g b / a)`
* A `transparent` string can also be used

Example:
```json
{
  "name": "example",
  "version": "4.2.0",
  "description": "Ugly theme... Now with BLUR!",
  "color": "#FFFFFF",
  "authors": [
    {
      "name": "NEO",
      "id": "424806150702366723"
    }
  ],
  "background": {
    "blur": 1,
    "url": "https://i.imgur.com/sEkjODE.jpeg",
    "alpha": 0.69
  },
  "theme_color_map": {
    "BACKGROUND_PRIMARY": ["#000000", "#FFFFFF"],
                        //Dark Mode , //Light Mode
    "BACKGROUND_SECONDARY": ["rgba(0, 0, 0, 1)", "rgba(255, 255, 255, 1)"],
  },
  "colours": {
    "PRIMARY_DARK": "#0F0FFF",
    "BRAND_NEW": "transparent",
  },
  "unsafe_colors": {
    "CHAT_GREY": "#000000"
  }
}
```
- - - -

# If you are confused by my medicore descriptions, I recommend you check out the theme [Bozo The Clown by Sudo](https://github.com/sudo9000/Enmity-Themes/blob/main/BozoTheClown.json). Each key has a different color, so it's easy to see what themes what.

- - - -

## **Theme `Information` Block**
[Back to Top](#)
#### Information about your theme
> General Information About your Theme

| Property        | Description       |
|:--------------- | :---------------: |
| name            | Theme Name        |
| version         | Versioning        |
| description     | Short Theme Description |
| color           | Enmity Settings Theme Color Bar |

- - - -

## **`authors` object**
[Back to Top](#)
#### Theme Authors Information
> Theme Author information. Used in Enmity's Theme Settings
> 
| Property        | Description       |
|:--------------- | :---------------: |
| name            | Theme Author Name |
| id              | Your unique Discord ID |

- - - -

## **`background` object**
[Back to Top](#)
#### Main Chat Background Images
> Customize custom theme background images
> 
| Property        | Description       |
| --------------- | :---------------: |
| blur            | Blur Amount to apply to the image |
| url             | Direct URL to image |
| alpha           | Alpha value to apply to the image |

- - - -

## **`theme_color_map` object**
[Back to Top](#)
#### Background Properties
> Properties that theme most background elements

| Property | Description |
|:--------------- | :---------------: |
| KEYBOARD | Global keyboard background color |
| BACKGROUND_PRIMARY | Main Chat Background [DMs, Channels, User List, Friends Tab, Search Tab, Mentions Tab], User Options Boxes Background [Mutual Servers, Friends, etc], Any pop up options boxes background |
| BACKGROUND_SECONDARY | Top Left button background, Join Server Button Background, Friends Call and Message button background, Missed Call Background, Reply to Bar, Codeblock background, Profile Bottom background, Server Info Bottom background, Reactions background, Embed Background, Slash Command Top bar, @user background, Emoji/GIF/Sticker Picker background |
| BACKGROUND_SECONDARY_ALT | Profile Notes background, About Me background, Chat Input background [Add Files, Gift Buttons], Emoji/GIF/Sticker slider background |
| BACKGROUND_TERTIARY | Global Border background when elements are slide out [Server List, User List], Search Bar background, Profile [About Me and Notes outline], Spoilers background, Top bar seperator when in channel, Settings options boxes seperator, Three Dots Button [Profiles, Search] |
| BACKGROUND_ACCENT | Reply Pipe, Edit user Profile button, Album Buttons, Thread Buttons, Sometimes flashes this color when stuff loads |
| BACKGROUND_FLOATING | Profile Top background, Server Boost Page Icons |
| BACKGROUND_NESTED_FLOATING | Settings buttons/boxes background |
| BACKGROUND_MOBILE_PRIMARY | Account/Settings background |
| BACKGROUND_MOBILE_SECONDARY | Channel List/DM Background, Global Header Color, User Status [Online, Away, DND, Offline] Background in chat input |
| BACKGROUND_MODIFIER_ACCENT | Seperators [Server List Top, Bottom Bar, Server Info, User List, User Info, @,  Notifications, Friends, Search, Settings] |
| BACKGROUND_MODIFIER_ACTIVE | Background color when clicking/holding a button [DM User, Channel, Server, Rectangle Buttons] |
| BACKGROUND_MODIFIER_SELECTED | Background color of selected User or Channel |
| CHANNELS_DEFAULT | Unselected DM User text color[including status], Server Category text color |
| HEADER_PRIMARY | Top Bar Text Color [Direct Messages, DM User name, Server Name, Channel name, User list, Friends Tab, Mentions Tab & channel name text, Settings titles], Server Info Name, User info name, Follow channels text, Invite members text, slash command text, Some pop-up text (add theme) |
| HEADER_SECONDARY | User Discord ID #s, User Text [Connections, About me, Notes], Server description [online and member count], User list status text [Listening, playing, etc], User list subtitles, Slash Command subtitles, Search titles, Most settings titles |
| INTERACTIVE_ACTIVE | Selected Server bar, Selected user text DMs, Selected Channel text, Unread Channel text and dot, @ user name text, # channel text, bottom bar icon fill, some random titles |
| INTERACTIVE_MUTED | Unselected muted channel text, block quote bar |
| INTERACTIVE_NORMAL | Button/Glyph accent colors [Top left button glyph, 3 bars, Call, Video, User list], User list [Threads, Pins, Notifs, Settings, Role names], User Info [Message, Call, Video], Server Info [Boost Text, Invite, Notifs], Channel [Search, User list, Add Files, Gift, Emoji buttons, add reactions], Slash Command title, Emoji bottom bar glyph color, # channel glyphs], bottom bar inactive icon fill, incoming typing member text |

#### Text Colors
> Properties that theme most text colors

| Property | Description |
|:--------------- | :---------------: |
| TEXT_DANGER | Enmity Theme/Plugin Uninstall text |
| TEXT_LINK | Link text global |
| TEXT_MUTED | Search bar text, timestamp, chat input text, @ user #id, Slash command owner text, Symbols [@, Lock, # (except muted channels)], various subtitles [settings, server info], Emoji/GIF/Stickers slider text |
| TEXT_NORMAL | Global text color [DMs, Channels, Typing text, Server info boxes text, User info boxes text, Settings text] |
| CHANNEL_ICON | Chat input text, Symbols [@, Lock, # (except muted channels)] |

## **`colours` object**

[Back to Top](#)
#### Colors used throughout Discord
> Some Properties overlap with the color map.

| Property | Description |
|:--------------- | :---------------: |
| PRIMARY_DARK | Profile Notes text, Popup box seperators|
| PRIMARY_DARK_100 | Popup text color [Enmity Apply], Search bar cursor color |
| PRIMARY_DARK_300 | Grabber Color, ? Glyph Color, No Pinned messages text, Channel Settings channel name, Connections text |
| PRIMARY_DARK_360 | Unselected and unread and unmuted channel name text |
| PRIMARY_DARK_400 | Different Day Message seperator, Search tab subtext, 2FA text, 'New Unreads' banner, @ user name text color |
| PRIMARY_DARK_500 | Invite Button background, User Watch Live button, Default (grey) Role circle color, "Public" server button |
| PRIMARY_DARK_600 | Chat Input Border Background fill, Global? pop up background [Enmity apply] |
| PRIMARY_DARK_630 | Hold/Click on message background, Slash Command background, Search in Channel background, Spotify Now playing scrubber bar, "Ring" around the ping |
| PRIMARY_DARK_700 | Top and Bottom bar Seperators, Global Toast Background, Role Background color, Side of screen flashes this color sometimes ??? |
| PRIMARY_DARK_800 | The Entire Bottom bar (and homebar) [Discord Icon, People Icon, Profile, etc.], Tints GIF categories in search |
| BRAND_NEW | Top left button background, New message Top banner, Floating new message banner progress bar, Global Switch color, Send button background, bot tag background, add to server button |
| BRAND_NEW_360 | "Get Nitro" text in settings, Reply mention "on" button |
| WHITE | Top Left button icon fill, DMs username text, Server invite button text, No Role or default color role (grey) username color, User profile role text color, global spinners, Send button glyph, global cursor color, bot tag text color, add files button text color, GIF text, server with banner text and 3 dots, public server text, channel search text, (edited text subscript), follow channel text color |
| STATUS_GREEN_600 | Green Elements ( Create/Add Server Icon color, Nitro Settings Buttons) |
| <s>STATUS_YELLOW</s> | <s>Mentions Colors (Side Bar and Tint)</s> Not hooked yet. Doesn't work |
| STATUS_RED | Ping colors, "Remove from favorites" button in emoji settings |
| STATUS_RED/GREEN/GREY/ORANGE 100-900 | Various colored elements like logout text, security text. *Many of These need to be hooked to work* |

## **`unsafe_colors` object**
[Back to Top](#)
#### Used to theme the annoying grey bottom bar (homebar area)

| Property | Description |
|:--------------- | :---------------: |
| CHAT_GREY | Homebar grey bar |

## **`Unknowns`**
[Back to Top](#)
#### **Long** list of unknown properties. 
> Some of these just don't do anything, or I couldn't find what they changed.
>> If you can figure these out, let me know


<details>
  <summary>Expand Me!</summary>
  
  #### **`theme_color_map` object unknown**
| Property | Description |
|:--------------- | :---------------: |
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

#### **`colors` object unknown**

| Property | Description |
|:--------------- | :---------------: |
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
