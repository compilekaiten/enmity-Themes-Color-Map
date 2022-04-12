# Enmity Theme Color Map
Created by: NEO#7154

If you have any new findings you want listed here, contact me on discord.

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
 }
```
- - - -

## **"theme_color_map" object**

#### Background Properties
> Properties that theme most background elements

| Property | Description |
| --------------- | :---------------: |
| BACKGROUND_PRIMARY | Background (Search, Mentions, Channel, Channel Info, Invite UI, Set Status, User List, Threads, Notifications, Behind the keyboard *looks sick yo*) |
| BACKGROUND_SECONDARY | Profile background, Server info background, Slash Command Top bar, Button Backgrounds (Server List, Reactions), Embed Background, Code Blocks, Call background in chat |
| BACKGROUND_SECONDARY_ALT | Profile Notes background, About Me background, Embed Background, Reactions Background, Message Input Background, Missed Call/etc |
| BACKGROUND_TERTIARY | Background background BACKGROUND (server list and around things), Search bar background, spoilers, Top bar seperator, About me and Notes outline, three dots button |
| BACKGROUND_ACCENT | Reply Pipe, Album Buttons, Thread Buttons, Flashes this color when some stuff loads |
| BACKGROUND_FLOATING | Profile background, Server Boost Page Icons |
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
| STATUS_RED -> RED_900 | One of these changes the logout text color. lmao good luck |
| WHITE | Global Cursor, DMs username text, Add Files button colors, GIF text, Send button glyph, Server Name and 3 dots text, Invite Text, Role Text color, Video/Picture controls, Channel Search text |
