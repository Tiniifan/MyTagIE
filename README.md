# MyTagIE

MyTagIE provides enhanced tag definitions for editing .cfg.bin files using CfgBinEditor.  
These binary configuration files contain game data such as player statistics, team information, and other game parameters.

## Overview

.cfg.bin files can be automatically modified using [Lynx](https://github.com/Tiniifan/Lynx), but when you need to modify unsupported files or make custom modifications,  
manual editing is required using [CfgBinEditor](https://github.com/onepiecefreak3/CfgBinEditor/) by onepiecefreak3.

## Installation

1. Download and install CfgBinEditor
2. Download the `MyTags.txt` file from this repository
3. Place `MyTags.txt` in the same directory as `CfgBinEditor.exe`
4. Launch CfgBinEditor and open your .cfg.bin file
5. Use the tag selector to choose the appropriate tag for your file

## Usage

When you first open a .cfg.bin file in CfgBinEditor without the MyTags.txt file, you'll see a list of meaningless numerical values:

![CfgBinEditor without tags](https://github.com/user-attachments/assets/34c4d846-f2a8-46e5-b627-1452f5a26ba2)

You need to close CfgBinEditor, download the MyTags.txt file from this repository and place it in the same folder as CfgBinEditor.exe:

![File placement](https://github.com/user-attachments/assets/14234ade-6413-4181-905c-4fce7116d3e6)

After installing MyTags.txt and selecting the appropriate tag, the values will be displayed with meaningful field names, making manual editing much more intuitive.

### Steps:
1. Open CfgBinEditor
2. Load your .cfg.bin file
3. Click on the tag selector dropdown:

![Tag selector](https://github.com/user-attachments/assets/8244986f-3470-464c-82b3-210a8d5a230e)

4. Choose the appropriate tag for your file type
5. Begin editing with labeled field names:

![Labeled fields](https://github.com/user-attachments/assets/a43f08d2-00d3-428d-9d28-a7f33facf168)

## Supported Tags

### IEGO
| Tag Name | Description | File |
|----------|-------------|------|
| NPC_BASE | Base NPC configuration data | [mapID].npc.bin |
| NPC_PRESET | allows you to link NPC_BASE and NPC_APPEAR | [mapID].npc.bin |
| NPC_APPEAR | the position and conditions of appearance of the NPC | [mapID].npc.bin |
| CHARA_BASE_INFO | Character base information | chara_base.cfg.bin |
| CHARA_PARAM_INFO | Character player data | chara_param.cfg.bin |
| TALK_INFO | Dialog system information | [mapID].talk.bin |
| TALK_CONFIG | Dialog configuration settings | [mapID].talk.bin |
| SKILL_CONFIG_INFO | Skill configuration data | skill_config.cfg.bin |
| SKILL_INDEX | Skill index data | skill_config.cfg.bin |
| SOCCER_INFO | Soccer match information | soccer_config.cfg.bin |
| ROUTE_CONFIG | Competitive route configuration | scr_br_XXXX.cfg.bin |
| ROUTE_CONFIG_BEGIN | Competitive route configuration header | scr_br_XXXX.cfg.bin |
| STORY_TEAM_INFO | Match team data (name, player, ...) | team_config.cfg.bin |
| ENCOUNT_TEAM_INFO | Mini battle team data (name, player, ...)  | team_config.cfg.bin |
| TEAM_PARAM_INFO | Team param data (teamConfigID used, level, coach, ...) | team_param.cfg.bin |
| NOUN_INFO | Noun entries | any text file |
| TEXT_INFO | Text entries | any text file |
| TEXT_WASHA | Text Washa data | any text file  |
| TEXT_CONFIG | Text configuration (to select the speaker) | any text file  |
| ITEM_EQUIPMENT | Equipment item data | item_config.cfg.bin|
| ITEM_CONSUME | Consumable item data | item_config.cfg.bin |
| ITEM_IMPORTANT | Important item data | item_config.cfg.bin |
| ITEM_UNIFORM | Uniform item data | item_config.cfg.bin |
| ITEM_KIZUNAX | Kizunax item data | item_config.cfg.bin |
| ITEM_AVATAR | Avatar item data | item_config.cfg.bin |
| ITEM_DIRECTOR | Coach item data | item_config.cfg.bin |
| ITEM_REF | Item reference data | item_config.cfg.bin |
| PASSWORD_CONFIG | Password configuration | password_config.cfg.bin |
| PASSWORD_CONFIG_BEGIN | Password configuration header | password_config.cfg.bin |
| SHOP_CONFIG_INFO | Shop configuration data | shop_shpXXXX.cfg.bin |
| SHOP_CONFIG_INFO_BEGIN | Shop configuration header | shop_shpXXXX.cfg.bin |
| VALUE_INFO | ??? | ??? |
| FORM_INFO | Formation information | btl_fm.cfg.bin and btl_fmXXXX.cfg.bin |
| ENCOUNT_INFO | Encounter information | graphic_font_config.cfg.bin |
| GFONT_CONFIG | Font configuration | graphic_font_config.cfg.bin |
| KERNING | Kerning Font settings | graphic_font_config.cfg.bin |
| KERNING_CONFIG | Kerning Font configuration | graphic_font_config.cfg.bin |

### IEGOGalaxy
| Tag Name | Description | File |
|----------|-------------|------|
| STORY_TEAM_INFO | Team param data (teamConfigID used, level, coach, ...) | team_param.cfg.bin |

## Contributing

If your game or file type is not currently supported, or if you discover new field mappings, you can create your own tags and submit them for inclusion in this
